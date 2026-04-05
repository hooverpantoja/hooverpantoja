<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Cálculo</title>
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
    nav a:hover { background: #2563eb; color: #fff; }
    main {
      flex: 1;
      padding: 2.5em 3em;
      background: #fff;
      min-height: 100vh;
      margin-left: 240px;
      overflow-x: hidden;
    }
    .container {
      max-width: 900px;
      margin: 0 auto;
    }
    h1 {
      font-size: 2.2em;
      color: #1a365d;
      margin-bottom: 0.5em;
      text-align: center;
    }
    .modulo-card {
      background: #fff;
      border-radius: 12px;
      box-shadow: 0 2px 12px #e0e7ef;
      padding: 1.5em 2em;
      margin-bottom: 1.5em;
      border-left: 5px solid #2563eb;
      transition: box-shadow 0.2s, transform 0.15s;
    }
    .modulo-card:hover {
      box-shadow: 0 4px 20px #c7d2fe;
      transform: translateY(-2px);
    }
    .modulo-card h2 {
      margin: 0 0 0.4em;
      font-size: 1.3em;
      color: #1a365d;
    }
    .modulo-card h2 a {
      color: #1a365d;
      text-decoration: none;
    }
    .modulo-card h2 a:hover {
      color: #2563eb;
      text-decoration: underline;
    }
    .modulo-card .desc {
      color: #555;
      font-size: 0.95em;
      margin: 0 0 0.3em;
      line-height: 1.6;
    }
    .modulo-card .meta {
      color: #888;
      font-size: 0.85em;
      margin: 0;
    }
    .back-link {
      font-size: 1em;
      color: #1a365d;
      text-decoration: underline;
    }
    @media (max-width: 900px) {
      nav {
        position: static;
        width: 100%;
        height: auto;
        min-height: auto;
      }
      main {
        margin-left: 0;
        padding: 1.5em;
      }
      body { flex-direction: column; }
    }
  </style>
</head>
<body>
  <nav>
    <h2>Temario</h2>
    <ul>
      <li><a href="#multivariable">Cálculo multivariable</a></li>
      <li><a href="#ecuaciones-diferenciales">Ecuaciones diferenciales</a></li>
      <li><a href="#algebra-lineal">Álgebra lineal avanzada</a></li>
      <li><a href="#tensorial">Cálculo tensorial</a></li>
      <li><a href="#fourier">Análisis funcional y de Fourier</a></li>
    </ul>
    <hr>
    <a class="back-link" href="../">&#8592; Volver a Clases</a>
  </nav>

  <main>
    <div class="container">
      <h1>Cálculo</h1>

      <div class="modulo-card" id="multivariable">
        <h2><a href="calculo-multivariable/">Cálculo multivariable</a></h2>
        <p class="desc">Gradiente, divergencia, rotacional, teoremas de Gauss y Stokes</p>
        <p class="meta">2 semanas · 8h · +50 XP al completar</p>
      </div>

      <div class="modulo-card" id="ecuaciones-diferenciales">
        <h2><a href="ecuaciones-diferenciales/">Ecuaciones diferenciales</a></h2>
        <p class="desc">EDOs y EDPs: separación de variables, series de potencias, método de Green</p>
        <p class="meta">2 semanas · 8h · +50 XP al completar</p>
      </div>

      <div class="modulo-card" id="algebra-lineal">
        <h2><a href="algebra-lineal-avanzada/">Álgebra lineal avanzada</a></h2>
        <p class="desc">Eigenvalores, vectores propios, diagonalización, formas cuadráticas</p>
        <p class="meta">2 semanas · 8h · +50 XP al completar</p>
      </div>

      <div class="modulo-card" id="tensorial">
        <h2><a href="calculo-tensorial/">Cálculo tensorial</a></h2>
        <p class="desc">Tensores covariantes y contravariantes, notación de Einstein, métrica</p>
        <p class="meta">2 semanas · 8h · +50 XP al completar</p>
      </div>

      <div class="modulo-card" id="fourier">
        <h2><a href="analisis-funcional-fourier/">Análisis funcional y de Fourier</a></h2>
        <p class="desc">Series de Fourier, espacios de Hilbert, distribuciones de Schwartz</p>
        <p class="meta">2 semanas · 8h · +50 XP al completar</p>
      </div>
    </div>
  </main>
</body>
</html>
