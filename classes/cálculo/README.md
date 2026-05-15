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
    nav li ul {
      margin-top: 0.4em;
      margin-left: 0.7em;
      margin-bottom: 0.8em;
      border-left: 2px solid #dbe4f4;
      padding-left: 0.7em;
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
    nav a:hover { background: #2563eb; color: #fff; }
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
      max-width: 100%;
      margin: 0 auto;
      overflow-x: auto;
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
      margin: 0 0 0.7em;
    }
    .estado {
      display: inline-block;
      font-size: 0.8em;
      border-radius: 999px;
      padding: 0.2em 0.8em;
      margin-bottom: 0.8em;
      background: #dcfce7;
      color: #166534;
    }
    .estado.dev {
      background: #fff7ed;
      color: #9a3412;
    }
    .temas-clave {
      margin: 0.5em 0 0;
      padding-left: 1.2em;
      color: #475569;
      line-height: 1.6;
      font-size: 0.9em;
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
      <li>
        <a href="#multivariable">Cálculo multivariable</a>
        <ul>
          <li><a href="calculo-multivariable/gradiente.html">Gradiente</a></li>
          <li><a href="calculo-multivariable/divergencia.html">Divergencia</a></li>
          <li><a href="calculo-multivariable/rotacional.html">Rotacional</a></li>
        </ul>
      </li>
      <li>
        <a href="#ecuaciones-diferenciales">Ecuaciones diferenciales</a>
        <ul>
          <li><a href="ecuaciones-diferenciales/edo-primer-orden.html">EDO de primer orden</a></li>
          <li><a href="ecuaciones-diferenciales/edo-segundo-orden.html">EDO de segundo orden</a></li>
          <li><a href="ecuaciones-diferenciales/funcion-green.html">Función de Green</a></li>
        </ul>
      </li>
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
        <span class="estado">Disponible</span>
        <ul class="temas-clave">
          <li>Gradiente, derivada direccional y campo escalar</li>
          <li>Divergencia y flujo en campos vectoriales</li>
          <li>Rotacional y circulación</li>
        </ul>
      </div>
      <div class="modulo-card" id="ecuaciones-diferenciales">
        <h2><a href="ecuaciones-diferenciales/">Ecuaciones diferenciales</a></h2>
        <p class="desc">EDOs y EDPs: separación de variables, series de potencias, método de Green</p>
        <p class="meta">2 semanas · 8h · +50 XP al completar</p>
        <span class="estado">Disponible</span>
        <ul class="temas-clave">
          <li>EDO de primer y segundo orden</li>
          <li>Series de potencias y separación de variables</li>
          <li>Función de Green para problemas lineales</li>
        </ul>
      </div>
      <div class="modulo-card" id="algebra-lineal">
        <h2><a href="algebra-lineal-avanzada/">Álgebra lineal avanzada</a></h2>
        <p class="desc">Eigenvalores, vectores propios, diagonalización, formas cuadráticas</p>
        <p class="meta">2 semanas · 8h · +50 XP al completar</p>
        <span class="estado dev">En desarrollo</span>
        <ul class="temas-clave">
          <li>Espacios vectoriales y transformaciones lineales</li>
          <li>Diagonalización y forma de Jordan</li>
          <li>Descomposición en valores singulares (SVD)</li>
        </ul>
      </div>
      <div class="modulo-card" id="tensorial">
        <h2><a href="calculo-tensorial/">Cálculo tensorial</a></h2>
        <p class="desc">Tensores covariantes y contravariantes, notación de Einstein, métrica</p>
        <p class="meta">2 semanas · 8h · +50 XP al completar</p>
        <span class="estado dev">En desarrollo</span>
        <ul class="temas-clave">
          <li>Notación de índices y convención de Einstein</li>
          <li>Derivada covariante y transporte paralelo</li>
          <li>Tensor de curvatura de Riemann</li>
        </ul>
      </div>
      <div class="modulo-card" id="fourier">
        <h2><a href="analisis-funcional-fourier/">Análisis funcional y de Fourier</a></h2>
        <p class="desc">Series de Fourier, espacios de Hilbert, distribuciones de Schwartz</p>
        <p class="meta">2 semanas · 8h · +50 XP al completar</p>
        <span class="estado dev">En desarrollo</span>
        <ul class="temas-clave">
          <li>Series y transformada de Fourier</li>
          <li>Espacios de Hilbert y operadores lineales</li>
          <li>Distribuciones de Schwartz y delta de Dirac</li>
        </ul>
      </div>
    </div>
  </main>
</body>
</html>
