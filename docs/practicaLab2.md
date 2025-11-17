# 🧬 Práctica de Laboratorio 2 — Ficheros

Esta práctica aborda el manejo, lectura y procesamiento de ficheros en bioinformática utilizando Python y Biopython. A lo largo del trabajo se desarrollan ejercicios orientados al tratamiento de secuencias biológicas reales en formato FASTA, así como la descarga y visualización de estructuras proteicas en formato PDB. Además, se incorporan representaciones interactivas con `py3Dmol` para explorar modelos tridimensionales de proteínas.

---

## Descarga del ZIP del proyecto

Haz clic para obtener el paquete completo del proyecto:

➡️ **[Descargar ZIP](./P2_Ficheros_G9_Gisela_Diego.zip)**

---

## Repositorio oficial

Puedes consultar el repositorio completo aquí:

- **Práctica de Laboratorio 2**: https://github.com/giselabcruz/P2_Ficheros

---

## Ejercicio 1 — Manejo de secuencias FASTA

En este ejercicio se realizó el procesamiento de secuencias de ADN en formato FASTA mediante Python. Entre las tareas desarrolladas se encuentran:

#### ✔ Lectura de secuencias de ADN desde un archivo FASTA  
#### ✔ Cálculo del contenido GC  
#### ✔ Traducción automática ADN → proteína  
#### ✔ Escritura de las proteínas generadas en un nuevo archivo FASTA  
#### ✔ Visualizaciones complementarias (histogramas, comparativas, etc.)

**Archivos utilizados:**

- **Entrada:** `input/dna_seqs.fasta`  
- **Salida:** `output/proteins.fasta`

---

## Ejercicio 2 — Búsqueda y visualización de proteínas

En este apartado se trabajó con ficheros PDB y visualización 3D con `py3Dmol` de proteínas obtenidas del Protein Data Bank.

Proteínas analizadas:

- **Oxitocina** — PDB: *1NPO*  
- **Colágeno** — PDB: *1CAG*  
- **Queratina** — PDB: *4ZRY*


<style>
.card-grid {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 24px;
  margin-top: 1.8em;
}

.card {
  background: linear-gradient(145deg, #f5f7ff, #e6e9ff);
  border-radius: 18px;
  padding: 16px 16px 18px;
  width: 220px;
  text-align: center;
  box-shadow: 0 6px 18px rgba(10, 20, 60, 0.18);
  transition: transform 0.25s ease, box-shadow 0.25s ease, background 0.25s ease;
  border: 1px solid rgba(120, 130, 200, 0.18);
}

.card:hover {
  transform: translateY(-8px) scale(1.02);
  box-shadow: 0 14px 30px rgba(10, 20, 60, 0.28);
  background: linear-gradient(145deg, #eef1ff, #dde2ff);
}

.card img {
  border-radius: 14px;
  width: 100%;
  display: block;
  box-shadow: 0 4px 14px rgba(0,0,0,0.25);
  margin-bottom: 10px;
  transition: transform 0.25s ease, box-shadow 0.25s ease;
}

.card:hover img {
  transform: scale(1.03);
  box-shadow: 0 6px 18px rgba(0,0,0,0.30);
}

.card h4 {
  margin: 0.2em 0 0;
  font-size: 1.05rem;
  letter-spacing: 0.02em;
}
</style>

<div class="card-grid">

  <div class="card">
    <img src="../protein_gifs/colageno.gif" alt="Colágeno">
    <h4>Colágeno</h4>
  </div>

  <div class="card">
    <img src="../protein_gifs/queratina.gif" alt="Queratina">
    <h4>Queratina</h4>
  </div>

  <div class="card">
    <img src="../protein_gifs/oxitocina.gif" alt="Oxitocina">
    <h4>Oxitocina</h4>
  </div>

</div>


---

