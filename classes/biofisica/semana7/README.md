<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Semana 7 - Termodinámica</title>
  <script>
    window.MathJax = {
      tex: { inlineMath: [['\\(','\\)']], displayMath: [['\\[','\\]']] }
    };
  </script>
  <script src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-chtml.js" async></script>
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
      overflow-x: hidden;
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
      padding: 10px;
      border: 1px solid #bfc9d9;
      text-align: center;
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
        position: static;
        width: 100%;
        height: auto;
        min-height: auto;
      }
      main {
        margin-left: 0;
        padding: 1.5em;
      }
      .container {
        padding: 1em;
      }
      .videos-dos {
        flex-direction: column;
        align-items: center;
      }
      .video-frame {
        width: 100%;
      }
      .img-contenido {
        max-width: 100%;
      }
    }
  </style>
</head>
<body>
  <!-- NAV LATERAL -->
  <nav>
    <h2>Temario</h2>
    <ul>
      <li><a href="#temperatura">Temperatura y calor</a></li>
      <li><a href="#principios">Leyes de la termodinámica</a></li>
      <li><a href="#transiciones">Transiciones de fase</a></li>
      <li><a href="#biologicos">Sistemas biológicos</a></li>
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

  <!-- CONTENIDO PRINCIPAL -->
  <main>
    <div class="container">

      <h1 class="titulo-principal">Semana 7 (Jueves Oct 30)</h1>
      <h1 class="titulo-principal">Termodinámica</h1>
      <p class="parrafo" style="text-align:center; color:#555;">Biofísica &mdash; Termodinámica y sistemas biológicos</p>

      <!-- ==================== INTRODUCCIÓN ==================== -->
      <div class="videos-dos">
        <div class="video-frame">
          <iframe width="420" height="240" src="https://www.youtube.com/embed/ZLAoKBVglU8?si=ie_N6MbjElBdsYK0" title="Explicación sencilla y un poco de historia" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
          <div style="color:#2563eb; font-size:0.95em; margin-top:0.5em;">Video 1. Resumen general y un poco de historia.</div>
        </div>
      </div>

      <a href="https://drive.google.com/file/d/1VTUUN-J4ZzfDO-ab1MGtAmoCuag7V1cD/view?usp=sharing" target="_blank" style="display:block;margin:1em 0;font-weight:bold;color:#2563eb;">🎧 Escucha el podcast - Termodinámica y Vida</a>

      <p class="parrafo">La termodinámica se enfoca en sistemas compuestos por elevados números de partículas, átomos o moléculas. Del orden del número de Avogadro, que es aproximadamente \(6.02 \times 10^{23}\).</p>

      <div class="videos-dos">
        <div class="video-frame">
          <iframe width="420" height="240" src="https://www.youtube.com/embed/UoQqglMVW1g?si=AH2hoZ0CVpOx0ld2" title="Número de Avogadro" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
          <div style="color:#2563eb; font-size:0.95em; margin-top:0.5em;">Video 2. ¿De dónde viene el número de Avogadro?</div>
        </div>
      </div>

      <!-- ==================== TEMPERATURA, CALOR Y TRABAJO ==================== -->
      <section id="temperatura">
        <h2 class="subtitulo">Temperatura, Calor y Trabajo</h2>

        <div class="definicion">
          <strong>Temperatura:</strong> Promedio de la energía cinética de las partículas que componen un objeto. Se mide en grados Celsius (°C), grados Fahrenheit (°F) o Kelvin (K). La energía cinética promedio de un gas ideal se relaciona con la temperatura mediante:
          \[\frac{3}{2}k_BT = \frac{1}{2}m\langle v^2\rangle\]
        </div>

        <div class="definicion">
          <strong>Calor:</strong> Transferencia de energía térmica entre sistemas a diferente temperatura. La unidad en el Sistema Internacional es el Julio (J). La cantidad de calor necesaria para cambiar la temperatura de una sustancia está dada por:
          \[Q = mc\Delta T\]
          donde \(m\) es la masa, \(c\) es el calor específico y \(\Delta T\) es el cambio de temperatura.
        </div>

        <div class="definicion">
          <strong>Trabajo termodinámico:</strong> Energía transferida cuando un sistema ejerce una fuerza sobre su entorno. En un proceso termodinámico, el trabajo se relaciona con el calor y la energía interna a través de la primera ley. En una expansión isobárica: \(W = P\Delta V\).
        </div>

        <p class="parrafo">Energía térmica: Suma de la energía de todas las partículas de un objeto. Si un objeto es más grande, tendrá una mayor energía térmica debido a su tamaño. La unidad en el Sistema Internacional para la energía térmica son los Julios (J).</p>

        <div class="nota">
          <strong>Conversión de temperatura:</strong> Para convertir de grados Celsius a Kelvin se usa:
          \[T(K) = T(°C) + 273.15\]
        </div>

        <div class="nota">
          <strong>Expansión térmica:</strong> Cuando un material se calienta, sus dimensiones cambian. Para una expansión lineal:
          \[\Delta L = \alpha L_0 \Delta T\]
          donde \(\alpha\) es el coeficiente de expansión lineal y \(L_0\) la longitud original.
        </div>

        <div class="ejemplo">
          <strong>Ejemplo:</strong> ¿Cuánto calor se necesita para elevar la temperatura de 500 g de agua de 20 °C a 100 °C? (calor específico del agua: \(c = 4.184\) J/g·°C).<br><br>
          <strong>Solución:</strong><br>
          Datos: \(m = 500\) g, \(\Delta T = 100 - 20 = 80\) °C, \(c = 4.184\) J/g·°C.<br>
          \[Q = mc\Delta T = (500)(4.184)(80) = 167{,}360 \text{ J} \approx 167.4 \text{ kJ}\]
          Se necesitan aproximadamente <strong>167.4 kJ</strong> de calor.
        </div>
      </section>

      <!-- ==================== LEYES DE LA TERMODINÁMICA ==================== -->
      <section id="principios">
        <h2 class="subtitulo">Leyes de la termodinámica</h2>

        <h3 class="subtitulo2">Ley cero</h3>
        <p class="parrafo">Aunque se añadió al final, la ley cero sirve como base para las demás. Se refiere al <strong>equilibrio térmico</strong>. Si dos sistemas están en equilibrio térmico con un tercer sistema, significa que los dos primeros están en equilibrio entre sí. Aunque parezca elemental, esta ley permite inferir que si la temperatura medida por un termómetro en el sistema A (\(T_a\)), es igual a la temperatura medida por un termómetro en el sistema B (\(T_b\)), es decir \(T_a = T_b\), esto quiere decir que los sistemas A y B se encuentran en equilibrio.</p>

        <h3 class="subtitulo2">Primera Ley</h3>
        <p class="parrafo">También conocida como ley de la conservación de la energía. La energía no se crea ni se destruye, solo se transforma. De esta ley se infiere que el calor (\(\Delta Q\)) es igual a la energía interna del sistema (\(\Delta U\)) más el trabajo producido (\(\Delta W\)). Esto quiere decir que se puede aprovechar el calor para producir trabajo.</p>

        <div class="definicion">
          <strong>Energía interna:</strong> Es la suma de todas las formas de energía microscópica de un sistema (cinética y potencial de sus partículas). En forma diferencial, la primera ley se escribe:
          \[dU = \delta Q - \delta W\]
          o equivalentemente:
          \[\Delta Q = \Delta U + \Delta W\]
        </div>

        <p class="parrafo"><a href="https://phet.colorado.edu/en/simulations/energy-forms-and-changes" target="_blank" style="font-weight:bold; color:#2563eb;">🔗 Explora la simulación: Energy Forms and Changes (PBS Learning Media)</a></p>

        <h3 class="subtitulo2">Segunda Ley</h3>

        <div class="definicion">
          <strong>Entropía:</strong> Magnitud que mide el desorden o el número de microestados accesibles de un sistema. La definición estadística de Boltzmann es:
          \[S = k_B \ln \Omega\]
          donde \(k_B\) es la constante de Boltzmann y \(\Omega\) es el número de microestados. La definición clásica (Clausius) para un proceso reversible es:
          \[\Delta S = \frac{Q}{T}\]
        </div>

        <p class="parrafo">La segunda ley, o la ley de la entropía, dice que el calor siempre fluirá desde el objeto con mayor temperatura hacia el objeto con menor temperatura y no en el sentido contrario. Clausius la enunció así: &ldquo;Es imposible que una máquina autónoma sin ayuda de un agente externo transfiera calor de un cuerpo a otro más caliente&rdquo;. De aquí nace el concepto de entropía, una magnitud que mide la relación entre la energía térmica y la temperatura, o la cantidad de energía que no puede ser utilizada para convertirse en trabajo mecánico. Si un sistema reduce la entropía interna, esto produce un aumento de la entropía del entorno. Por esto, la entropía siempre aumenta en el universo.</p>

        <p class="parrafo"><a href="https://phet.colorado.edu/en/simulations/diffusion" target="_blank" style="font-weight:bold; color:#2563eb;">🔗 Explora la simulación: Difusión (PBS Learning Media)</a></p>

        <p class="parrafo">Aunque el concepto de entropía nace en la termodinámica, no se entendía claramente qué movía la entropía siempre hacia adelante, o en otras palabras, por qué existen procesos que no son reversibles. Posteriormente, la mecánica estadística de la teoría cinética del calor de finales del siglo XIX logró explicar este fenómeno a partir de una explicación estadística. La entropía no surge a partir de una fuerza o un fenómeno físico, sino que surge de un proceso de combinatoria de estados. Así, la definición moderna de entropía es la siguiente: una magnitud que mide el número de microestados equivalentes que generan un mismo macroestado de un sistema. En otras palabras, de cuántas formas posibles se pueden organizar los microelementos de un sistema para obtener un estado en el macrosistema. Con esta definición, se puede reescribir la segunda ley como: un sistema evoluciona a su configuración más probable, que es la que se da con más microestados y coincide con la que mayor entropía tiene.</p>

        <div class="nota">
          <strong>Entropía en sistemas biológicos:</strong> Los organismos vivos mantienen un estado de baja entropía interna (alta organización) a costa de aumentar la entropía de su entorno (liberando calor, desechos, etc.). Esto no viola la segunda ley, ya que la entropía total del universo sigue aumentando.
        </div>

        <div class="videos-dos">
          <div class="video-frame">
            <iframe width="420" height="240" src="https://www.youtube.com/embed/ttjM-dMPddY?si=i1kI3lEn99o6VxM" title="Explicación de la entropía" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
            <div style="color:#2563eb; font-size:0.95em; margin-top:0.5em;">Video 3. Explicación de la entropía.</div>
          </div>
        </div>

        <h3 class="subtitulo2">Tercera Ley</h3>
        <p class="parrafo">La tercera ley, o ley del cero absoluto, dice que es imposible bajar la temperatura de cualquier sistema a cero absoluto en un número finito de pasos. Es decir, el cero absoluto es solo posible teóricamente.</p>

        <div class="nota">
          <strong>Cero absoluto:</strong> El cero absoluto corresponde a \(0\,\text{K} = -273.15\,°\text{C}\). A esta temperatura, las partículas tendrían la mínima energía posible (pero no energía nula, debido al principio de incertidumbre de Heisenberg).
        </div>

        <h3 class="subtitulo2">Gases ideales y eficiencia</h3>

        <div class="videos-dos">
          <div class="video-frame">
            <iframe width="420" height="240" src="https://www.youtube.com/embed/92QHLRt1Bv0?si=42oP-E_tfW0PJqj-" title="Gases ideales" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
            <div style="color:#2563eb; font-size:0.95em; margin-top:0.5em;">Video 4. Gases ideales.</div>
          </div>
        </div>

        <p class="parrafo">La ley de los gases ideales relaciona presión, volumen, cantidad de sustancia y temperatura:</p>
        \[PV = nRT\]

        <p class="parrafo">La eficiencia máxima teórica de cualquier motor térmico que opera entre dos temperaturas está dada por el ciclo de Carnot:</p>
        \[\eta = 1 - \frac{T_C}{T_H}\]
        <p class="parrafo">donde \(T_C\) es la temperatura del foco frío y \(T_H\) la del foco caliente (ambas en Kelvin).</p>

        <p class="parrafo"><a href="https://phet.colorado.edu/en/simulations/gas-properties" target="_blank" style="font-weight:bold; color:#2563eb;">🔗 Explora la simulación: Gases ideales y leyes (PHET Learning Media)</a></p>
      </section>

      <!-- ==================== TRANSICIONES DE FASE ==================== -->
      <section id="transiciones">
        <h2 class="subtitulo">Transiciones de fase</h2>

        <p class="parrafo">Las transiciones de fase son cambios en el estado de agregación de la materia. Las principales son:</p>
        <ul style="margin-left:1.2em; line-height:1.7;">
          <li><strong>Fusión</strong> (sólido &rarr; líquido): el material absorbe calor y sus partículas ganan suficiente energía para romper la estructura cristalina.</li>
          <li><strong>Vaporización</strong> (líquido &rarr; gas): las partículas adquieren suficiente energía para escapar de la fase líquida. Puede ocurrir como evaporación (superficie) o ebullición (todo el volumen).</li>
          <li><strong>Sublimación</strong> (sólido &rarr; gas): el material pasa directamente de sólido a gas sin pasar por el estado líquido (ejemplo: hielo seco, CO₂).</li>
          <li><strong>Condensación</strong> (gas &rarr; líquido), <strong>solidificación</strong> (líquido &rarr; sólido) y <strong>deposición</strong> (gas &rarr; sólido) son los procesos inversos.</li>
        </ul>

        <p class="parrafo">Un <strong>diagrama de fases</strong> representa las condiciones de presión y temperatura bajo las cuales coexisten las diferentes fases de una sustancia. El punto triple es la condición en la que las tres fases coexisten en equilibrio, y el punto crítico marca el límite a partir del cual no se distingue entre líquido y gas.</p>

        <div class="definicion">
          <strong>Calor latente:</strong> Durante una transición de fase, la temperatura permanece constante mientras el material absorbe o libera energía. Esta energía se llama calor latente:
          \[Q = mL\]
          donde \(L\) es el calor latente específico. Para el agua:
          <ul style="margin:0.5em 0 0 1.2em;">
            <li>Calor latente de fusión: \(L_f = 334\) J/g</li>
            <li>Calor latente de vaporización: \(L_v = 2{,}260\) J/g</li>
          </ul>
        </div>

        <div class="nota">
          <strong>Transiciones de fase y calor latente:</strong> Durante un cambio de fase (por ejemplo, cuando el hielo se derrite), toda la energía absorbida se utiliza para romper enlaces intermoleculares y no para aumentar la temperatura. Por eso la temperatura permanece constante hasta que todo el material ha cambiado de fase.
        </div>

        <p class="parrafo"><strong>Relevancia biológica:</strong></p>
        <ul style="margin-left:1.2em; line-height:1.7;">
          <li><strong>Termorregulación en organismos marinos:</strong> El alto calor específico del agua ayuda a estabilizar la temperatura corporal de los organismos acuáticos. Los océanos actúan como reguladores térmicos globales.</li>
          <li><strong>Enfriamiento evaporativo:</strong> La evaporación del sudor o del agua en superficies corporales absorbe gran cantidad de calor (\(L_v = 2{,}260\) J/g), proporcionando un mecanismo eficiente de enfriamiento. Muchos animales (incluyendo perros y aves) usan ventilación respiratoria para disipar calor.</li>
        </ul>

        <p class="parrafo"><a href="https://phet.colorado.edu/en/simulations/states-of-matter" target="_blank" style="font-weight:bold; color:#2563eb;">🔗 Explora la simulación: Estados de la materia (PHET Learning Media)</a></p>
      </section>

      <!-- ==================== TERMODINÁMICA EN SISTEMAS BIOLÓGICOS ==================== -->
      <section id="biologicos">
        <h2 class="subtitulo">Termodinámica en sistemas biológicos</h2>

        <p class="parrafo">Los organismos vivos son <strong>sistemas termodinámicos abiertos</strong>: intercambian tanto materia como energía con su entorno. A diferencia de los sistemas aislados, los seres vivos pueden mantener estados de alta organización (baja entropía) importando energía libre del ambiente y exportando entropía en forma de calor y desechos.</p>

        <p class="parrafo">El <strong>metabolismo</strong> es fundamentalmente un proceso termodinámico. Las reacciones metabólicas transforman energía química de los nutrientes en trabajo mecánico, transporte activo, biosíntesis y calor. Todas estas transformaciones obedecen las leyes de la termodinámica.</p>

        <div class="definicion">
          <strong>Energía libre de Gibbs:</strong> La cantidad de energía disponible para realizar trabajo útil en un proceso a presión y temperatura constantes se mide con la energía libre de Gibbs:
          \[\Delta G = \Delta H - T\Delta S\]
          donde \(\Delta H\) es el cambio de entalpía, \(T\) la temperatura absoluta y \(\Delta S\) el cambio de entropía. Si \(\Delta G < 0\), el proceso es espontáneo. Si \(\Delta G > 0\), requiere un aporte de energía.
        </div>

        <p class="parrafo">La molécula central del metabolismo energético es el <strong>ATP</strong> (adenosín trifosfato). La hidrólisis de ATP libera energía que se acopla a procesos celulares esenciales:</p>
        \[\text{ATP} + \text{H}_2\text{O} \rightarrow \text{ADP} + \text{P}_i \quad \Delta G \approx -30.5\,\text{kJ/mol}\]

        <p class="parrafo"><strong>Eficiencia de los motores biológicos vs. Carnot:</strong> Los motores biológicos (como los músculos) operan a temperaturas casi uniformes, por lo que no funcionan como motores térmicos clásicos. Su eficiencia no está limitada por el ciclo de Carnot, ya que convierten directamente energía química en trabajo mecánico. La eficiencia muscular típica es del 20–25%, lejos del 100% pero independiente de la diferencia de temperatura. En contraste, un motor de Carnot operando entre 37 °C (\(310\) K) y 20 °C (\(293\) K) tendría una eficiencia máxima de solo:</p>
        \[\eta_{\text{Carnot}} = 1 - \frac{293}{310} \approx 5.5\%\]
        <p class="parrafo">Esto demuestra que los sistemas biológicos superan ampliamente la eficiencia que tendría un motor térmico operando con las mismas temperaturas, precisamente porque no son motores térmicos.</p>
      </section>

      <!-- ==================== EJERCICIOS RESUELTOS ==================== -->
      <section id="ejercicios">
        <h2 class="subtitulo">Ejercicios resueltos</h2>

        <div class="ejemplo">
          <strong>Ejercicio 1: Calentamiento de agua de mar</strong><br><br>
          ¿Cuánto calor se necesita para calentar 2 kg de agua de mar desde 15 °C hasta 25 °C? El calor específico del agua de mar es \(c \approx 3.93\) kJ/(kg·°C). Luego, ¿cuánto calor adicional se necesita para evaporar toda el agua?<br><br>

          <strong>Parte 1 — Calentamiento:</strong><br>
          Datos: \(m = 2\) kg, \(\Delta T = 25 - 15 = 10\) °C, \(c = 3.93\) kJ/(kg·°C).<br>
          \[Q_1 = mc\Delta T = (2)(3.93)(10) = 78.6 \text{ kJ}\]
          Se necesitan <strong>78.6 kJ</strong> para calentar el agua de mar.<br><br>

          <strong>Parte 2 — Evaporación:</strong><br>
          Para evaporar el agua, primero debemos llevarla desde 25 °C hasta 100 °C y luego suministrar el calor latente de vaporización.<br>
          Calentamiento de 25 °C a 100 °C:<br>
          \[Q_2 = mc\Delta T = (2)(3.93)(75) = 589.5 \text{ kJ}\]
          Evaporación a 100 °C (\(L_v \approx 2{,}260\) kJ/kg para agua):<br>
          \[Q_3 = mL_v = (2)(2{,}260) = 4{,}520 \text{ kJ}\]
          Calor total para evaporar (desde 25 °C):<br>
          \[Q_{\text{total}} = Q_2 + Q_3 = 589.5 + 4{,}520 = 5{,}109.5 \text{ kJ} \approx 5.11 \text{ MJ}\]
          Se necesitan aproximadamente <strong>5.11 MJ</strong> adicionales para evaporar toda el agua de mar (desde 25 °C). Nótese la enorme cantidad de energía que requiere la vaporización comparada con el simple calentamiento.
        </div>

        <div class="ejemplo">
          <strong>Ejercicio 2: Eficiencia de un motor biológico</strong><br><br>
          Un músculo de pez convierte energía química en trabajo mecánico con una eficiencia del 25%. Si necesita producir 50 J de trabajo mecánico:<br>
          a) ¿Cuánta energía química debe consumir?<br>
          b) ¿Qué sucede con el resto de la energía?<br>
          c) Calcula el cambio de entropía si la temperatura corporal del pez es 20 °C.<br><br>

          <strong>a) Energía química consumida:</strong><br>
          La eficiencia se define como \(\eta = \frac{W}{E_{\text{entrada}}}\). Despejando:<br>
          \[E_{\text{entrada}} = \frac{W}{\eta} = \frac{50}{0.25} = 200 \text{ J}\]
          El músculo debe consumir <strong>200 J</strong> de energía química.<br><br>

          <strong>b) Energía restante:</strong><br>
          La energía que no se convierte en trabajo se disipa como calor:<br>
          \[Q = E_{\text{entrada}} - W = 200 - 50 = 150 \text{ J}\]
          <strong>150 J</strong> se disipan como calor al entorno (agua circundante). Esta es la razón por la cual los organismos generan calor durante la actividad muscular.<br><br>

          <strong>c) Cambio de entropía:</strong><br>
          La temperatura corporal del pez es \(T = 20\,°\text{C} = 293.15\) K. El calor disipado genera un aumento de entropía en el entorno:<br>
          \[\Delta S = \frac{Q}{T} = \frac{150}{293.15} \approx 0.512 \text{ J/K}\]
          La entropía del entorno aumenta en aproximadamente <strong>0.512 J/K</strong>. Esto es consistente con la segunda ley: la actividad muscular es un proceso irreversible que incrementa la entropía del universo.
        </div>
      </section>

    </div>
  </main>
</body>
</html>
