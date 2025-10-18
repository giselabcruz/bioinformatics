# 🧬 Práctica de Aula 4 – Algoritmos de Brujin

---

### Descripción del trabajo realizado

Este informe presenta el desarrollo de tres ejercicios prácticos enfocados en los **algoritmos de Brujin**, aplicados al **ensamblaje de secuencias de ADN** a partir de fragmentos cortos.  
El objetivo principal fue comprender el funcionamiento de los grafos de Brujin como herramienta bioinformática en los métodos modernos de **secuenciación genómica**.

A lo largo de la práctica se abordaron tres escenarios complementarios:

- **Cuestión 1:** Se partió de un conjunto de fragmentos de ADN y se construyó el grafo de Brujin a partir de sus prefijos y sufijos de longitud \(k-1\), observando cómo las lecturas se conectaban mediante aristas que representaban las superposiciones entre fragmentos.  
- **Cuestión 2:** Se elaboró un nuevo grafo con diferentes lecturas, logrando encontrar un **camino euleriano** que permitió reconstruir la secuencia original de ADN.  
- **Cuestión 3:** Se analizó un caso con **repeticiones y ambigüedades**, donde no fue posible determinar un único camino euleriano, reflexionando sobre las causas y posibles soluciones, como variar la longitud de \(k\) o emplear técnicas complementarias.

El conjunto de ejercicios permitió demostrar tanto la potencia como las limitaciones de estos algoritmos en el ensamblaje de genomas.

---

## Visualización de los ejercicios

[📄 **Abrir informe completo en PDF**](Algoritmos_de_Brujin_Gisela_Diego.pdf)

<style>
.pdf-embed {
  position: relative;
  width: 100%;
  padding-top: 70%; /* altura dinámica */
  margin-top: 1em;
  border-radius: 10px;
  box-shadow: 0 4px 12px rgba(0,0,0,0.15);
  overflow: hidden;
}
.pdf-embed iframe,
.pdf-embed object {
  position: absolute;
  top: 0; left: 0;
  width: 100%; height: 100%;
  border: none;
}
.pdf-fallback {
  text-align: center;
  font-style: italic;
  color: #555;
  margin-top: 1em;
}
</style>

<div class="pdf-embed">
  <object data="Algoritmos_de_Brujin_Gisela_Diego.pdf" type="application/pdf">
    <div class="pdf-fallback">
      Tu navegador no permite visualizar el PDF directamente.<br>
      👉 <a href="Algoritmos_de_Brujin_Gisela_Diego.pdf" target="_blank">Haz clic aquí para descargarlo</a>.
    </div>
  </object>
</div>