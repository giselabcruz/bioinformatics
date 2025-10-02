# 🧬 Práctica 2 – Del ADN a la Proteína  

## Ejercicio 1. Replicación del ADN  
**Objetivo:** comprender el mecanismo semiconservativo y las enzimas implicadas.  

1. Considera la siguiente secuencia de ADN:  
   `5’ – ATG CCG TTA GCT – 3’`  
   `3’ – TAC GGC AAT CGA – 5’`  

2. **Realiza una ronda de replicación:**

- **Identifica las nuevas hebras que se formarán:**  

  ```
  TAC GGC AAT CGA
  ATG CCG TTA GCT
  ```

- **Indica la función de helicasa, primasa, ADN polimerasa y ligasa.**  

  - **Helicasa:** desenrolla la doble hélice y rompe los puentes de hidrógeno entre las bases.  
  - **Primasa:** sintetiza pequeños fragmentos de ARN (cebadores) para iniciar la síntesis.  
  - **ADN polimerasa:** incorpora nucleótidos complementarios en dirección 5’→3’.  
  - **Ligasa:** sella los fragmentos de Okazaki en la hebra retardada.  

3. **Reflexiona: ¿qué ocurriría si la ADN polimerasa cometiera un error en una base y no se corrigiera?**  

   Si la ADN polimerasa comete un error y no lo corrige, se produce una **mutación**.  

   Esta puede ser:  
   - **Silenciosa:** sin efecto en la proteína.  
   - **De cambio de sentido:** altera un aminoácido.  
   - **Sin sentido:** introduce un codón de paro prematuro.
   Si ocurre en una región no codificante, el error puede no tener consecuencias.


**Extensión con Biopython:**  
Escribe un script que, dada una cadena de ADN, genere automáticamente su hebra complementaria y compara con tu resultado manual.  

---

## Ejercicio 2. Transcripción del ADN a ARN  
**Objetivo:** traducir correctamente la información de la cadena molde.  

**Instrucciones:**  
1. Usa la siguiente secuencia de ADN:  
   `5’ – ATG CCT GAA TGC – 3’`  
   `3’ – TAC GGA CTT ACG – 5’`  

2. Identifica cuál es la cadena molde.  
3. Obtén el transcrito de ARN correspondiente (recuerda usar uracilo en lugar de timina).  
4. Explica cuál sería la región promotora y cuál la codificante.  

**Extensión con Biopython:**  
Crea un script que lea un archivo FASTA con ADN y produzca la secuencia de ARNm. Experimenta cambiando la orientación de la hebra.  

---

## Ejercicio 3. Traducción del ARNm a proteína  
**Objetivo:** aplicar el código genético y reflexionar sobre mutaciones.  

**Instrucciones:**  
1. Usa el siguiente transcrito de ARN:  
   `5’ – AUG UAU GCU UAA – 3’`  

2. Identifica el codón de inicio y el codón de paro.  
3. Traduce la secuencia en aminoácidos.  
4. Reflexiona:  
   - ¿Qué pasaría si AUG mutara a GUG?  
   - ¿Y si el codón de paro desapareciera?  

**Extensión con Biopython:**  
Usa `Bio.Seq` para traducir automáticamente el ARNm y compara con tu traducción manual.  

---

## Ejercicio 4. Splicing alternativo  
**Objetivo:** comprender cómo un mismo gen puede generar varias proteínas.  

**Instrucciones:**  
1. Considera un gen con 5 exones: `1–2–3–4–5`.  
2. Diseña al menos dos combinaciones de splicing (ej. `1–2–4–5` o `1–3–5`).  
3. Explica qué diferencias esperarías en las proteínas resultantes.  
4. Reflexiona: ¿por qué este mecanismo aumenta la diversidad proteica sin necesidad de más genes?  

**Extensión con Biopython / bases de datos:**  
Busca en Ensembl un gen humano con isoformas (ej. **FGFR2**) y compara transcritos.  

---

## Ejercicio 5. Introducción a las proteínas  
**Objetivo:** relacionar secuencia, estructura y función.  

**Instrucciones:**  
1. Considera la secuencia:  
   `Met – Ile – Ser – Gly – Val – Lys – His`  

2. Identifica el extremo N y el extremo C.  
3. Reflexiona:  
   - ¿Cómo influye el orden de los aminoácidos en la estructura final?  
   - ¿Qué ocurriría si un aminoácido hidrofóbico se sustituyera por uno hidrofílico en una región interna?  

**Extensión con bioinformática:**  
Busca en el **PDB** la estructura de una proteína y analiza el efecto de una mutación puntual en el plegamiento.  

---

## Ejercicio 6. Actividad integradora: del ADN a la proteína  
**Objetivo:** recorrer el dogma central completo.  

**Instrucciones:**  
1. Escoge una secuencia de ADN de un banco de datos.  
2. Paso 1: replica la secuencia indicando las dos nuevas hebras.  
3. Paso 2: transcribe la cadena molde en ARNm.  
4. Paso 3: traduce el ARNm en aminoácidos.  
5. Reflexiona: ¿qué punto del proceso es más vulnerable a errores?  
6. Programa un pipeline que realice los tres procesos (replicación, transcripción y traducción).  

**Extensión con Biopython:**  
El pipeline debe informar de cada paso y producir las tres salidas: hebra complementaria, ARNm y proteína.  

---

## 📊 Informe
- Informe en PDF con formato académico:


## 📌 Código  

- 💻 Enlace al repositorio 👉 [Practica 2 - ejercicios](https://github.com/giselabcruz/pa_2_bio)  
- 📦 Código en formato `.zip`: 

## 📌 Presentación
- Apoyo visual en PDF: 

