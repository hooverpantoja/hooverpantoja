<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Biofísica</title>
  <style>
    *, *::before, *::after { box-sizing: border-box; }
    body {
      font-family: 'Segoe UI', Arial, sans-serif;
      background: #f8fafc;
      margin: 0;
      padding: 0;
      display: flex;
      min-height: 100vh;
    }
    nav {
      width: 240px;
      background: #f4f4f4;
      padding: 2em 1.2em;
      min-height: 100vh;
      box-shadow: 2px 0 8px #e0e7ef;
      border-right: 1px solid #e0e7ef;
      position: fixed;
      top: 0; left: 0;
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
    nav li { margin-bottom: 0.5em; }
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
    main {
      flex: 1;
      padding: 2em 2em;
      background: #fff;
      min-height: 100vh;
      margin-left: 240px;
      overflow-wrap: break-word;
      word-wrap: break-word;
    }
    .container {
      max-width: 900px;
      margin: 0 auto;
      overflow-x: auto;
    }
    h1 {
      font-size: 2.2em;
      color: #1a365d;
      margin-bottom: 0.5em;
      text-align: center;
    }
    h2 {
      font-size: 1.5em;
      color: #2563eb;
      margin-top: 2em;
      margin-bottom: 1em;
    }
    p {
      font-size: 1em;
      color: #222;
      line-height: 1.7;
      margin-bottom: 1.2em;
    }
    .modulo-card {
      background: #fff;
      border-radius: 12px;
      box-shadow: 0 2px 12px #e0e7ef;
      padding: 1.5em 2em;
      margin-bottom: 1.5em;
      border-left: 5px solid #2563eb;
      transition: box-shadow 0.2s;
    }
    .modulo-card:hover {
      box-shadow: 0 4px 20px #c7d2fe;
    }
    .modulo-card h3 {
      margin: 0 0 0.4em 0;
      font-size: 1.2em;
      color: #1a365d;
    }
    .modulo-card h3 a {
      color: #1a365d;
      text-decoration: none;
    }
    .modulo-card h3 a:hover {
      color: #2563eb;
      text-decoration: underline;
    }
    .modulo-card .desc {
      color: #555;
      font-size: 0.95em;
      margin: 0;
    }
    .modulo-card .meta {
      color: #888;
      font-size: 0.85em;
      margin-top: 0.3em;
    }
    a {
      font-size: 1em;
      color: #1a365d;
      text-decoration: underline;
    }

    @media (max-width: 900px) {
      body { flex-direction: column; }
      nav {
        position: static;
        width: 100%;
        height: auto;
        min-height: auto;
      }
      main {
        margin-left: 0;
        padding: 1em;
      }
      .container {
        padding: 1em;
      }
    }
  </style>
</head>
<body>
  <nav>
    <h2>Temario</h2>
    <ul>
      <li><a href="#introduccion">Introducción</a></li>
      <li><a href="#biomecanica">Biomecánica</a></li>
      <li><a href="#ondas">Ondas y electromagnetismo</a></li>
      <li><a href="#termodinamica">Termodinámica</a></li>
      <li><a href="#fluidos">Mecánica de fluidos</a></li>
      <li><a href="#proyecto">Proyecto Final</a></li>
    </ul>
    <hr>
    <h2>Recursos</h2>
    <ul>
      <li><a href="res/Microcurrículo.pdf">Microcurrículo</a></li>
      <li><a href="https://drive.google.com/drive/folders/1-8WeZK28iaaEToQVGgGCnHxfx8AhXX3f?usp=sharing">Fundamentos físicos de los fenómenos biológicos</a></li>
    </ul>
    <h2>Autores</h2>
    <ul>
      <li><a href="https://www.researchgate.net/profile/Hoover-Pantoja-Sanchez">Hoover Pantoja-Sánchez</a></li>
      <li><a href="https://www.researchgate.net/profile/Marco-Giraldo">Marco A. Giraldo</a></li>
    </ul>
    <hr>
    <a href="../" style="display:inline-block; margin-top:1em;">&#8592; Volver al perfil</a>
  </nav>
  <main>
    <div class="container">
      <h1>Biofísica</h1>
      <p style="text-align:center; color:#555; margin-bottom:2em;">Fundamentos físicos de los fenómenos biológicos en contextos marinos y costeros</p>
      <section id="introduccion">
        <h2>Módulo 1 &mdash; Introducción y conceptos fundamentales</h2>
        <div class="modulo-card">
          <h3><a href="semana1/">Semana 1: El método científico</a></h3>
          <p class="desc">Presentación del curso, el método científico, hechos vs. opiniones, ecología de zonas costeras.</p>
          <p class="meta">Jueves Sept 12, 09:00–12:00</p>
        </div>
        <div class="modulo-card">
          <h3><a href="semana2/">Semana 2: Magnitudes, unidades, vectores y leyes de escala</a></h3>
          <p class="desc">Magnitudes físicas, análisis dimensional, sistemas de unidades, vectores, tamaño y forma, leyes de escala isométricas y alométricas.</p>
          <p class="meta">Jueves Sept 19, 09:00–12:00</p>
        </div>
      </section>
      <section id="biomecanica">
        <h2>Módulo 2 &mdash; Biomecánica</h2>
        <div class="modulo-card">
          <h3><a href="semana3/">Semana 3: Cinemática</a></h3>
          <p class="desc">Posición, trayectoria, velocidad, aceleración, caída libre, movimiento circular, proyectiles e implicaciones biológicas.</p>
          <p class="meta">Jueves Sept 26, 09:00–12:00</p>
        </div>
        <div class="modulo-card">
          <h3><a href="semana4/">Semana 4: Dinámica, trabajo y energía</a></h3>
          <p class="desc">Leyes de Newton, fuerzas fundamentales y derivadas, gravitación, trabajo, energía cinética y potencial, calorimetría.</p>
          <p class="meta">Jueves Oct 2, 09:00–12:00</p>
        </div>
      </section>
      <section id="ondas">
        <h2>Módulo 3 &mdash; Ondas, radiación y electromagnetismo</h2>
        <div class="modulo-card">
          <h3><a href="semana5/">Semanas 5–6: Ondas mecánicas, sonido, luz y electromagnetismo</a></h3>
          <p class="desc">Ondas mecánicas y electromagnéticas, sonido (frecuencia, decibelios), electricidad, magnetismo, ecuaciones de Maxwell, radiación.</p>
          <p class="meta">Jueves Oct 10 y Oct 17, 09:00–12:00</p>
        </div>
      </section>
      <section id="termodinamica">
        <h2>Módulo 4 &mdash; Termodinámica</h2>
        <div class="modulo-card">
          <h3><a href="semana7/">Semanas 7–8: Termodinámica</a></h3>
          <p class="desc">Temperatura, calor, trabajo, leyes de la termodinámica, entropía, gases ideales, transiciones de fase.</p>
          <p class="meta">Jueves Oct 24 y Oct 31, 09:00–12:00</p>
        </div>
      </section>
      <section id="fluidos">
        <h2>Módulo 5 &mdash; Mecánica de fluidos</h2>
        <div class="modulo-card">
          <h3><a href="mecanicaF/">Semanas 9–10: Mecánica de fluidos</a></h3>
          <p class="desc">Hidrostática (presión, Arquímedes, Pascal), hidrodinámica (Bernoulli, Reynolds, Torricelli), tensión superficial, capilaridad, ósmosis.</p>
          <p class="meta">Jueves Nov 7 y Nov 14, 09:00–12:00</p>
        </div>
      </section>
      <section id="proyecto">
        <h2>Módulo 6 &mdash; Proyecto Final y Evaluación</h2>
        <div class="modulo-card">
          <h3>Semana 11: Presentación proyecto final</h3>
          <p class="meta">Jueves Nov 21, 09:00–12:00</p>
        </div>
        <div class="modulo-card">
          <h3>Semana 12: Cierre de evaluaciones</h3>
          <p class="meta">Jueves Nov 28, 09:00–12:00</p>
        </div>
      </section>
    </div>
  </main>
</body>
</html>
