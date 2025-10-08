# 🧬 Práctica de Aula 3 - Avances y Aplicaciones del PGH

## 📘 Artículo seleccionado

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

### 1. Contexto e impacto
- ¿Por qué la caída del precio de la secuenciación genómica transformó el panorama de la bioinformática en 2015?  
- ¿Cómo influyó este avance en la investigación médica y en la medicina personalizada?

### 2. Aspectos técnicos
- ¿Qué características hacen que **GDC 2** sea más eficiente que otros compresores como FRESCO o GDC-ultra?  
- ¿Qué papel juega la similitud genética entre individuos en la mejora de la compresión?  
- ¿Cómo afecta el número de referencias o el uso de varios hilos de ejecución a la velocidad y al rendimiento?

### 3. Dimensión ética y social
- ¿Qué desafíos éticos surgen al almacenar y compartir miles de genomas humanos?  
- ¿Qué riesgos existen para la privacidad de los individuos?  
- ¿Cómo podrían estos avances aumentar la desigualdad entre países o instituciones con distinto acceso a tecnología?

### 4. Reflexión final
- ¿De qué manera este artículo refleja los retos y oportunidades de la bioinformática en la década de 2010?  
- ¿Qué avances tecnológicos posteriores (por ejemplo, inteligencia artificial o cloud computing) podrían potenciar aún más el enfoque de GDC 2?

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