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

Esta visualización muestra el número de artículos por periódico incluidos en la colección. Permite identificar qué medios tuvieron una participación más activa en la cobertura del rock colombiano durante el periodo 1985–1995 y sirve como punto de partida para entender qué voces institucionales participaron en la construcción de la cobertura periodística sobre el rock colombiano en la prensa escrita.

<div style="width: 100%; text-align: center; margin: 2rem 0;">
  <iframe 
    src="{{ site.baseurl }}/assets/html/distribucion_publicaciones_donut.html"
    style="width: 100%; max-width: 1100px; height: 650px; border: none; margin: 0 auto; display: block;">
  </iframe>
</div>

##### b. Cantidad de publicaciones por género periodístico

La siguiente gráfica cruza los géneros periodísticos con los periódicos representados en los documentos de esta colección. Este cruce permite reconocer variaciones en la forma en que cada medio abordó el rock, así como posibles diferencias en el peso relativo de cada género, lo que aporta indicios sobre la diversidad de la cobertura mediática.

<div style="width: 100%; text-align: center; margin: 2rem 0;">
  <iframe 
    src="{{ site.baseurl }}/assets/html/heatmap_generos_periodicos.html"
    style="width: 100%; max-width: 1100px; height: 650px; border: none; margin: 0 auto; display: block;">
  </iframe>
</div>

##### c. Distribución de géneros por década

La siguiente gráfica cruza los géneros periodísticos con las décadas representadas en los documentos de esta colección. La categorización de géneros fue establecida específicamente para este proyecto con el fin de organizar los tipos de textos presentes y facilitar su comparación temporal. Esta clasificación permite identificar variaciones en la manera en que se abordó el rock a lo largo del tiempo y observar cambios en el peso relativo de cada género dentro de la cobertura mediática.

<div style="width: 100%; text-align: center; margin: 2rem 0;">
  <iframe 
    src="{{ site.baseurl }}/assets/html/barras_apiladas_decadas.html"
    style="width: 100%; max-width: 1100px; height: 650px; border: none; margin: 0 auto; display: block;">
  </iframe>
</div>


## Voyant Tools

#### Resumen del Corpus

En primer lugar, se muestra el resumen general del corpus de 210 artículos los cuales sumaron 133.075 palabras distribuidas en 15.694 formas léxicas únicas. Así mismo, se pueden observar las medidas textuales relevantes, como la longitud relativa de los documentos, la densidad de vocabulario, el promedio de palabras por oración y el índice de legibilidad de los textos. Se puede identificar las palabras más frecuentes del corpus entre las cuales destacan *rock, grupo, música, concierto* y *grupos*.
##### Nube de palabras 
La siguiente nube de palabras fue generada a partir del corpus completo de prensa, eliminado las palabras vacías o *stopwords" de los documentos. En esta se observa un panórama general de las palabras más frecuentes de los artículos que componen está colección.

<div style="display: flex; justify-content: center; margin: 2rem 0;">
  <iframe 
    style="width: 80%; height: 400px; border: none;" 
    src="https://voyant-tools.org/tool/Cirrus/?stopList=keywords-59c6c1c26b811ae678f38ca30ffb4c69&whiteList=&visible=200&corpus=f99f79bd376cc31cd7a87bb6281a3c1a">
  </iframe>
</div>

##### Términos frecuentes 



<iframe style='width: 1422px; height: 556px;' src='https://voyant-tools.org/tool/CorpusTerms/?view=CorpusTerms&stopList=keywords-1a9921d84b8a086821313840dacd1f86&comparisonCorpus=&corpus=5ea6f2777dc0845027a440049ea659d6'></iframe>
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