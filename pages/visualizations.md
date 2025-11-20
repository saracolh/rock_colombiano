---
title: Visualizaciones
layout: visualizations
permalink: /visualizations.html

---
{% include feature/nav-menu.html sections="Visualizaciones Generales;Voyant Tools;Orange Data Mining; AntConc" %}

## ¿Qué visualizaciones contiene esta colección? 

Esta sección reúne las visualizaciones generadas a partir del corpus de prensa sobre el rock en Colombia entre 1985 y 1995.

En primer lugar, se presentan las visualizaciones generales elaboradas en Google Colab con Python, basadas en el archivo *CSV* que integra los 229 artículos de la colección. Estas gráficas ofrecen una lectura inicial sobre la distribución del corpus por periódico, género periodístico y año de publicación.

Posteriormente, se presentan los resultados obtenidos con herramientas como *Voyant Tools, Orange Data Mining* y *AntConc*, organizados por herramienta para facilitar la consulta. Para esta etapa se trabajó con 210 artículos en formato .txt, generados mediante OCR, ya que algunos documentos fueron excluidos debido a errores en el reconocimiento óptico de caracteres que impidieron su procesamiento completo.

## Visualizaciones generales

##### a. Cantidad de publicaciones por periódico

Esta visualización muestra el número de artículos por periódico incluidos en la colección. Permite identificar qué medios tuvieron una participación más activa en la cobertura del rock colombiano durante el periodo 1985–1995 y sirve como punto de partida para comprender qué voces institucionales intervinieron en la construcción del discurso periodístico de la época.

<div style="width: 100%; text-align: center; margin: 2rem 0;">
  <iframe 
    src="{{ site.baseurl }}/assets/html/distribucion_publicaciones_donut.html"
    style="width: 100%; max-width: 1100px; height: 650px; border: none; margin: 0 auto; display: block;">
  </iframe>
</div>

##### b. Cantidad de publicaciones por género periodístico

La siguiente gráfica presenta la distribución de los géneros periodísticos en los documentos de esta colección. Este cruce permite reconocer variaciones en la forma en que cada medio abordó el rock, así como diferencias en el peso relativo de cada género, lo que ofrece indicios sobre la diversidad de la cobertura mediática.

La categorización de géneros fue definida específicamente para este proyecto como una forma de organizar el corpus durante el análisis exploratorio. Aunque es una propuesta propia, ofrece un marco de referencia que permite identificar posibles variaciones en las estrategias de representación a lo largo de la década y aproximarse al papel que cada género pudo ocupar dentro del discurso periodístico.

<div style="width: 100%; text-align: center; margin: 2rem 0;">
  <iframe 
    src="{{ site.baseurl }}/assets/html/heatmap_generos_periodicos.html"
    style="width: 100%; max-width: 1100px; height: 650px; border: none; margin: 0 auto; display: block;">
  </iframe>
</div>

##### c. Distribución de géneros por década

Esta gráfica muestra cómo se distribuyen los géneros periodísticos por década y permite identificar cambios en el tipo de textos publicados sobre el rock colombiano en cada periodo.

<div style="width: 100%; text-align: center; margin: 2rem 0;">
  <iframe 
    src="{{ site.baseurl }}/assets/html/barras_apiladas_decadas.html"
    style="width: 100%; max-width: 1100px; height: 650px; border: none; margin: 0 auto; display: block;">
  </iframe>
</div>


## Voyant Tools
La primera aproximación al análisis textual se realizó con Voyant Tools, que permite examinar el vocabulario dominante, las tendencias y la estructura general del corpus. Esta herramienta facilita una lectura global del conjunto de textos y ofrece una visión inicial sobre los temas, términos recurrentes y variaciones léxicas presentes en los artículos.
#### Resumen del Corpus
El corpus analizado está compuesto por 210 artículos que suman 133.075 palabras y 15.694 formas léxicas únicas. Este resumen incluye medidas textuales como la longitud de los documentos, la densidad de vocabulario, el promedio de palabras por oración y el índice de legibilidad. También ofrece un primer vistazo a las palabras con mayor frecuencia, entre las que destacan *rock, grupo, música, concierto* y *grupos*.

<div style="display: flex; justify-content: center; margin: 2rem 0;">
  <iframe 
    style="width: 1422px; height: 556px;" 
    src="https://voyant-tools.org/tool/Summary/?view=Summary&stopList=keywords-59c6c1c26b811ae678f38ca30ffb4c69&limit=20&corpus=5ea6f2777dc0845027a440049ea659d6">
  </iframe>
</div>

#### Nube de palabras 
La siguiente nube de palabras fue generada a partir del corpus completo de prensa, eliminado las palabras vacías o *stopwords" de los documentos. En esta se observa un panórama general de las palabras más frecuentes de los artículos que componen está colección.

<div style="display: flex; justify-content: center; margin: 2rem 0;">
  <iframe 
    style="width: 80%; height: 400px; border: none;" 
    src="https://voyant-tools.org/tool/Cirrus/?stopList=keywords-59c6c1c26b811ae678f38ca30ffb4c69&whiteList=&visible=200&corpus=f99f79bd376cc31cd7a87bb6281a3c1a">
  </iframe>
</div>

#### Racimo de términos 

Esta visualización complementa la nube de palabras, ya que, aunque ambas muestran la frecuencia total de los términos, TermsBerry añade información sobre la cantidad de documentos en los que aparece cada palabra. Esto permite entender no solo qué términos son más frecuentes, sino también cuán extendidos están a lo largo del corpus.

<div class="d-flex justify-content-center my-4">
  <iframe
    style="width: 1422px; height: 556px;"
    src="https://voyant-tools.org/tool/TermsBerry/?view=TermsBerry&stopList=keywords-30dd93a07c481aa6a70826f6d5cd4c78&corpus=5ea6f2777dc0845027a440049ea659d6"
    loading="lazy">
  </iframe>
</div>

##### Términos frecuentes 

La visualización Terms presenta un listado ordenado por frecuencia de los términos del corpus e incorpora la gráfica Trend, que muestra la variación de cada palabra a lo largo del conjunto de documentos. Esto permite identificar momentos de mayor o menor presencia de términos como rock, grupo o música, ofreciendo una lectura temporal que complementa tanto la nube de palabras como TermsBerry. 

<div class="d-flex justify-content-center my-4">
  <iframe
    style="width: 1422px; height: 556px;"
    src="https://voyant-tools.org/tool/CorpusTerms/?view=CorpusTerms&stopList=keywords-1a9921d84b8a086821313840dacd1f86&comparisonCorpus=&corpus=5ea6f2777dc0845027a440049ea659d6"
    loading="lazy">
  </iframe>
</div>

##### Relación entidades detectadas por Voyant Tools

<div class="d-flex justify-content-center my-4">
  <iframe
    style="width: 80%; height: 800px; border: none;"
    src="https://voyant-tools.org/?view=RezoViz&corpus=f73299667c2b5f97a41c069787e019f2"
    loading="lazy">
  </iframe>
</div>




---
## Orange Data Mining



---
## AntConc

---