---
title: Visualizaciones
layout: visualizations
permalink: /visualizations.html

---
{% include feature/nav-menu.html sections="Visualizaciones Generales;Voyant Tools;Orange Data Mining; AntConc" %}

## ¿Qué visualizaciones contiene esta colección? 

Este espacio reúne las principales visualizaciones realizadas a partir del corpus de prensa sobre el rock en Colombia (1985–1995). Las gráficas permiten observar, desde diferentes niveles de detalle, cómo se organiza el conjunto documental y cuáles son algunos de los patrones discursivos identificados durante el análisis.

En primer lugar, se presentan las visualizaciones generales —elaboradas en Google Colab con Python— a partir del archivo CSV final que reúne todos los documentos de esta colección; es decir, 229 artículos de prensa de los periódicos *El Tiempo, La Prensa, El Espectador, El Mundo, El Nuevo Siglo* y *Revista Semana*. Su objetivo es ofrecer una panorámica de la distribución de las publicaciones por periódico, género periodístico y década, antes de profundizar en el análisis textual con las demás herramientas. 

Luego, se incluyen los resultados obtenidos con *Voyant Tools*, *Orange Data Mining* y *AnTConC*, organizados por herramienta para facilitar la lectura del proceso metodológico. Cabe precisar que, para el análisis exploratorio de datos, se usaron 210 artículos de la presente colección a expeción... Estos artículos no se tuvieron en cuenta en el análisis porque no fue posible extraer completamente el texto por medio del reconocimiento óptico de carácteres (OCR)

## Visualizaciones generales



##### a. Cantidad de publicaciones por periódico

Esta gráfica muestra el número de artículos por periódico incluidos en el corpus. Permite identificar qué medios tuvieron una participación más activa en la cobertura del rock colombiano durante el periodo 1985–1995 y sirve como punto de partida para entender desde qué voces institucionales se construyó el relato mediático.

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
##### Nube de palabras 
La siguiente nube de palabras fue generada a partir del corpus completo de prensa, eliminado las palabras vacías o *stopwords" de los documentos. En esta se observa un panórama general de las palabras más frecuentes de los artículos que componen está colección.

<div style="display: flex; justify-content: center; margin: 2rem 0;">
  <iframe 
    style="width: 80%; height: 400px; border: none;" 
    src="https://voyant-tools.org/tool/Cirrus/?stopList=keywords-59c6c1c26b811ae678f38ca30ffb4c69&whiteList=&visible=200&corpus=f99f79bd376cc31cd7a87bb6281a3c1a">
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

<div class="d-flex justify-content-center my-4">
  <iframe
    style="width: 80%; height: 800px; border: none;"
    src="https://voyant-tools.org/tool/Documents/?stopList=keywords-59c6c1c26b811ae678f38ca30ffb4c69&corpus=f99f79bd376cc31cd7a87bb6281a3c1a"
    loading="lazy">
  </iframe>
</div>



---
## Orange Data Mining

---
## AntConc

---