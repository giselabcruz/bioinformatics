# 🧬 Práctica de Aula 3 - Avances y Aplicaciones del PGH

### - Artículo seleccionado -

**Referencia:**  
Deorowicz, S., Danek, A. & Niemiec, M. (2015). *GDC 2: Compression of large collections of genomes.*  
**Scientific Reports**, 5:11565.  
DOI: [10.1038/srep11565](https://doi.org/10.1038/srep11565)  
Disponible en: [https://www.nature.com/articles/srep11565](https://www.nature.com/articles/srep11565)

**Resumen breve:**  
El artículo presenta un algoritmo llamado **GDC 2 (Genome Differential Compressor 2)**, diseñado para comprimir colecciones completas de genomas humanos. Su método logra reducir hasta **9.500 veces** el tamaño original de los datos (por ejemplo, 6.7 TB de genomas comprimidos a 700 MB), siendo además **cuatro veces más eficiente** que los compresores existentes en ese momento.  
El algoritmo se basa en una doble factorización de Ziv–Lempel y aprovecha la similitud entre los genomas humanos. Fue desarrollado en C++ con soporte multihilo, alcanzando velocidades de compresión de **200 MB/s** y descompresión de **1 GB/s**, lo que representó un avance significativo para la bioinformática de 2015.

---

## Preguntas que se responden en el informe realizado

### Cuestión 1
¿Qué impacto crees que ha tenido el avance descrito en el artículo en el desarrollo actual de la
bioinformática y la medicina genómica? Reflexiona sobre cómo ese estudio ha contribuido al análisis
de datos, a la interpretación del genoma o al progreso tecnológico.

### Cuestión 2
¿Qué desafíos éticos, técnicos o sociales identificas a partir del estudio analizado y cómo podrían
abordarse en el futuro? Piensa en temas como la privacidad de los datos, el uso responsable de la
información genética, el sesgo en los datos o la equidad científica.
---

## 📄 Visualización del informe

[Abrir informe en PDF](Avances_y_aplicaciones_del_PGH_Gisela.pdf)

<style>
.pdf-embed { 
  position: relative; 
  width: 100%; 
  padding-top: 75%; 
}
.pdf-embed iframe, 
.pdf-embed object {
  position: absolute; 
  top: 0; 
  left: 0; 
  width: 100%; 
  height: 100%; 
  border: 0; 
}
</style>

<div class="pdf-embed">
  <object data="Avances_y_aplicaciones_del_PGH_Gisela.pdf" type="application/pdf"></object>
</div>