---
title: Visualizaciones
layout: visualization
permalink: /visualizations.html

---
{% include feature/image.html objectid="1993-08-06_seguridadsocial" %}

Este espacio reúne visualizaciones del análisis del corpus de prensa sobre el rock en Colombia (1985–1995).
Despliega cada bloque para ver los resultados por herramienta.

<div class="accordion my-4" id="accordionHerramientas">

  <!-- Voyant Tools (interactivo) -->
  <div class="accordion-item">
    <h2 class="accordion-header" id="headVoyant">
      <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#colVoyant" aria-expanded="true" aria-controls="colVoyant">
        Voyant Tools (interactivo)
      </button>
    </h2>
    <div id="colVoyant" class="accordion-collapse collapse show" aria-labelledby="headVoyant" data-bs-parent="#accordionHerramientas">
      <div class="accordion-body">
        <p>Exploración con Voyant (nubes, frecuencias, tendencias).</p>

        <!-- Pega aquí el iframe que te da Voyant (sin comentar) -->
        <iframe
          src="https://voyant-tools.org/?corpus=demo" 
          width="100%" height="600" frameborder="0" loading="lazy"></iframe>
      </div>
    </div>
  </div>

  <!-- Orange Data Mining -->
  <div class="accordion-item">
    <h2 class="accordion-header" id="headOrange">
      <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#colOrange" aria-expanded="false" aria-controls="colOrange">
        Orange Data Mining
      </button>
    </h2>
    <div id="colOrange" class="accordion-collapse collapse" aria-labelledby="headOrange" data-bs-parent="#accordionHerramientas">
      <div class="accordion-body">
        <p>Heatmaps, clustering y redes de términos.</p>

        <!-- Imagen de prueba (cámbiala por la tuya) -->
        <figure class="mb-3">
          <img src="{{ '/assets/img/visualizaciones/ejemplo_orange.png' | relative_url }}" 
               alt="Ejemplo Orange" class="img-fluid rounded shadow-sm" loading="lazy">
          <figcaption class="small text-muted mt-1">Ejemplo Orange (sustituir por tu gráfico).</figcaption>
        </figure>

        <!-- Cuando tengas una versión interactiva (Flourish/Observable), sustituye por su iframe -->
        <!--
        <iframe src="https://public.flourish.studio/visualisation/XXXXX/embed"
                width="100%" height="600" frameborder="0" loading="lazy"></iframe>
        -->
      </div>
    </div>
  </div>

  <!-- AntConc -->
  <div class="accordion-item">
    <h2 class="accordion-header" id="headAntconc">
      <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#colAntconc" aria-expanded="false" aria-controls="colAntconc">
        AntConc
      </button>
    </h2>
    <div id="colAntconc" class="accordion-collapse collapse" aria-labelledby="headAntconc" data-bs-parent="#accordionHerramientas">
      <div class="accordion-body">
        <p>Concordancias (KWIC), n-gramas y listas de frecuencia.</p>

        <!-- Imagen de prueba (cámbiala por la tuya) -->
        <figure class="mb-3">
          <img src="{{ '/assets/img/visualizaciones/ejemplo_antconc.png' | relative_url }}" 
               alt="Ejemplo AntConc" class="img-fluid rounded shadow-sm" loading="lazy">
          <figcaption class="small text-muted mt-1">Ejemplo AntConc (sustituir por tu gráfico).</figcaption>
        </figure>
      </div>
    </div>
  </div>

</div>