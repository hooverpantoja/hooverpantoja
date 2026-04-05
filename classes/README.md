<html lang="es">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>Clases</title>
    <style>
      *, *::before, *::after { box-sizing: border-box; }
      body {
        font-family: 'Segoe UI', Arial, sans-serif;
        background: #f8fafc;
        margin: 0;
        padding: 0;
      }
      .container {
        max-width: 600px;
        margin: 3em auto;
        background: #fff;
        border-radius: 12px;
        box-shadow: 0 4px 16px #e0e7ef;
        padding: 2em 2.5em;
        text-align: center;
      }
      h1 {
        font-size: 2.2em;
        color: #1a365d;
        margin-bottom: 0.5em;
      }
      ul {
        list-style: none;
        padding: 0;
      }
      li {
        margin: 1.5em 0;
      }
      .btn-curso {
        font-size: 1.3em;
        color: #2563eb;
        text-decoration: none;
        padding: 0.5em 1.2em;
        border-radius: 6px;
        background: #e0e7ef;
        transition: background 0.2s, color 0.2s, transform 0.15s;
        display: inline-block;
      }
      .btn-curso:hover {
        background: #2563eb;
        color: #fff;
        transform: translateY(-1px);
      }
      .back-link {
        font-size: 1em;
        color: #1a365d;
        text-decoration: underline;
      }
      @media (max-width: 700px) {
        .container { margin: 1.5em 1em; padding: 1.5em; }
        h1 { font-size: 1.6em; }
        .btn-curso { font-size: 1.1em; padding: 0.5em 1em; }
      }
    </style>
</head>
<body>
  <div class="container">
    <h1>Clases</h1>
    <ul>
      <li><a class="btn-curso" href="biofisica/">Biofísica</a></li>
      <li><a class="btn-curso" href="cálculo/">Cálculo</a></li>
    </ul>
  </div>
  <div style="text-align:center; margin-top:2em;">
    <a class="back-link" href="../">&#8592; Volver al perfil</a>
  </div>
</body>
</html>