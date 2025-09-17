<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Semana 1 - Jueves Ago 14</title>
  <style>
    .subtitulo, .subtitulo2 {
      font-size: 1.5em;
      color: #2563eb;
      margin-top: 2em;
      margin-bottom: 1em;
      text-align: left;
    }
    .subtitulo2 {
      color: #1a365d;
      font-size: 1.3em;
      margin-top: 2em;
      margin-bottom: 1em;
    }
    body {
      font-family: 'Segoe UI', Arial, sans-serif;
      background: #f8fafc;
      margin: 0;
      padding: 0;
    }
    nav {
      width: 240px;
      background: #f4f4f4;
      padding: 2em 1.2em 2em 1.2em;
      min-height: 100vh;
      box-shadow: 2px 0 8px #e0e7ef;
      border-right: 1px solid #e0e7ef;
      position: fixed;
      top: 0;
      left: 0;
      height: 100vh;
      overflow-y: auto;
      z-index: 1000;
    }
    nav h2 {
      font-size: 1.2em;
      color: #1a365d;
      margin-top: 0;
      margin-bottom: 1.2em;
      letter-spacing: 0.5px;
    }
    nav ul {
      list-style: none;
      padding: 0;
      margin-bottom: 1.5em;
    }
    nav a {
      font-size: 1em;
      color: #2563eb;
      text-decoration: none;
      padding: 0.3em 0.8em;
      border-radius: 6px;
      background: #e0e7ef;
      transition: background 0.2s, color 0.2s;
      display: inline-block;
    }
    nav a:hover {
      background: #2563eb;
      color: #fff;
    }
    .titulo-principal {
      font-size: 2.2em;
      color: #1a365d;
      margin-bottom: 0.5em;
      text-align: center;
    }
    .subtitulo, .subtitulo2 {
      font-size: 1.5em;
      color: #2563eb;
      margin-top: 2em;
      margin-bottom: 1em;
      text-align: left;
    }
    .subtitulo2 {
      color: #1a365d;
      font-size: 1.3em;
      margin-top: 2em;
      margin-bottom: 1em;
    }
    .parrafo {
      font-size: 1em;
      color: #222;
      margin-bottom: 1.2em;
      line-height: 1.7;
    }
    .texto {
      margin-bottom: 2em;
    }
    table {
      width: 100%;
      border-collapse: collapse;
      margin: 2em 0;
      background: #fff;
      box-shadow: 0 2px 8px #e0e7ef;
      border-radius: 10px;
      padding: 12px;
    }
    th, td {
      padding: 8px;
      border: 1px solid #bfc9d9;
    }
    thead tr {
      background: #e0e7ef;
      color: #1a365d;
    }
    .videos-dos {
      display: flex;
      gap: 2em;
      justify-content: center;
      margin-bottom: 2em;
      flex-wrap: wrap;
    }
    .video-frame {
      background: #f1f5fa;
      border-radius: 10px;
      box-shadow: 0 2px 8px #e0e7ef;
      padding: 1em;
      width: 350px;
      text-align: center;
    }
    .video-frame iframe {
      width: 100%;
      height: 200px;
      border: none;
      border-radius: 8px;
      margin-bottom: 0.5em;
    }
    .img-contenido {
      max-width: 900px;
      width: 100%;
      height: auto;
      border-radius: 10px;
      box-shadow: 0 2px 8px #e0e7ef;
      margin: 0 0 1.5em 0;
      display: block;
    }
    a {
      font-size: 1em;
      color: #1a365d;
      background: none;
      border: none;
      text-decoration: underline;
    }
  </style>
</head>
<body style="display: flex; margin: 0; min-height: 100vh;">
  <nav style="width: 240px; background: #f4f4f4; padding: 2em 1.2em 2em 1.2em; min-height: 100vh; box-shadow: 2px 0 8px #e0e7ef; border-right: 1px solid #e0e7ef; position: fixed; top: 0; left: 0; height: 100vh; overflow-y: auto; z-index: 1000;">
    <h2 style="font-size: 1.2em; color: #1a365d; margin-top: 0; margin-bottom: 1.2em; letter-spacing: 0.5px;">Temario</h2>
    <ul style="list-style: none; padding: 0; margin-bottom: 1.5em;">
      <li><a href="#magnitudes">Magnitudes físicas, análisis dimensional y sistemas de unidades</a></li>
      <li><a href="#vectores">Vectores</a></li>
      <li><a href="#conversion">Conversión de unidades y análisis dimensional</a></li>
      <li><a href="#grafico">Elaboración de gráficos y vectores</a></li>
      <li><a href="#alometria">Alometría y ley de Kleiber</a></li>
      <li><a href="#escala">Factores de escala</a></li>
    </ul>
    <hr>
    <a href="../" style="font-size:1em; color:#1a365d; background:none; border:none; text-decoration:underline;">&#8592; Volver al cronograma</a>
  </nav>
  <main style="flex: 1; padding: 2.5em 3em; background: #fff; min-height: 100vh; margin-left: 240px;">
    <h1 class="titulo-principal">Semana 2 (Jueves Ago 14)</h1>
    <section id="generalidades">
      <h1 class="titulo-principal">Generalidades de la biofísica</h1>
      <div class="texto">
        <p class="parrafo">Aunque los procesos biológicos son bastante complejos, al final, se encuentran gobernados por las mismas leyes físicas que gobiernan sistemas más simples. En otras palabras los fenómenos físicos se convierten en la base sobre la cual se estructura la realidad en la que habitan los organismos biológicos. Por lo tanto, entender la relación entre los procesos biológicos y los fenómenos físicos subyacentes, es un paso crucial para aproximarse a la ecología. Para comprender esta relación, se requiere interiorizar conceptos que permitan a la física y la biología "hablar un mismo lenguaje". Al final, este rol lo cumple el lenguaje matemático.<strong>En esta sesión discutiremos conceptos básicos o fundamentales que permitirán adentrarse en temas físicos dentro de un contexto ecológico.</strong></p>
        <a href="https://drive.google.com/file/d/1LXqpWhVRihNQVxRNapYJI4FAxwwwvBCk/view?usp=sharing" target="_blank" style="display:block;margin:1em 0;font-weight:bold;color:#2563eb;">🎧 Escucha el podcast: Física y vida: conceptos básicos y la ley de escala</a>
      </div>
    </section>
    <section id="magnitudes">
      <h2 class="subtitulo" id="magnitudes">Magnitudes físicas, análisis dimensional y sistemas de unidades</h2>
      <p class="parrafo">Una <strong>magnitud física</strong> se refiere a cualquier propiedad de un objeto o fenómeno que puede ser expresada numéricamente, como: la distancia, el tiempo, la masa o la temperatura. La <strong>cantidad</strong>, por su parte, se refiere a la medida de una magnitud física, expresada en un sistema de unidades específico como: metros, segundos, gramos y °C.</p>
      <p class="parrafo">Se reconocen <strong>cuatro cantidades fundamentales</strong> la longitud con dimensión L, la masa cuya dimensión es M, el tiempo cuya dimensión es T y la carga eléctrica cuya dimensión es C. Desde aquí expresaremos la dimensión de una cantidad física encerrandola entre corchetes. Por ejemplo, si T es una temperatura, su dimensión se expresaría [T].</p>
      <p class="parrafo">Cualquier otra cantidad física se expresa a partir de las cantidades fundamentales. Por ejemplo el área (A) con dimensión [A]=L<sup>2</sup>, o la densidad (&rho;) con dimensión [&rho;]=ML<sup>-3</sup>.</p>
      <p class="parrafo">Existen 3 sistemas de unidades para expresar las cantidades físicas de manera coherente: El <strong>Sistema Internacional (SI)</strong>, el <strong>Sistema Gaussiano</strong> y el <strong>Sistema Ingles (SU)</strong>. Los factores de conversión, entre los sistemas
      de unidades SI y gaussiano, están dados por  1m=10<sup>2</sup>cm y 1kg=10<sup>3</sup>g.  El sistema de unidades SU no es común en contextos científicos. En este sistema las cantidades fun damentales son la fuerza con dimensión F, la longitud con dimensión L y el tiempo con dimensión T y sus unidades patrón son, respectivamente, la libra (lb), el pié (p) y el segundo (s).</p>
      <figure style="text-align:center; margin:2em 0;">
        <a href="res/unidades.png" target="_blank">
          <img src="res/unidades.png" alt="Unidades físicas" style="max-width:300px; width:100%; border-radius:10px; box-shadow:0 2px 8px #e0e7ef;">
        </a>
        <figcaption style="color:#2563eb; font-size:1em; margin-top:0.5em;">Figura: Ejemplo de unidades físicas. Las unidades de fuerza que se llaman Newton (N), a las de trabajo y energía Julio (J), potencia Vatio (W) y presión Pascal (Pa)</figcaption>
      </figure>
          <div style="display: flex; justify-content: center; align-items: center; gap: 2em; margin: 2em 0;">
            <div class="video-frame">
              <iframe src="https://www.youtube.com/embed/eBML4oHcUXQ?si=TByBOrhgT31Rt7YL" title="Importancia del análisis dimensional" allowfullscreen></iframe>
              <figcaption style="color:#2563eb; font-size:1em; margin-top:0.5em;">Video: No seas un pend#$%#$%: la importancia del análisis dimensional para hablar de física</figcaption>
            </div>
            <div class="video-frame">
              <iframe src="https://www.youtube.com/embed/87pGTT68izY?si=R4-DMAYCatFUFrnG" title="Video adicional" allowfullscreen></iframe>
              <figcaption style="color:#2563eb; font-size:1em; margin-top:0.5em;">Por qué es tan peligroso ver estas pendej"#$$"#$</figcaption>
            </div>
          </div>
    </section>
    <section id="vectores">
        <h2 class="subtitulo" id="vectores">Representación espacial y vectores</h2>
        <p class="parrafo">Para poder representar los fenómenos físicos reales, las cantidades físicas pueden ser escalares o vectoriales. Una <strong>cantidad escalar</strong> se refiere a cualquier propiedad de un objeto o fenómeno que puede ser expresada numéricamente, como: la distancia, el tiempo, la masa o la temperatura. La <strong>cantidad</strong>, por su parte, se refiere a la medida de una magnitud física, expresada en un sistema de unidades específico como: metros, segundos, gramos y °C.</p>
    </section>
    <!-- Puedes agregar más secciones, tablas, videos o imágenes aquí -->
  </main>
</body>
</html>
