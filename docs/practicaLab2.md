# 🧬 Práctica de Laboratorio 2 — Ficheros

Esta práctica se centra en el manejo, lectura y procesamiento de ficheros en bioinformática, especialmente utilizando Python y Biopython. A lo largo del trabajo se desarrollan ejercicios que permiten trabajar con secuencias biológicas reales (FASTA) y estructuras proteicas (PDB), así como visualizaciones interactivas mediante `py3Dmol`.
 
---

## Descarga del ZIP del proyecto

➡️ [Descargar ZIP](./P2_Ficheros_G9_Gisela_Diego.zip)

---

## Repositorio

- **Práctica de Laboratorio 2**: [https://github.com/giselabcruz/P2_Ficheros](https://github.com/giselabcruz/P2_Ficheros)

---

## Ejercicio 1 — Manejo de secuencias FASTA

En este ejercicio se trabaja sobre ficheros FASTA mediante Python. Las tareas realizadas fueron:

#### ✔ Lectura de secuencias de ADN desde un archivo FASTA  
#### ✔ Cálculo del contenido GC  
#### ✔ Traducción automática ADN → proteína  
#### ✔ Escritura de las secuencias traducidas en un nuevo archivo FASTA  
#### ✔ Representación gráfica (histogramas, comparaciones, etc.)

**Archivos usados:**

- Entrada: `input/dna_seqs.fasta`  
- Salida: `output/proteins.fasta`  

---

## Ejercicio 2 — Búsqueda y visualización de proteínas

Este ejercicio se centra en el trabajo con ficheros PDB y visualización estructural.

#### ✔ Descarga de secuencias reales en formato FASTA  
#### ✔ Recuperación de estructuras 3D reales desde el Protein Data Bank (PDB)  
Proteínas utilizadas:

- **Oxitocina** — PDB: *1NPO*  
- **Colágeno** — PDB: *1CAG*  
- **Queratina** — PDB: *4ZRY*

#### ✔ Visualización 3D con `py3Dmol`

<style>
.card-grid {
  display: flex;
  justify-content: center;
  gap: 20px;
  margin-top: 1.5em;
}

.card {
  background: linear-gradient(145deg, #f9f9ff, #ececff);
  border-radius: 16px;
  padding: 18px;
  width: 200px;
  text-align: center;
  box-shadow: 0 4px 14px rgba(0,0,50,0.15);
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.card:hover {
  transform: translateY(-6px);
  box-shadow: 0 10px 25px rgba(0,0,50,0.25);
}

.card img {
  border-radius: 12px;
  width: 100%;
  box-shadow: 0 3px 10px rgba(0,0,0,0.2);
  margin-top: 10px;
}
</style>

<div class="card-grid">

  <div class="card">
    <h4>Colágeno</h4>
    <img src="../protein_gifs/colageno.gif" alt="Colágeno">
  </div>

  <div class="card">
    <h4>Queratina</h4>
    <img src="../protein_gifs/queratina.gif" alt="Queratina">
  </div>

  <div class="card">
    <h4>Oxitocina</h4>
    <img src="../protein_gifs/oxitocina.gif" alt="Oxitocina">
  </div>

</div>