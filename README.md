<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Hoover Pantoja - Perfil</title>
  <style>
    *, *::before, *::after { box-sizing: border-box; }
    body {
      font-family: 'Segoe UI', Arial, sans-serif;
      background: #f8fafc;
      margin: 0;
      padding: 0;
      color: #222;
    }
    header {
      background: linear-gradient(135deg, #1a365d 0%, #2563eb 100%);
      color: #fff;
      padding: 2.5em 2em 2em;
      text-align: center;
    }
    header h1 {
      font-size: 2.2em;
      margin: 0 0 0.3em;
      letter-spacing: 0.5px;
    }
    header p.tagline {
      font-size: 1.05em;
      opacity: 0.9;
      margin: 0 0 1.2em;
    }
    .nav-links {
      display: flex;
      justify-content: center;
      gap: 0.8em;
      flex-wrap: wrap;
      list-style: none;
      margin: 0;
      padding: 0;
    }
    .nav-links a {
      font-size: 0.95em;
      color: #fff;
      text-decoration: none;
      padding: 0.45em 1.1em;
      border-radius: 6px;
      background: rgba(255,255,255,0.15);
      transition: background 0.2s, transform 0.15s;
      display: inline-block;
    }
    .nav-links a:hover {
      background: rgba(255,255,255,0.3);
      transform: translateY(-1px);
    }
    .container {
      max-width: 860px;
      margin: 0 auto;
      padding: 2em 2.5em 3em;
    }
    .profile-card {
      display: flex;
      align-items: flex-start;
      gap: 2em;
      background: #fff;
      border-radius: 12px;
      box-shadow: 0 4px 16px #e0e7ef;
      padding: 2em 2.5em;
      margin-top: -2.5em;
      position: relative;
      z-index: 1;
    }
    .profile-card img {
      width: 120px;
      height: 120px;
      object-fit: cover;
      border-radius: 50%;
      border: 3px solid #e0e7ef;
      flex-shrink: 0;
    }
    .profile-card .bio {
      flex: 1;
      line-height: 1.7;
      font-size: 1em;
      color: #333;
    }
    .profile-card .affiliations {
      margin-top: 1em;
      font-size: 0.95em;
      color: #555;
    }
    .profile-card .affiliations a { color: #2563eb; }
    section.cv-section {
      background: #fff;
      border-radius: 12px;
      box-shadow: 0 4px 16px #e0e7ef;
      padding: 2em 2.5em;
      margin-top: 1.5em;
    }
    section.cv-section h2 {
      font-size: 1.4em;
      color: #1a365d;
      margin-top: 0;
      margin-bottom: 1em;
      padding-bottom: 0.4em;
      border-bottom: 2px solid #e0e7ef;
    }
    section.cv-section ul {
      padding-left: 0;
      list-style: none;
    }
    section.cv-section li {
      padding: 0.6em 0 0.6em 1.2em;
      border-left: 3px solid #2563eb;
      margin-bottom: 0.8em;
      line-height: 1.6;
    }
    section.cv-section li strong { color: #1a365d; }
    section.cv-section a { color: #2563eb; text-decoration: none; }
    section.cv-section a:hover { text-decoration: underline; }
    .distinction {
      border-left-color: #f59e0b !important;
    }
    footer {
      text-align: center;
      padding: 2em;
      color: #888;
      font-size: 0.9em;
    }
    @media (max-width: 700px) {
      .profile-card {
        flex-direction: column;
        align-items: center;
        text-align: center;
        padding: 1.5em;
      }
      .container { padding: 1em; }
      section.cv-section { padding: 1.5em; }
      header { padding: 1.5em 1em; }
      header h1 { font-size: 1.6em; }
      .nav-links a { font-size: 0.85em; padding: 0.4em 0.8em; }
    }
  </style>
</head>
<body>
  <header>
    <h1>Hoover Pantoja-Sánchez</h1>
    <p class="tagline">Bioingeniero · Doctor en Ingeniería Electrónica · Bioacústica </p>
    <ul class="nav-links">
      <li><a href="https://scholar.google.com/citations?hl=es&user=P25cVk0AAAAJ&view_op=list_works&sortby=pubdate">Google Scholar</a></li>
      <li><a href="https://www.researchgate.net/profile/Hoover-Pantoja-Sanchez?ev=hdr_xprf">ResearchGate</a></li>
      <li><a href="https://github.com/hooverpantoja">GitHub</a></li>
      <li><a href="classes/">Clases</a></li>
      <li><a href="https://docs.google.com/document/d/169RXjrX9qdvuedMKvQ1fy9OIzpFIRpxa/edit?usp=sharing&ouid=104479509763680947324&rtpof=true&sd=true">CV</a></li>
    </ul>
  </header>

  <div class="container">
    <div class="profile-card">
      <img src="res/Photo%20face.jpeg" alt="Hoover Pantoja-Sánchez" />
      <div>
        <p class="bio">Soy bioingeniero y doctor en Ingeniería Electrónica de la Universidad de Antioquia y con formación posdoctoral en biología sensorial. Me interesa la intersección entre la ingeniería, la biología y la ecología. Creo que los organismos biológicos son una fuente de inspiración para el desarrollo tecnológico y que la ingeniería es fundamental para poder entender la naturaleza. Mis áreas de experticia son la bioacústica, la ecoacústica y la neurociencia en insectos.</p>
        <div class="affiliations">
          <strong>Afiliaciones:</strong> Universidad de Antioquia · <a href="https://bernal-lab.weebly.com/team.html">Purdue University</a> · <a href="https://manacus.github.io/Manacus/">Fundación Manacus</a><br>
          <strong>Email:</strong> <a href="mailto:hoover.pantoja@udea.edu.co">hoover.pantoja@udea.edu.co</a>
        </div>
      </div>
    </div>

    <section class="cv-section">
      <h2>Experiencia</h2>
      <ul>
        <li><strong>Curador de la <a href="https://colecciones.humboldt.org.co/sonidos/">Colección de Sonidos Ambientales</a></strong>, Instituto Humboldt, 2021 – 2024</li>
        <li><strong>Investigador Posdoctoral – <a href="https://bernal-lab.weebly.com/team.html">Lab. Bernal de Biología Sensorial y Evolutiva</a></strong>, Purdue University, 2019 – 2021</li>
        <li><strong>Profesor de Cátedra – <a href="https://pecet-colombia.org/pecet/">Facultad de Medicina</a></strong>, Universidad de Antioquia, 2019</li>
        <li><strong>Joven Investigador – <a href="https://pecet-colombia.org/pecet/">PECET</a></strong>, Universidad de Antioquia, 2014 – 2015</li>
      </ul>
    </section>

    <section class="cv-section">
      <h2>Educación</h2>
      <ul>
        <li><strong>Doctorado en Ingeniería Electrónica</strong>, Universidad de Antioquia, 2015 – 2019</li>
        <li><strong>Bioingeniería</strong>, Universidad de Antioquia, 2013</li>
      </ul>
    </section>

    <section class="cv-section">
      <h2>Distinciones</h2>
      <ul>
        <li class="distinction"><strong><a href="https://www.biologists.com/100-years/100-biologists/">100 biólogos extraordinarios</a></strong>, Journal of Experimental Biology, 2025</li>
        <li class="distinction"><strong><a href="https://journals.biologists.com/jeb/article/227/3/jeb247403/342993/Announcing-the-2023-Journal-of-Experimental">Outstanding Paper Prize</a></strong>, Journal of Experimental Biology, 2023</li>
        <li class="distinction"><strong>Mejor proyecto de investigación en medicina tropical</strong>, Universidad CES, 2017</li>
        <li class="distinction"><strong>Mejor estudiante de posgrado en Latinoamérica</strong>, Asoc. Americana de Control de Mosquitos, 2016</li>
      </ul>
    </section>
  </div>

  <footer>
    &copy; Hoover Pantoja-Sánchez · Universidad de Antioquia
  </footer>
</body>
</html>