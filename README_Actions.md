# Publicación automática con GitHub Actions (MkDocs → GitHub Pages)

Este documento explica **cómo automatizar** la construcción y el despliegue del sitio de la práctica usando **GitHub Actions** y **GitHub Pages**.

---

## 1) Prerrequisitos

- Estructura de MkDocs en el repo:
  - `mkdocs.yml` en la raíz
  - Carpeta `docs/` con el contenido
- Python 3.10+ recomendado (solo para pruebas locales)
- (Opcional) `requirements.txt` con:
  ```txt
  mkdocs>=1.5
  mkdocs-material>=9.5
  ```

---

## 2) Crear el workflow

Crea la carpeta (si no existe):

```
.github/workflows/
```

Dentro, crea el fichero:

```
.github/workflows/deploy.yml
```

### Contenido del workflow (comentado)

```yaml
name: Deploy MkDocs site to GitHub Pages

on:
  push:
    branches: [ main ]   # Ejecuta al subir cambios a la rama 'main' (ajusta si usas otra)

permissions:
  contents: read         # Permiso de lectura del repo (para checkout)
  pages: write           # Necesario para publicar en GitHub Pages
  id-token: write        # Requisito para autenticación OIDC en despliegue

jobs:
  build-deploy:
    runs-on: ubuntu-latest

    steps:
      - name: Checkout
        uses: actions/checkout@v4    # Trae el código del repo al runner

      - name: Set up Python
        uses: actions/setup-python@v5
        with:
          python-version: '3.11'     # Versión de Python del runner

      # Instala MkDocs y el tema Material
      # Si tienes requirements.txt, sustituye por: pip install -r requirements.txt
      - name: Install dependencies
        run: |
          python -m pip install --upgrade pip
          pip install mkdocs mkdocs-material

      # Construye el sitio en la carpeta 'site'
      - name: Build MkDocs site
        run: mkdocs build --strict

      # Sube el sitio construido como artefacto para Pages
      - name: Upload artifact
        uses: actions/upload-pages-artifact@v3
        with:
          path: site

      # Despliega en GitHub Pages
      - name: Deploy to GitHub Pages
        uses: actions/deploy-pages@v4
```

---

## 3) Activar GitHub Pages

1. Ve a **Settings → Pages** en tu repositorio.  
2. En **Build and deployment**, elige **GitHub Actions**.  
3. Guarda.

Tras el siguiente **push a `main`**, se publicará en:
```
https://<usuario>.github.io/<repositorio>/
```

---

## 4) Validación local (opcional)

```bash
pip install -r requirements.txt   # o instala mkdocs y mkdocs-material
mkdocs serve                     # abre http://127.0.0.1:8000
mkdocs build --strict            # verifica que compila sin errores
```

---

## 5) Problemas comunes (y cómo resolverlos)

- **Falta `mkdocs.yml` o `docs/`**  
  → El build fallará. Asegúrate de que ambos existen en la raíz del repo.
- **No se publica la web**  
  → Revisa que en *Settings → Pages* está seleccionado **GitHub Actions**.
- **Imágenes no se ven**  
  → Usa rutas relativas correctas: `![alt](img/practica1/captura.png)` si la imagen está en `docs/img/practica1/`.
- **El workflow pasa pero la URL da 404**  
  → Espera ~1–2 minutos tras el deploy y purga caché del navegador; revisa la pestaña **Actions** por errores.

---

## 6) Checklist para la entrega

- [ ] He añadido / verificado `mkdocs.yml` y `docs/`.
- [ ] He creado `.github/workflows/deploy.yml` con el contenido correcto.
- [ ] He activado **GitHub Pages → GitHub Actions** en Settings.
- [ ] `mkdocs build --strict` funciona en local (opcional).
- [ ] Puedo abrir la URL pública tras el push a `main`.


---

## Flujo real

1. Editas algo en local (por ejemplo docs/practica1.md o mkdocs.yml).
2. Haces commit y push a la rama configurada en el workflow (ej: main).

'''bash
git add .
git commit -m "Actualizo práctica 1"
git push origin main

'''

3. GitHub detecta el push en main y lanza automáticamente el workflow en la pestaña Actions del repositorio.
4. El workflow:  
- Instala MkDocs  
- Genera el sitio con mkdocs build  
- Sube el artefacto  
- Lo despliega en GitHub Pages  
5. Tras unos segundos/minutos, los cambios se ven en: https://<usuario>.github.io/<repositorio>/

