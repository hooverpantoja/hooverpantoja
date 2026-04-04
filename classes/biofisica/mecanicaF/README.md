<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Mecánica de Fluidos — Biofísica</title>
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
      .container {
        padding: 1em !important;
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
<body>
  <nav aria-label="Navegación lateral">
    <h2>Temario</h2>
    <ul>
      <li><a href="#hidrostatica">Hidrostática</a></li>
      <li><a href="#hidrodinamica">Hidrodinámica</a></li>
      <li><a href="#tension">Tensión superficial</a></li>
      <li><a href="#osmosis">Ósmosis</a></li>
      <li><a href="#ejercicios">Ejercicios resueltos</a></li>
    </ul>
    <hr>
    <h2>Recursos</h2>
    <ul>
      <li><a href="../res/Microcurrículo.pdf">Microcurrículo</a></li>
      <li><a href="https://drive.google.com/drive/folders/1-8WeZK28iaaEToQVGgGCnHxfx8AhXX3f?usp=sharing">Fundamentos físicos de los fenómenos biológicos</a></li>
    </ul>
    <h2>Autores</h2>
    <ul>
      <li><a href="https://www.researchgate.net/profile/Hoover-Pantoja-Sanchez">Hoover Pantoja-Sánchez</a></li>
      <li><a href="https://www.researchgate.net/profile/Marco-Giraldo">Marco A. Giraldo</a></li>
    </ul>
    <hr>
    <a href="../">&#8592; Volver al cronograma</a>
  </nav>

  <main>
    <div class="container">

      <h1 class="titulo-principal">Mecánica de fluidos</h1>

      <p class="parrafo">La mecánica de fluidos estudia el comportamiento de líquidos y gases en reposo (hidrostática) y en movimiento (hidrodinámica). Comprender estos principios es esencial en biofísica: desde la circulación sanguínea y la respiración hasta la locomoción acuática y el transporte de agua en plantas, los fluidos gobiernan procesos vitales en todos los organismos.</p>

      <a href="https://drive.google.com/file/d/1H8DW8wL6wqH5nj7whNVQydUS1J91BVtO/view?usp=drive_link" target="_blank" style="display:block;margin:1em 0;font-weight:bold;color:#2563eb;">🎧 Escucha el podcast — Introducción a la Mecánica de fluidos</a>

      <div class="videos-dos">
        <div class="video-frame">
          <iframe width="420" height="240" src="https://www.youtube.com/embed/De90h8LAu8s?si=NYe8kRblGmphK6sL" title="Explicación sencilla y un poco de historia" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
          <div style="color:#2563eb; font-size:0.95em; margin-top:0.5em;">Video 1. Un poco de historia acerca de la flotación</div>
        </div>
      </div>

      <!-- ═══════════════════════════════════════════════ -->
      <!--  HIDROSTÁTICA                                   -->
      <!-- ═══════════════════════════════════════════════ -->
      <section id="hidrostatica">
        <h2 class="subtitulo">Hidrostática</h2>

        <p class="parrafo">La hidrostática se ocupa de los fluidos en reposo. La magnitud fundamental es la <strong>presión</strong>, que describe la fuerza que un fluido ejerce por unidad de área sobre una superficie.</p>

        <div class="definicion">
          <strong>Presión:</strong> Se define como la fuerza normal por unidad de área:
          \[ P = \frac{F}{A} \]
          Su dimensión es \([P] = M L^{-1} T^{-2}\) y su unidad en el SI es el <em>pascal</em>: \(1\;\text{Pa} = 1\;\text{N/m}^2\).
        </div>

        <div class="nota">
          <strong>Presión atmosférica:</strong> A nivel del mar la presión atmosférica estándar vale \(P_{\text{atm}} = 101\,325\;\text{Pa} \approx 1\;\text{atm}\). Esta presión actúa sobre todos los cuerpos sumergidos y debe sumarse a la presión hidrostática.
        </div>

        <p class="parrafo">La <strong>presión hidrostática</strong> aumenta linealmente con la profundidad. A una profundidad \(h\) bajo la superficie de un fluido de densidad \(\rho\):</p>
        \[ P = P_0 + \rho\, g\, h \]
        <p class="parrafo">donde \(P_0\) es la presión en la superficie (generalmente la atmosférica) y \(g \approx 9{,}8\;\text{m/s}^2\).</p>

        <h3 class="subtitulo2">Principio de Pascal</h3>
        <p class="parrafo">Un cambio de presión aplicado a un fluido incompresible confinado se transmite íntegramente a todos los puntos del fluido y a las paredes del recipiente. Este principio es la base de sistemas hidráulicos como frenos, prensas y jeringas.</p>

        <div class="definicion">
          <strong>Principio de Arquímedes:</strong> Todo cuerpo sumergido en un fluido experimenta una fuerza de empuje vertical hacia arriba igual al peso del fluido desplazado:
          \[ F_b = \rho_f\, V_{\text{sum}}\, g \]
          donde \(\rho_f\) es la densidad del fluido y \(V_{\text{sum}}\) el volumen sumergido del cuerpo.
        </p>
        </div>

        <p class="parrafo"><strong>Condición de flotación:</strong> un objeto flota si su densidad es menor que la del fluido (\(\rho_{\text{obj}} &lt; \rho_f\)). Si \(\rho_{\text{obj}} &gt; \rho_f\), el objeto se hunde.</p>

        <div class="ejemplo">
          <strong>Ejemplo — ¿Se hunde un pez en agua de mar?</strong><br>
          Un pez tiene densidad \(\rho_{\text{pez}} = 1050\;\text{kg/m}^3\) y el agua de mar \(\rho_{\text{mar}} = 1025\;\text{kg/m}^3\).<br>
          Como \(\rho_{\text{pez}} > \rho_{\text{mar}}\), el pez tiende a hundirse. Para compensar, muchos peces óseos poseen una <strong>vejiga natatoria</strong> llena de gas que reduce su densidad promedio y les permite alcanzar flotabilidad neutra.
        </div>

        <p class="parrafo"><strong>Relevancia biológica:</strong> La vejiga natatoria de los peces óseos es un órgano hidrostático que regula la densidad del animal ajustando el volumen de gas. Organismos marinos como medusas, cuya composición es mayoritariamente agua, tienen densidades muy cercanas a la del medio, lo que les permite mantenerse en suspensión con un gasto energético mínimo. Las ballenas y focas controlan su flotabilidad mediante la cantidad de aire en los pulmones y la distribución de grasa subcutánea (muy ligera).</p>

        <div class="videos-dos">
          <div class="video-frame">
            <iframe width="420" height="240" src="https://www.youtube.com/embed/wLlXS5j0Fuo?si=4VcobNzDukEMLXPp" title="Principio fundamental" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
            <div style="color:#2563eb; font-size:0.95em; margin-top:0.5em;">Video 2. Principio fundamental</div>
          </div>
        </div>
        <div class="videos-dos">
          <div class="video-frame">
            <iframe width="420" height="240" src="https://www.youtube.com/embed/XoF9s5ODsHI?si=Xo0J_ZRFhEGfvuOS" title="Principio de Arquímedes - Flotación" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
            <div style="color:#2563eb; font-size:0.95em; margin-top:0.5em;">Video 3. Principio de Arquímedes — Flotación</div>
          </div>
        </div>
        <p class="parrafo"><a href="https://phet.colorado.edu/en/simulations/buoyancy" target="_blank" style="font-weight:bold; color:#2563eb;">🔗 Explora la simulación: Flotabilidad (PHET Learning Media)</a></p>
        <div class="videos-dos">
          <div class="video-frame">
            <iframe width="420" height="240" src="https://www.youtube.com/embed/MyybIRPX010?si=3KgA-YKQonVgoqdw" title="Principio de Pascal - Presión hidráulica" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
            <div style="color:#2563eb; font-size:0.95em; margin-top:0.5em;">Video 4. Principio de Pascal — Presión hidráulica</div>
          </div>
        </div>
        <p class="parrafo"><a href="https://phet.colorado.edu/en/simulations/under-pressure" target="_blank" style="font-weight:bold; color:#2563eb;">🔗 Explora la simulación: Under pressure (PHET Learning Media)</a></p>
      </section>

      <!-- ═══════════════════════════════════════════════ -->
      <!--  HIDRODINÁMICA                                  -->
      <!-- ═══════════════════════════════════════════════ -->
      <section id="hidrodinamica">
        <h2 class="subtitulo">Hidrodinámica</h2>

        <p class="parrafo">La hidrodinámica estudia los fluidos en movimiento. Dos ecuaciones centrales —la de continuidad y la de Bernoulli— derivan de la conservación de la masa y la energía, respectivamente.</p>

        <h3 class="subtitulo2">Ecuación de continuidad</h3>
        <p class="parrafo">Para un fluido incompresible que circula por un tubo de sección variable, el caudal se conserva:</p>
        \[ A_1\, v_1 = A_2\, v_2 \]
        <p class="parrafo">Esto implica que, donde el tubo se estrecha, la velocidad aumenta y viceversa. En el sistema cardiovascular, la sección total de los capilares es enorme, por lo que la sangre fluye lentamente ahí, favoreciendo el intercambio de nutrientes y gases.</p>

        <div class="definicion">
          <strong>Ecuación de Bernoulli:</strong> Para un fluido ideal (incompresible, no viscoso) en régimen estacionario:
          \[ P + \tfrac{1}{2}\,\rho\, v^2 + \rho\, g\, h = \text{constante} \]
          La presión disminuye donde la velocidad aumenta. Este principio explica la sustentación aerodinámica en aves y aviones.
        </div>

        <div class="definicion">
          <strong>Número de Reynolds:</strong> Parámetro adimensional que predice la naturaleza del flujo:
          \[ \text{Re} = \frac{\rho\, v\, L}{\mu} \]
          donde \(L\) es una longitud característica y \(\mu\) la viscosidad dinámica del fluido.
          <ul>
            <li>\(\text{Re} &lt; 2000\): flujo <strong>laminar</strong> (capas paralelas ordenadas).</li>
            <li>\(\text{Re} &gt; 4000\): flujo <strong>turbulento</strong> (caótico, con vórtices).</li>
            <li>\(2000 &lt; \text{Re} &lt; 4000\): régimen de transición.</li>
          </ul>
        </div>

        <div class="nota">
          <strong>Flujo laminar y turbulento en vasos sanguíneos:</strong> En condiciones normales, la sangre fluye de forma laminar en la mayoría de los vasos (Re ≈ 1000 en la aorta). Sin embargo, en estenosis (estrechamientos por aterosclerosis) la velocidad local aumenta y Re puede superar 4000, generando turbulencia que produce soplos cardíacos audibles con el estetoscopio y daña el endotelio vascular.
        </div>

        <div class="ejemplo">
          <strong>Ejemplo — Número de Reynolds para una ballena nadando</strong><br>
          Una ballena azul nada a \(v = 10\;\text{m/s}\), con longitud corporal \(L = 25\;\text{m}\), en agua de mar (\(\rho = 1025\;\text{kg/m}^3\), \(\mu = 1{,}08 \times 10^{-3}\;\text{Pa·s}\)).
          \[ \text{Re} = \frac{1025 \times 10 \times 25}{1{,}08 \times 10^{-3}} \approx 2{,}37 \times 10^{8} \]
          El flujo alrededor de la ballena es altamente turbulento. Sin embargo, adaptaciones como piel lisa y forma hidrodinámica reducen la resistencia.
        </div>

        <h3 class="subtitulo2">Teorema de Torricelli</h3>
        <p class="parrafo">Un caso particular de Bernoulli: la velocidad de salida de un fluido por un orificio situado a una profundidad \(h\) bajo la superficie libre es:</p>
        \[ v = \sqrt{2\,g\,h} \]

        <h3 class="subtitulo2">Viscosidad y ley de Poiseuille</h3>
        <p class="parrafo">Los fluidos reales poseen viscosidad. Para flujo laminar en un tubo cilíndrico de radio \(r\) y longitud \(L\), el caudal volumétrico viene dado por la <strong>ley de Poiseuille</strong>:</p>
        \[ Q = \frac{\pi\, r^4\, \Delta P}{8\, \mu\, L} \]
        <p class="parrafo">La dependencia con \(r^4\) es crítica: una reducción del 50 % en el radio disminuye el flujo a un \(6{,}25\,\%\) del original. Esto explica por qué la aterosclerosis (que reduce el radio arterial) tiene un impacto desproporcionado sobre el flujo sanguíneo.</p>

        <p class="parrafo"><strong>Relevancia biológica:</strong> La circulación sanguínea obedece aproximadamente a la ley de Poiseuille en vasos pequeños. En peces, el agua fluye unidireccionalmente sobre las branquias gracias a un sistema contracorriente que maximiza la extracción de oxígeno. Las ballenas y delfines aprovechan formas hidrodinámicas y movimientos ondulatorios de la aleta caudal para minimizar el arrastre viscoso.</p>

        <div class="videos-dos">
          <div class="video-frame">
            <iframe width="420" height="240" src="https://www.youtube.com/embed/DzWgqxUNIXM?si=uO7Rbjtow1MPceE8" title="Principio de Bernoulli" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
            <div style="color:#2563eb; font-size:0.95em; margin-top:0.5em;">Video 5. Principio de Bernoulli — ¿Por qué vuelan los aviones o las aves?</div>
          </div>
        </div>
        <div class="videos-dos">
          <div class="video-frame">
            <iframe width="420" height="240" src="https://www.youtube.com/embed/3bkh3HkKL8w?si=Ms-ObWQZXU-kHuKm" title="Tipos de flujo y número de Reynolds" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
            <div style="color:#2563eb; font-size:0.95em; margin-top:0.5em;">Video 6. Tipos de flujo y número de Reynolds</div>
          </div>
        </div>
        <div class="videos-dos">
          <div class="video-frame">
            <iframe width="420" height="240" src="https://www.youtube.com/embed/3rNQXXuyhMw?si=dzErP5rIVF1jJGjs" title="Ley de Torricelli" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
            <div style="color:#2563eb; font-size:0.95em; margin-top:0.5em;">Video 7. Ley de Torricelli</div>
          </div>
        </div>
        <p class="parrafo"><a href="https://phet.colorado.edu/en/simulations/fluid-pressure-and-flow" target="_blank" style="font-weight:bold; color:#2563eb;">🔗 Explora la simulación: Presión y flujo (PHET Learning Media)</a></p>
      </section>

      <!-- ═══════════════════════════════════════════════ -->
      <!--  TENSIÓN SUPERFICIAL Y CAPILARIDAD              -->
      <!-- ═══════════════════════════════════════════════ -->
      <section id="tension">
        <h2 class="subtitulo">Tensión superficial y capilaridad</h2>

        <p class="parrafo">En la interfaz entre un líquido y otro medio, las moléculas superficiales experimentan una fuerza neta hacia el interior del líquido. Esta asimetría origina la <strong>tensión superficial</strong>, que hace que la superficie se comporte como una membrana elástica.</p>

        <div class="definicion">
          <strong>Tensión superficial:</strong> Se define como la fuerza por unidad de longitud a lo largo de la superficie:
          \[ \gamma = \frac{F}{L} \]
          Unidades: \(\text{N/m}\). Para el agua a 20 °C, \(\gamma \approx 0{,}073\;\text{N/m}\).
        </div>

        <div class="nota">
          <strong>¿Por qué importa la tensión superficial para organismos pequeños?</strong> A escalas milimétricas, la tensión superficial puede superar al peso. Insectos como los zapateros (<em>Gerridae</em>) se sostienen sobre el agua porque su peso no es suficiente para romper la superficie. Sus patas hidrófobas distribuyen la carga sobre una longitud de contacto grande, manteniendo \(F &lt; \gamma \cdot L\).
        </div>

        <h3 class="subtitulo2">Capilaridad</h3>
        <p class="parrafo">Cuando un tubo estrecho se introduce en un líquido, la combinación de adhesión (líquido-vidrio) y cohesión (líquido-líquido) produce un ascenso o descenso capilar. La altura de ascenso es:</p>
        \[ h = \frac{2\,\gamma\,\cos\theta}{\rho\, g\, r} \]
        <p class="parrafo">donde \(\theta\) es el ángulo de contacto y \(r\) el radio del tubo. Para el agua en vidrio (\(\theta \approx 0°\)), el menisco es cóncavo y el líquido asciende.</p>

        <h3 class="subtitulo2">Presión de Laplace</h3>
        <p class="parrafo">La curvatura de una superficie produce una diferencia de presión entre el interior y el exterior de una burbuja o gota esférica:</p>
        \[ \Delta P = \frac{2\,\gamma}{r} \]
        <p class="parrafo">Cuanto menor sea el radio, mayor es la presión interna. En los alvéolos pulmonares (r ≈ 0,1 mm), esta presión sería enorme sin la presencia de <strong>surfactante pulmonar</strong>, una mezcla de fosfolípidos que reduce \(\gamma\) y evita el colapso alveolar.</p>

        <p class="parrafo"><strong>Relevancia biológica:</strong> La capilaridad es fundamental en el transporte de agua en plantas (xilema). Los meniscos en los poros de las paredes celulares generan presiones negativas (tensión) que contribuyen a elevar la savia bruta decenas de metros. En nuestros pulmones, el surfactante reduce la tensión superficial de forma dinámica: más reducción al exhalar (alvéolos pequeños), evitando el colapso.</p>

        <div class="videos-dos">
          <div class="video-frame">
            <iframe width="420" height="240" src="https://www.youtube.com/embed/y8Er1_cfKlU?si=16hIwG7p46JBb5Xn" title="Tensión superficial" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
            <div style="color:#2563eb; font-size:0.95em; margin-top:0.5em;">Video 8. Tensión superficial</div>
          </div>
          <div class="video-frame">
            <iframe width="420" height="240" src="https://www.youtube.com/embed/zB6QxKT9GT8?si=JiewnNkDDg6FAJJB" title="Capilaridad" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
            <div style="color:#2563eb; font-size:0.95em; margin-top:0.5em;">Video 9. Capilaridad</div>
          </div>
        </div>
      </section>

      <!-- ═══════════════════════════════════════════════ -->
      <!--  ÓSMOSIS                                        -->
      <!-- ═══════════════════════════════════════════════ -->
      <section id="osmosis">
        <h2 class="subtitulo">Ósmosis</h2>

        <p class="parrafo">La ósmosis es el paso de solvente (generalmente agua) a través de una membrana semipermeable desde una solución de menor concentración de soluto hacia una de mayor concentración, tendiendo a igualar las concentraciones.</p>

        <div class="definicion">
          <strong>Ósmosis — Presión osmótica:</strong> La presión necesaria para detener el flujo osmótico se calcula con la ecuación de van 't Hoff:
          \[ \Pi = M\,R\,T \]
          donde \(M\) es la molaridad del soluto, \(R = 8{,}314\;\text{J/(mol·K)}\) la constante de gases y \(T\) la temperatura absoluta en kelvin.
        </div>

        <h3 class="subtitulo2">Tipos de soluciones</h3>
        <table>
          <thead>
            <tr><th>Tipo</th><th>Relación</th><th>Efecto en la célula</th></tr>
          </thead>
          <tbody>
            <tr><td><strong>Isotónica</strong></td><td>\(\Pi_{\text{ext}} = \Pi_{\text{int}}\)</td><td>Sin cambio neto de volumen.</td></tr>
            <tr><td><strong>Hipotónica</strong></td><td>\(\Pi_{\text{ext}} &lt; \Pi_{\text{int}}\)</td><td>El agua entra → la célula se hincha (turgencia en plantas; lisis en animales).</td></tr>
            <tr><td><strong>Hipertónica</strong></td><td>\(\Pi_{\text{ext}} &gt; \Pi_{\text{int}}\)</td><td>El agua sale → la célula se contrae (plasmólisis en plantas; crenación en eritrocitos).</td></tr>
          </tbody>
        </table>

        <p class="parrafo"><strong>Relevancia biológica:</strong> Los organismos marinos enfrentan un medio hipertónico y deben osmorregular activamente. Los peces óseos marinos beben agua de mar y excretan sal por las branquias. Los peces de agua dulce, en un medio hipotónico, absorben agua por ósmosis y excretan grandes volúmenes de orina diluida. En los riñones humanos, el asa de Henle crea un gradiente osmótico en la médula renal que permite concentrar la orina, conservando agua. La <strong>turgencia celular</strong> en plantas (consecuencia de la ósmosis en medio hipotónico) es la fuerza que mantiene erguidos los tallos herbáceos.</p>

        <div class="videos-dos">
          <div class="video-frame">
            <iframe width="420" height="240" src="https://www.youtube.com/embed/xcDNAxwIMkY?si=Xo5kpRMd27LmQ5AD" title="Ósmosis" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
            <div style="color:#2563eb; font-size:0.95em; margin-top:0.5em;">Video 10. Ósmosis</div>
          </div>
        </div>
        <p class="parrafo"><a href="https://phet.colorado.edu/en/simulations/membrane-transport" target="_blank" style="font-weight:bold; color:#2563eb;">🔗 Explora la simulación: Transporte en una membrana (PHET Learning Media)</a></p>
        <p class="parrafo"><a href="https://phet.colorado.edu/en/simulations/neuron" target="_blank" style="font-weight:bold; color:#2563eb;">🔗 Explora la simulación: Neurona (PHET Learning Media)</a></p>
      </section>

      <!-- ═══════════════════════════════════════════════ -->
      <!--  EJERCICIOS RESUELTOS                           -->
      <!-- ═══════════════════════════════════════════════ -->
      <section id="ejercicios">
        <h2 class="subtitulo">Ejercicios resueltos</h2>

        <!-- Ejercicio 1 -->
        <div class="ejemplo">
          <strong>Ejercicio 1: Presión a profundidad</strong>
          <p>Un buzo se sumerge a \(h = 30\;\text{m}\) en agua de mar (\(\rho = 1025\;\text{kg/m}^3\)). Su membrana timpánica tiene un área de \(A = 0{,}55\;\text{cm}^2 = 5{,}5 \times 10^{-5}\;\text{m}^2\).</p>
          <p><strong>a) Presión total sobre el buzo:</strong></p>
          \[
            P = P_0 + \rho\,g\,h = 101\,325 + 1025 \times 9{,}8 \times 30
          \]
          \[
            P = 101\,325 + 301\,350 = 402\,675\;\text{Pa} \approx 4{,}03 \times 10^5\;\text{Pa}
          \]
          <p>Esto equivale a aproximadamente \(3{,}98\;\text{atm}\), es decir, casi 4 veces la presión atmosférica.</p>
          <p><strong>b) Fuerza sobre la membrana timpánica:</strong></p>
          <p>La fuerza debida únicamente a la presión del agua (no la atmosférica, que actúa por ambos lados del tímpano si el oído medio se ecualiza):</p>
          \[
            \Delta P = \rho\,g\,h = 301\,350\;\text{Pa}
          \]
          \[
            F = \Delta P \times A = 301\,350 \times 5{,}5 \times 10^{-5} \approx 16{,}6\;\text{N}
          \]
          <p>Esta fuerza equivale al peso de ≈ 1,7 kg concentrado en un área pequeña, lo que subraya la importancia de la ecualización de presión (maniobra de Valsalva) al bucear.</p>
        </div>

        <!-- Ejercicio 2 -->
        <div class="ejemplo">
          <strong>Ejercicio 2: Flujo sanguíneo (Poiseuille)</strong>
          <p>
            La sangre fluye por una arteria de radio \(r = 2\;\text{mm} = 2 \times 10^{-3}\;\text{m}\), longitud \(L = 10\;\text{cm} = 0{,}1\;\text{m}\), con una diferencia de presión \(\Delta P = 400\;\text{Pa}\). La viscosidad de la sangre es \(\mu = 3{,}5 \times 10^{-3}\;\text{Pa·s}\).
          </p>
          <p><strong>a) Caudal volumétrico:</strong></p>
          \[
            Q = \frac{\pi\, r^4\, \Delta P}{8\, \mu\, L}
              = \frac{\pi \times (2 \times 10^{-3})^4 \times 400}{8 \times 3{,}5 \times 10^{-3} \times 0{,}1}
          \]
          \[
            Q = \frac{\pi \times 1{,}6 \times 10^{-11} \times 400}{2{,}8 \times 10^{-3}}
              = \frac{\pi \times 6{,}4 \times 10^{-9}}{2{,}8 \times 10^{-3}}
          \]
          \[
            Q = \frac{2{,}011 \times 10^{-8}}{2{,}8 \times 10^{-3}}
              \approx 7{,}18 \times 10^{-6}\;\text{m}^3\text{/s}
              \approx 7{,}18\;\text{mL/s}
          \]
          <p><strong>b) Efecto de la aterosclerosis:</strong></p>
          <p>Si la arteria se estrecha a \(r' = 1{,}5\;\text{mm}\):</p>
          \[
            \frac{Q'}{Q} = \left(\frac{r'}{r}\right)^4 = \left(\frac{1{,}5}{2{,}0}\right)^4 = (0{,}75)^4 = 0{,}3164
          \]
          \[
            Q' \approx 0{,}3164 \times 7{,}18 \approx 2{,}27\;\text{mL/s}
          \]
          <p>Una reducción del 25 % en el radio causa una caída del <strong>68 %</strong> en el flujo sanguíneo. Esto demuestra la extrema sensibilidad del caudal al radio arterial y las consecuencias hemodinámicas graves de la aterosclerosis.</p>
        </div>
      </section>

    </div><!-- /.container -->
  </main>
</body>
</html>
