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

<table>
  <tr>
    <th>Oxitocina</th>
    <th>Colágeno</th>
    <th>Queratina</th>
  </tr>
  <tr>
    <td><img src="../protein_gifs/oxitocina.gif" width="260"/></td>
    <td><img src="../protein_gifs/colageno.gif" width="260"/></td>
    <td><img src="../protein_gifs/keratina.gif" width="260"/></td>
  </tr>
</table>