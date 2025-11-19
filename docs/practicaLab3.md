# 🧬 Práctica de Laboratorio 3 — Alineamientos de Proteínas

## ***Repositorio oficial de GitHub***

Puedes consultar el repositorio completo aquí:

- https://github.com/giselabcruz/P3_Alineamientos


## Objetivo de la práctica

Aplicar la clase **`PairwiseAligner`** de *Biopython* para alinear secuencias de **aminoácidos** y analizar cómo varían los resultados según el origen de las secuencias y la matriz de sustitución empleada.

---

## Enunciado

Implementa un programa en Python que realice alineamientos de proteínas en dos escenarios distintos:

---

### **a) Generación automática de secuencias aleatorias**
- Crear secuencias de aminoácidos **de manera automática**, sin intervención manual.
- Utilizar `PairwiseAligner` para obtener:
  - El alineamiento óptimo.
  - La puntuación total (*score*).
  - Métricas adicionales como porcentaje de identidad o número de coincidencias.

---

### **b) Alineamiento usando secuencias reales obtenidas de bases de datos**
- Descargar secuencias reales desde **UniProt** u otras bases de datos biológicas.
- Guardar las secuencias en formato **FASTA**.
- Explicar cómo se obtuvieron:
  - Buscar la proteína en UniProt.
  - Acceder a la entrada correspondiente.
  - Seleccionar **Download → FASTA**.
  - Guardar los archivos en tu carpeta de trabajo.

---

## Comparación de matrices de sustitución

Realiza el alineamiento empleando distintas matrices, comparando resultados, ventajas y limitaciones:

- **BLOSUM62** → estándar para secuencias moderadamente divergentes.  
- **PAM250** → adecuada para secuencias muy evolucionadas (divergentes).  
- **Matriz personalizada** → permite explorar penalizaciones distintas y analizar su impacto.

Incluye una reflexión comparando:
- Cambios en la puntuación.
- Alteraciones en la longitud del alineamiento.
- Sensibilidad de cada matriz según el tipo de secuencia.

---

## Descarga el ZIP del proyecto

Haz clic para obtener el paquete completo del proyecto:

➡️ **[Descargar ZIP](./P3_Alineamientos_G9_Gisela_Diego.zip)**


---

