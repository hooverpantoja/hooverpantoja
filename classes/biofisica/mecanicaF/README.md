<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Semana 9 - Jueves Noviembre 20</title>
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

    /* Responsividad básica */
    @media (max-width: 900px) {
      nav {
        position: static !important;
        width: 100% !important;
        height: auto !important;
        min-height: auto !important;
      }
      main {
        margin-left: 0 !important;
        padding: 1.5em !important;
      }
      .videos-dos {
        flex-wrap: wrap !important;
      }
      .video-frame {
        width: 100% !important;
        max-width: 520px;
      }
    }
  </style>
</head>
<body style="display: flex; margin: 0; min-height: 100vh;">
  <nav aria-label="Navegación lateral" style="width: 240px; background: #f4f4f4; padding: 2em 1.2em 2em 1.2em; min-height: 100vh; box-shadow: 2px 0 8px #e0e7ef; border-right: 1px solid #e0e7ef; position: fixed; top: 0; left: 0; height: 100vh; overflow-y: auto; z-index: 1000;">
    <h2 style="font-size: 1.2em; color: #1a365d; margin-top: 0; margin-bottom: 1.2em; letter-spacing: 0.5px;">Temario</h2>
    <ul style="list-style: none; padding: 0; margin-bottom: 1.5em;">
      <li><a href="#hidrostatica">Hidrostática</a></li>
  <li><a href="#hidrodinamica">Hidrodinámica</a></li>
      <li><a href="#tension">Tensión superficial y capilaridad</a></li>
      <li><a href="#osmosis">Osmosis</a></li>
    </ul>
    <hr>
    <h2 style="font-size: 1.2em; color: #1a365d; margin-top: 0; margin-bottom: 1.2em; letter-spacing: 0.5px;">Recursos</h2>
    <ul style="list-style: none; padding: 0; margin-bottom: 1.5em;">
      <li><a href="../res/Microcurrículo.pdf"> Microcurrículo</a></li>
      <li><a href="https://drive.google.com/drive/folders/1-8WeZK28iaaEToQVGgGCnHxfx8AhXX3f?usp=sharing"> Fundamentos físicos de los fenómenos biológicos</a></li>
    </ul>
    <h2 style="font-size: 1.2em; color: #1a365d; margin-top: 0; margin-bottom: 1.2em; letter-spacing: 0.5px;">Autores</h2>
    <ul style="list-style: none; padding: 0; margin-bottom: 1.5em;">
      <li><a href="https://www.researchgate.net/profile/Hoover-Pantoja-Sanchez">Hoover Pantoja-Sánchez</a></li>
      <li><a href="https://www.researchgate.net/profile/Marco-Giraldo">Marco A.Giraldo</a></li>
    </ul>
    <hr>
    <a href="../" style="font-size:1em; color:#1a365d; background:none; border:none; text-decoration:underline;">&#8592; Volver al cronograma</a>
  </nav>
  <main style="flex: 1; padding: 2.5em 3em; background: #fff; min-height: 100vh; margin-left: 240px;">
    <h1 class="titulo-principal">Semana 9 (Jueves Nov 20)</h1>
    <section id="generalidades">
      <h1 class="titulo-principal">Mecánica de fluidos</h1>
      <a href="https://drive.google.com/file/d/1H8DW8wL6wqH5nj7whNVQydUS1J91BVtO/view?usp=drive_link" target="_blank" style="display:block;margin:1em 0;font-weight:bold;color:#2563eb;">🎧 Escucha el podcast - Introducción a la Mecánica de fluidos </a>
      <div class="videos-dos" style="display: flex; gap:2em; justify-content:center; margin:2em 0; flex-wrap:wrap;">
        <div class="video-frame" style="background:#f1f5fa; border-radius:10px; box-shadow:0 2px 8px #e0e7ef; padding:1em; width:350px; text-align:center;">
          <iframe width="420" height="240" src="https://www.youtube.com/embed/De90h8LAu8s?si=NYe8kRblGmphK6sL" title="Explicación sencilla y un poco de historia" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
          <div style="color:#2563eb; font-size:0.95em; margin-top:0.5em;">Video 1. Un poco de historia acerca de la flotación</div>
        </div>
      </div>
  </section>
  <section id="hidrostatica">
      <h2 class="subtitulo">Hidrostática</h2>
      <div class="videos-dos" style="display: flex; gap:2em; justify-content:center; margin:2em 0; flex-wrap:wrap;">
        <div class="video-frame" style="background:#f1f5fa; border-radius:10px; box-shadow:0 2px 8px #e0e7ef; padding:1em; width:350px; text-align:center;">
          <iframe width="420" height="240" src="https://www.youtube.com/embed/wLlXS5j0Fuo?si=4VcobNzDukEMLXPp" title="Explicación sencilla y un poco de historia" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
          <div style="color:#2563eb; font-size:0.95em; margin-top:0.5em;">Video 2. Principio fundamental</div>
        </div>
      </div>
      <div class="videos-dos" style="display: flex; gap:2em; justify-content:center; margin:2em 0; flex-wrap:nowrap;">
        <div class="video-frame" style="background:#f1f5fa; border-radius:10px; box-shadow:0 2px 8px #e0e7ef; padding:1em; width:350px; text-align:center;">
          <iframe width="420" height="240" src="https://www.youtube.com/embed/XoF9s5ODsHI?si=Xo0J_ZRFhEGfvuOS" title="Principio de Arquímedes - Flotación" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
          <div style="color:#2563eb; font-size:0.95em; margin-top:0.5em;">Video 3. Principio de Arquímedes - Flotación</div>
        </div>
      </div>
      <p class="parrafo"><a href="https://phet.colorado.edu/en/simulations/buoyancy" target="_blank" style="font-weight:bold; color:#2563eb; ">🔗 Explora la simulación: Flotabilidad (PHET Learning Media)</a></p>
      <div class="videos-dos" style="display: flex; gap:2em; justify-content:center; margin:2em 0; flex-wrap:nowrap;">
        <div class="video-frame" style="background:#f1f5fa; border-radius:10px; box-shadow:0 2px 8px #e0e7ef; padding:1em; width:350px; text-align:center;">
          <iframe width="420" height="240" src="https://www.youtube.com/embed/MyybIRPX010?si=3KgA-YKQonVgoqdw" title="Principio de Pascal - Presión hidráulica" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
          <div style="color:#2563eb; font-size:0.95em; margin-top:0.5em;">Video 4. Principio de Pascal - Presión hidráulica</div>
        </div>
      </div>
      <p class="parrafo"><a href="https://phet.colorado.edu/en/simulations/under-pressure" target="_blank" style="font-weight:bold; color:#2563eb; ">🔗 Explora la simulación: Under pressure (PHET Learning Media)</a></p>
    </section>
    <section id="hidrodinamica">
      <h2 class="subtitulo">Hidrodinámica</h2>
      <div class="videos-dos" style="display: flex; gap:2em; justify-content:center; margin:2em 0; flex-wrap:nowrap;">
        <div class="video-frame" style="background:#f1f5fa; border-radius:10px; box-shadow:0 2px 8px #e0e7ef; padding:1em; width:350px; text-align:center;">
          <iframe width="420" height="240" src="https://www.youtube.com/embed/DzWgqxUNIXM?si=uO7Rbjtow1MPceE8" title="Principio de Bernoulli" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
          <div style="color:#2563eb; font-size:0.95em; margin-top:0.5em;">Video 5. Principio de Bernoulli - ¿Por qué vuelan los aviones o las aves?</div>
        </div>
      </div>   
      <div class="videos-dos" style="display: flex; gap:2em; justify-content:center; margin:2em 0; flex-wrap:nowrap;">
        <div class="video-frame" style="background:#f1f5fa; border-radius:10px; box-shadow:0 2px 8px #e0e7ef; padding:1em; width:350px; text-align:center;">
          <iframe width="420" height="240" src="https://www.youtube.com/embed/3bkh3HkKL8w?si=Ms-ObWQZXU-kHuKm" title="Tipos de flujo y número de Reynolds" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
          <div style="color:#2563eb; font-size:0.95em; margin-top:0.5em;">Video 6. Tipos de flujo y número de Reynolds </div>
        </div>
      </div>   
      <div class="videos-dos" style="display: flex; gap:2em; justify-content:center; margin:2em 0; flex-wrap:nowrap;">
        <div class="video-frame" style="background:#f1f5fa; border-radius:10px; box-shadow:0 2px 8px #e0e7ef; padding:1em; width:350px; text-align:center;">
          <iframe width="420" height="240" src="https://www.youtube.com/embed/3rNQXXuyhMw?si=dzErP5rIVF1jJGjs" title="Ley de Torricelli" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
          <div style="color:#2563eb; font-size:0.95em; margin-top:0.5em;">Video 7. Ley de Torricelli </div>
        </div>
      </div>  
      <p class="parrafo"><a href="https://phet.colorado.edu/en/simulations/under-pressure" target="_blank" style="font-weight:bold; color:#2563eb; ">🔗 Explora la simulación: Presión y flujo (PHET Learning Media)</a></p>
     </section>
     <section id="tension">
     <h2 class="subtitulo">Tensión superficial y capilaridad</h2>
      <div class="videos-dos" style="display: flex; gap:2em; justify-content:center; margin:2em 0; flex-wrap:nowrap;">
        <div class="video-frame" style="background:#f1f5fa; border-radius:10px; box-shadow:0 2px 8px #e0e7ef; padding:1em; width:350px; text-align:center;">
          <iframe width="420" height="240" src="https://www.youtube.com/embed/y8Er1_cfKlU?si=16hIwG7p46JBb5Xn" title="Tensión superficial" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
          <div style="color:#2563eb; font-size:0.95em; margin-top:0.5em;">Video 8. Tensión superficial </div>
        </div>
        <div class="video-frame" style="background:#f1f5fa; border-radius:10px; box-shadow:0 2px 8px #e0e7ef; padding:1em; width:350px; text-align:center;">
          <iframe width="420" height="240" src="https://www.youtube.com/embed/zB6QxKT9GT8?si=JiewnNkDDg6FAJJB" title="Capilaridad" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
          <div style="color:#2563eb; font-size:0.95em; margin-top:0.5em;">Video 9. Capilaridad </div>
        </div>
      </div>  
      </section>
      <section id="osmosis">
        <h2 class="subtitulo">Osmosis</h2>
        <div class="videos-dos" style="display: flex; gap:2em; justify-content:center; margin:2em 0; flex-wrap:nowrap;">
          <div class="video-frame" style="background:#f1f5fa; border-radius:10px; box-shadow:0 2px 8px #e0e7ef; padding:1em; width:350px; text-align:center;">
            <iframe width="420" height="240" src="https://www.youtube.com/embed/xcDNAxwIMkY?si=Xo5kpRMd27LmQ5AD" title="Ósmosis" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
            <div style="color:#2563eb; font-size:0.95em; margin-top:0.5em;">Video 10. Ósmosis </div>
          </div>
        </div>  
        <p class="parrafo"><a href="https://phet.colorado.edu/en/simulations/membrane-transport" target="_blank" style="font-weight:bold; color:#2563eb; ">🔗 Explora la simulación: Transporte en una membrana (PHET Learning Media)</a></p>
        <p class="parrafo"><a href="https://phet.colorado.edu/en/simulations/neuron" target="_blank" style="font-weight:bold; color:#2563eb; ">🔗 Explora la simulación: Neurona (PHET Learning Media)</a></p>
      </section>
  </main>
</body>
</html>
