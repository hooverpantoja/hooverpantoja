<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Semana 1 - El método científico</title>
  <script>
    window.MathJax = {
      tex: { inlineMath: [['\\(','\\)']], displayMath: [['\\[','\\]']] }
    };
  </script>
  <script src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-chtml.js" async></script>
  <style>
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
      padding: 2.5em 3em;
      background: #fff;
      min-height: 100vh;
      margin-left: 240px;
    }
    .container {
      max-width: 900px;
      margin: 0 auto;
      background: #fff;
      border-radius: 12px;
      box-shadow: 0 4px 16px #e0e7ef;
      padding: 2em 2.5em;
    }
    .titulo-principal {
      font-size: 2.2em;
      color: #1a365d;
      margin-bottom: 0.5em;
      text-align: center;
    }
    .subtitulo {
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
    .definicion {
      background: #eef2ff;
      border-left: 5px solid #2563eb;
      padding: 1.2em 1.5em;
      border-radius: 0 10px 10px 0;
      margin: 1.5em 0;
      font-size: 1em;
      line-height: 1.7;
    }
    .ejemplo {
      background: #f0fdf4;
      border-left: 5px solid #16a34a;
      padding: 1.2em 1.5em;
      border-radius: 0 10px 10px 0;
      margin: 1.5em 0;
      line-height: 1.7;
    }
    .nota {
      background: #fffbeb;
      border-left: 5px solid #f59e0b;
      padding: 1.2em 1.5em;
      border-radius: 0 10px 10px 0;
      margin: 1.5em 0;
      line-height: 1.7;
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
      padding: 10px;
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
<body>
  <!-- NAV LATERAL -->
  <nav>
    <h2>Temario</h2>
    <ul>
      <li><a href="#metodo-cientifico">El método científico</a></li>
      <li><a href="#conceptos">Conceptos fundamentales</a></li>
      <li><a href="#ecologia">Ecología de Zonas Costeras</a></li>
      <li><a href="#ejercicio">Ejercicio resuelto</a></li>
    </ul>
    <hr>
    <h2>Recursos</h2>
    <ul>
      <li><a href="../res/Microcurrículo.pdf">Microcurrículo</a></li>
      <li><a href="https://drive.google.com/drive/folders/1-8WeZK28iaaEToQVGgGCnHxfx8AhXX3f?usp=sharing">Fundamentos</a></li>
    </ul>
    <h2>Autores</h2>
    <ul>
      <li><a href="https://www.researchgate.net/profile/Hoover-Pantoja-Sanchez">Hoover Pantoja-Sánchez</a></li>
      <li><a href="https://www.researchgate.net/profile/Marco-Giraldo">Marco A. Giraldo</a></li>
    </ul>
    <a href="../">&#8592; Volver al cronograma</a>
  </nav>

  <!-- CONTENIDO PRINCIPAL -->
  <main>
    <div class="container">

      <h1 class="titulo-principal">Semana 1</h1>
      <p class="parrafo" style="text-align:center; color:#555;">Biofísica &mdash; Introducción al método científico</p>

      <!-- ==================== EL MÉTODO CIENTÍFICO ==================== -->
      <h2 class="subtitulo" id="metodo-cientifico">El método científico</h2>

      <div class="definicion">
        <strong>Definición &mdash; Método científico:</strong> Es una herramienta sistemática y estructurada diseñada para responder preguntas sobre el mundo que nos rodea de la manera más objetiva posible, a partir de evidencia, intentando eliminar los sesgos y usando la curiosidad como motor principal.
      </div>

      <div class="texto">
        <p class="parrafo">Entender claramente el concepto del método científico es una de las necesidades más importantes de nuestra época. En la actualidad, la distinción entre lo real y lo verdadero se ha vuelto un reto. Las burbujas de auto-confirmación creadas por las redes sociales y potenciadas por la inteligencia artificial, nos distancian como comunidad ya que moldean nuestra percepción del mundo de una manera sesgada, casi del mismo modo en que se ajustan nuestros gustos por la música, las compras o las películas. La persona que está a tu lado, probablemente tiene una percepción completamente distinta de la realidad. Sus gustos, creencias y opiniones se han construido, con una fuerte influencia de algoritmos desarrollados para incrementar el consumo de bienes y experiencias. Estos algoritmos operan en un bucle de retroalimentación que prioriza lo que te gusta o lo que crees correcto, recompensándote constantemente con microdosis de dopamina. Sin saberlo, nos convertimos en adictos: a videos de gatitos, a memes, a comprar… pero, sobre todo, a que nos den la razón. ¿Crees poder diferenciar hechos de opiniones? <a href="https://www.netflix.com/co/title/81254224">sugerencia: El dilema de las redes sociales</a></p>
        <p class="parrafo">Cuando las opiniones se presentan como hechos, se genera una confusión peligrosa. En este contexto, el método científico se convierte en una herramienta esencial: nos brinda una estratgegia para responder preguntas de la manera más objetiva posible, a partir de evidencia, intentando eliminar los sesgos y usando la curiosidad como motor principal. </p>
      </div>

      <div class="nota">
        <strong>Nota:</strong> La ciencia no busca "tener la razón"; busca acercarse a la verdad a través de un proceso iterativo de observación, prueba y corrección. Un resultado negativo (una hipótesis rechazada) es tan valioso como uno positivo.
      </div>

      <div class="texto">
        <p class="parrafo"><strong>Pasos del método científico:</strong></p>
        <ul>
          <li><strong>Paso 1:</strong> Observación y generación de la pregunta &mdash; Preguntas de si/no y preguntas acerca del fenómeno ¿cómo?, o ¿por qué?</li>
          <li><strong>Paso 2:</strong> Formulación de hipótesis</li>
          <li><strong>Paso 3:</strong> Experimentación</li>
          <li><strong>Paso 4:</strong> Análisis de resultados para llegar a conclusiones <strong>verificables y reproducibles</strong>.</li>
        </ul>
      </div>

      <!-- ==================== CONCEPTOS FUNDAMENTALES ==================== -->
      <h2 class="subtitulo" id="conceptos">Conceptos fundamentales</h2>

      <div class="definicion">
        <strong>Hipótesis:</strong> Una suposición o explicación provisional que puede ser probada mediante experimentación y análisis de datos. Ejemplo: <em>"Si la temperatura del agua aumenta, la tasa de respiración de los peces aumentará."</em>
      </div>
      <div class="definicion">
        <strong>Teoría:</strong> Una explicación generalizada y bien sustentada de un fenómeno, basada en pruebas repetidas y observaciones acumuladas. Ejemplo: <em>La teoría de la evolución por selección natural.</em>
      </div>
      <div class="definicion">
        <strong>Ley:</strong> Una descripción de un fenómeno natural que ocurre de manera constante bajo condiciones específicas. Ejemplo: <em>La ley de la gravitación universal de Newton.</em>
      </div>

      <table>
        <thead>
          <tr>
            <th>Concepto</th>
            <th>Definición</th>
            <th>Propósito</th>
            <th>Ejemplo</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>Hipótesis</td>
            <td>Una suposición o explicación provisional que puede ser probada mediante experimentación y análisis de datos.</td>
            <td>Proponer una explicación tentativa para un fenómeno específico y probar si es correcta o no.</td>
            <td>"Si la temperatura del agua aumenta, la tasa de respiración de los peces aumentará."</td>
          </tr>
          <tr>
            <td>Teoría</td>
            <td>Una explicación generalizada y bien sustentada de un fenómeno, basada en pruebas repetidas y observaciones.</td>
            <td>Explicar fenómenos relacionados de manera consistente, basada en evidencia experimental acumulada.</td>
            <td>La teoría de la evolución: Explica cómo las especies cambian a lo largo del tiempo por selección natural.</td>
          </tr>
          <tr>
            <td>Ley</td>
            <td>Una descripción de un fenómeno natural que ocurre de manera constante bajo condiciones específicas.</td>
            <td>Describir un fenómeno observable que siempre ocurre bajo las mismas condiciones.</td>
            <td>La ley de la gravitación universal de Newton: Todos los objetos se atraen entre sí con una fuerza que depende de sus masas y la distancia entre ellos.</td>
          </tr>
        </tbody>
      </table>

      <p class="parrafo">Por esta razón, la expresión "es solo una teoría", no tiene sentido, las teorías se construyen a partir de evidencia proporsionada por la comprobación de una gran cantidad de hipótesis. La teoría de la relatividad, por ejemplo, ha sido comprobada experimentalmente por investigadores de todo el mundo y en incontables escenarios. Sus leyes y limitaciones son claramente conocidas. </p>

      <div class="nota">
        <strong>Nota:</strong> En ciencia, una <em>teoría</em> no es una simple opinión o conjetura. Es el nivel más alto de validación que una explicación puede alcanzar, respaldada por evidencia experimental extensiva y reproducible.
      </div>

      <div class="videos-dos">
        <div class="video-frame">
          <iframe src="https://www.youtube.com/embed/mBKI2Z29hOk" allowfullscreen></iframe>
          <p>Discusión acerca del método científico</p>
        </div>
        <div class="video-frame">
          <iframe src="https://www.youtube.com/embed/lHtodB0S-zg?start=162" allowfullscreen></iframe>
          <p>Explicación detallada</p>
        </div>
      </div>

      <!-- ==================== EJEMPLO BIOLÓGICO ==================== -->
      <h2 class="subtitulo2">Ejemplo: El método científico aplicado a la biología marina</h2>

      <div class="ejemplo">
        <strong>Ejemplo &mdash; Estudio del blanqueamiento de coral:</strong>
        <ol>
          <li><strong>Observación:</strong> En un arrecife costero se observa que ciertos corales pierden su coloración durante los meses más cálidos del año.</li>
          <li><strong>Pregunta:</strong> ¿El aumento de la temperatura del agua es la causa principal del blanqueamiento de estos corales?</li>
          <li><strong>Hipótesis:</strong> Si la temperatura del agua supera los 29&thinsp;°C de forma sostenida durante más de dos semanas, los corales expulsan sus zooxantelas simbióticas, lo que provoca el blanqueamiento.</li>
          <li><strong>Experimentación:</strong> Se instalan sensores de temperatura en el arrecife y se monitorean colonias de coral durante 12 meses, registrando temperatura y porcentaje de blanqueamiento.</li>
          <li><strong>Análisis:</strong> Se aplica un análisis de correlación entre temperatura y porcentaje de blanqueamiento. Si \( r > 0.7 \) y \( p < 0.05 \), se concluye que existe una asociación estadísticamente significativa.</li>
        </ol>
      </div>

      <!-- ==================== ECOLOGÍA DE ZONAS COSTERAS ==================== -->
      <h1 class="titulo-principal" id="ecologia">El método científico en la Ecología de Zonas Costeras</h1>

      <p class="parrafo">Al concluir este curso, la persona estará capacitada para enunciar, comprender, describir, analizar, utilizar y aplicar los principios y leyes fundamentales de la biofísica en sistemas biológicos complejos dentro de contextos marinos y costeros. Se fomentará el reconocimiento y valoración de la importancia de una argumentación sistemática y rigurosa, promoviendo la práctica de debates fundamentados en diversas situaciones, explicadas inicialmente desde la biofísica marino-costera. Además, se buscará el desarrollo de habilidades en el estudiantado de ciencias del mar para entender, modelar y analizar procesos biofísicos tanto en organismos marinos como en ecosistemas acuáticos.</p>

      <h2 class="subtitulo" id="gestion">Gestión de Zonas Costeras</h2>

      <p class="parrafo">La gestión de zonas costeras debe basarse en evidencia clara; por lo tanto, responder preguntas utilizando el método científico es fundamental. De lo contrario, las decisiones y la normatividad generadas estarán cargadas de especulación, lo que impedirá que tengan el impacto deseado.</p>
      <div style="width:80%; display:flex; justify-content:center; margin:2em 0;" id="impacto">
        <img src="res/Gestión de Zonas costeras.png" alt="Gestión de zonas costeras" class="img-contenido" style="margin-bottom:0.5em; display:block; margin-left:auto; margin-right:auto;" />
      </div>
      <p class="parrafo">En el contexto actual de impacto ambiental asociado a las actividades productivas humanas, conocer los fenómenos y comprender su impacto es crucial para tomar decisiones informadas y acertadas. En particular, entender los fenómenos físicos que causan dicho impacto posibilita discusiones objetivas y permite mitigar dichos impactos, permitiendo el diseño e implementación de nuevos métodos de producción sostenibles o regenerativos.</p>
      <div style="width:100%; display:flex; justify-content:center; margin:2em 0;">
        <img src="res/Impacto Zonas Costeras.png" alt="Impacto en zonas costeras" class="img-contenido" />
      </div>

      <!-- ==================== EJERCICIO RESUELTO ==================== -->
      <h2 class="subtitulo" id="ejercicio">Ejercicio Resuelto: Diseñar un experimento usando el método científico</h2>

      <p class="parrafo"><strong>Problema:</strong> Se desea determinar si la temperatura del agua afecta la tasa de respiración de peces de una especie costera (<em>Mugil cephalus</em>). Diseñe un experimento completo aplicando los pasos del método científico.</p>

      <div class="ejemplo">
        <strong>Solución paso a paso:</strong>

        <p><strong>Paso 1 &mdash; Observación y pregunta:</strong></p>
        <p>Los pescadores locales reportan que los peces parecen más activos y respiran más rápido durante los meses cálidos. <br>
        <em>Pregunta:</em> ¿La temperatura del agua afecta significativamente la tasa de respiración de <em>Mugil cephalus</em>?</p>

        <p><strong>Paso 2 &mdash; Hipótesis:</strong></p>
        <p>\( H_0 \): La temperatura del agua no tiene efecto significativo sobre la tasa de respiración de los peces (\( \mu_{20°C} = \mu_{25°C} = \mu_{30°C} \)).</p>
        <p>\( H_1 \): La tasa de respiración aumenta significativamente con la temperatura del agua (\( \mu_{20°C} < \mu_{25°C} < \mu_{30°C} \)).</p>

        <p><strong>Paso 3 &mdash; Diseño experimental:</strong></p>
        <ul>
          <li><strong>Variable independiente:</strong> Temperatura del agua (20&thinsp;°C, 25&thinsp;°C, 30&thinsp;°C).</li>
          <li><strong>Variable dependiente:</strong> Tasa de respiración (medida como frecuencia opercular en movimientos/minuto).</li>
          <li><strong>Variables controladas:</strong> Salinidad, oxígeno disuelto, iluminación, tamaño de los peces, volumen del acuario.</li>
          <li><strong>Réplicas:</strong> 10 peces por tratamiento (3 tratamientos &times; 10 réplicas = 30 individuos).</li>
          <li><strong>Protocolo:</strong> Aclimatar los peces durante 48&thinsp;h a cada temperatura. Registrar la frecuencia opercular durante 5 minutos por individuo.</li>
        </ul>

        <p><strong>Paso 4 &mdash; Análisis de resultados:</strong></p>
        <p>Se aplica un análisis de varianza (ANOVA) de un factor para comparar las medias entre los tres grupos:</p>
        \[
          F = \frac{\text{Varianza entre grupos}}{\text{Varianza dentro de los grupos}} = \frac{MS_{\text{entre}}}{MS_{\text{dentro}}}
        \]
        <p>donde:</p>
        \[
          MS_{\text{entre}} = \frac{SS_{\text{entre}}}{k - 1}, \qquad MS_{\text{dentro}} = \frac{SS_{\text{dentro}}}{N - k}
        \]
        <p>con \( k = 3 \) grupos y \( N = 30 \) individuos totales.</p>

        <p>Si el valor-\(p\) asociado al estadístico \( F \) es menor que el nivel de significancia \( \alpha = 0.05 \), se rechaza \( H_0 \) y se concluye que la temperatura tiene un efecto significativo sobre la tasa de respiración.</p>

        <p><strong>Incertidumbre en las mediciones:</strong></p>
        <p>Cada medición de frecuencia opercular tiene una incertidumbre asociada. Si se realizan \( n \) mediciones repetidas, la incertidumbre estándar de la media se calcula como:</p>
        \[
          u(\bar{x}) = \frac{s}{\sqrt{n}}
        \]
        <p>donde \( s \) es la desviación estándar muestral y \( n \) el número de mediciones. El resultado se reporta como \( \bar{x} \pm u(\bar{x}) \) movimientos/min.</p>

        <p><strong>Conclusión esperada:</strong></p>
        <p>Si \( F_{\text{calculado}} > F_{\text{crítico}} \) (o equivalentemente \( p < 0.05 \)), se confirma que la temperatura del agua afecta significativamente la tasa de respiración, apoyando la hipótesis alternativa \( H_1 \).</p>
      </div>

      <div class="nota">
        <strong>Nota sobre reproducibilidad:</strong> Para que este experimento sea válido dentro del método científico, debe ser <strong>reproducible</strong>: otro investigador, en otro laboratorio, debe poder replicar el protocolo y obtener resultados consistentes. Por ello es esencial documentar todas las condiciones experimentales con precisión.
      </div>

    </div>
  </main>
</body>
</html>
