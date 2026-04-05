<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Semana 2 - BiofÃ­sica</title>
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
      background: #fff;
      border-radius: 12px;
      box-shadow: 0 4px 16px #e0e7ef;
      padding: 2em 2.5em;
      overflow-x: auto;
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
  <nav>
    <h2>Temario</h2>
    <ul>
      <li><a href="#magnitudes">Magnitudes y unidades</a></li>
      <li><a href="#vectores">Vectores</a></li>
      <li><a href="#tamano-forma">TamaÃ±o y forma</a></li>
      <li><a href="#leyes-escala">Leyes de escala</a></li>
      <li><a href="#ejercicios">Ejercicios resueltos</a></li>
    </ul>
    <hr>
    <h2>Recursos</h2>
    <ul>
      <li><a href="../res/MicrocurrÃ­culo.pdf">MicrocurrÃ­culo</a></li>
      <li><a href="https://drive.google.com/drive/folders/1-8WeZK28iaaEToQVGgGCnHxfx8AhXX3f?usp=sharing">Fundamentos fÃ­sicos de los fenÃ³menos biolÃ³gicos</a></li>
    </ul>
    <hr>
    <h2>Autores</h2>
    <ul>
      <li><a href="https://www.researchgate.net/profile/Hoover-Pantoja-Sanchez">Hoover Pantoja-SÃ¡nchez</a></li>
      <li><a href="https://www.researchgate.net/profile/Marco-Giraldo">Marco A. Giraldo</a></li>
    </ul>
    <a href="../" style="font-size:1em; color:#1a365d; text-decoration:underline;">&#8592; Volver al cronograma</a>
  </nav>
  <main>
    <div class="container">
      <h1 class="titulo-principal">Semana 2 (Jueves Ago 14)</h1>
      <!-- =============== GENERALIDADES =============== -->
      <section id="generalidades">
        <h2 class="subtitulo">Generalidades de la biofÃ­sica</h2>
        <div class="texto">
          <p class="parrafo">Aunque los procesos biolÃ³gicos son bastante complejos, al final, se encuentran gobernados por las mismas leyes fÃ­sicas que gobiernan sistemas mÃ¡s simples. En otras palabras los fenÃ³menos fÃ­sicos se convierten en la base sobre la cual se estructura la realidad en la que habitan los organismos biolÃ³gicos. Por lo tanto, entender la relaciÃ³n entre los procesos biolÃ³gicos y los fenÃ³menos fÃ­sicos subyacentes, es un paso crucial para aproximarse a la ecologÃ­a. Para comprender esta relaciÃ³n, se requiere interiorizar conceptos que permitan a la fÃ­sica y la biologÃ­a "hablar un mismo lenguaje". Al final, este rol lo cumple el lenguaje matemÃ¡tico. <strong>En esta sesiÃ³n discutiremos conceptos bÃ¡sicos o fundamentales que permitirÃ¡n adentrarse en temas fÃ­sicos dentro de un contexto ecolÃ³gico.</strong></p>
          <a href="https://drive.google.com/file/d/1LXqpWhVRihNQVxRNapYJI4FAxwwwvBCk/view?usp=sharing" target="_blank" style="display:block;margin:1em 0;font-weight:bold;color:#2563eb;">ðŸŽ§ Escucha el podcast: FÃ­sica y vida: conceptos bÃ¡sicos y la ley de escala</a>
        </div>
      </section>
      <!-- =============== MAGNITUDES =============== -->
      <section id="magnitudes">
        <h2 class="subtitulo">Magnitudes fÃ­sicas, anÃ¡lisis dimensional y sistemas de unidades</h2>
        <div class="definicion">
          <strong>Magnitud fÃ­sica:</strong> cualquier propiedad de un objeto o fenÃ³meno que puede ser expresada numÃ©ricamente, como la distancia, el tiempo, la masa o la temperatura. La <em>cantidad</em> se refiere a la medida de una magnitud fÃ­sica expresada en un sistema de unidades especÃ­fico (metros, segundos, gramos, Â°C).
        </div>
        <p class="parrafo">Se reconocen <strong>cuatro cantidades fundamentales</strong>: la longitud (\(L\)) con dimensiÃ³n \([L]\), la masa (\(M\)) cuya dimensiÃ³n es \([M]\), el tiempo (\(t\)) cuya dimensiÃ³n es \([T]\) y la carga elÃ©ctrica (\(C\)) cuya dimensiÃ³n es \([C]\). Desde aquÃ­ expresaremos la dimensiÃ³n de una cantidad fÃ­sica encerrÃ¡ndola entre corchetes. Por ejemplo, si \(T\) es una temperatura, su dimensiÃ³n se expresarÃ­a \([T]\).</p>
        <p class="parrafo">Cualquier otra cantidad fÃ­sica se expresa a partir de las cantidades fundamentales. Por ejemplo el Ã¡rea (\(A\)) con dimensiÃ³n \([A] = L^2\), o la densidad (\(\rho\)) con dimensiÃ³n \([\rho] = ML^{-3}\).</p>
        <div class="nota">
          <strong>Nota:</strong> El anÃ¡lisis dimensional es una herramienta poderosa para verificar la consistencia de ecuaciones fÃ­sicas. Si las dimensiones no coinciden a ambos lados de una ecuaciÃ³n, la ecuaciÃ³n es necesariamente incorrecta.
        </div>
        <p class="parrafo">Existen 3 sistemas de unidades para expresar las cantidades fÃ­sicas de manera coherente: El <strong>Sistema Internacional (SI)</strong>, el <strong>Sistema Gaussiano</strong> y el <strong>Sistema InglÃ©s (SU)</strong>. Los factores de conversiÃ³n, entre los sistemas de unidades SI y gaussiano, estÃ¡n dados por \(1\,\text{m} = 10^{2}\,\text{cm}\) y \(1\,\text{kg} = 10^{3}\,\text{g}\). El sistema de unidades SU no es comÃºn en contextos cientÃ­ficos. En este sistema las cantidades fundamentales son la fuerza con dimensiÃ³n \(F\), la longitud con dimensiÃ³n \(L\) y el tiempo con dimensiÃ³n \(T\) y sus unidades patrÃ³n son, respectivamente, la libra (lb), el pie (p) y el segundo (s).</p>
        <figure style="text-align:center; margin:2em 0;">
          <a href="res/unidades.png" target="_blank">
            <img src="res/unidades.png" alt="Unidades fÃ­sicas" style="max-width:300px; width:100%; border-radius:10px; box-shadow:0 2px 8px #e0e7ef;">
          </a>
          <figcaption style="color:#2563eb; font-size:1em; margin-top:0.5em;">Tabla 1: Ejemplo de unidades fÃ­sicas. Las unidades de fuerza que se llaman Newton (N), a las de trabajo y energÃ­a Julio (J), potencia Vatio (W) y presiÃ³n Pascal (Pa)</figcaption>
        </figure>
        <figure style="text-align:center; margin:2em 0;">
          <a href="res/multiplos.png" target="_blank">
            <img src="res/multiplos.png" alt="MÃºltiplos y submÃºltiplos" style="max-width:300px; width:100%; border-radius:10px; box-shadow:0 2px 8px #e0e7ef;">
          </a>
          <figcaption style="color:#2563eb; font-size:1em; margin-top:0.5em;">Tabla 2: MÃºltiplos y submÃºltiplos de las unidades del SI</figcaption>
        </figure>
        <div class="ejemplo">
          <strong>Ejemplo &mdash; AnÃ¡lisis dimensional en biomecÃ¡nica:</strong><br>
          Considere la ecuaciÃ³n de la velocidad terminal de una semilla cayendo en el aire:
          \[ v = \sqrt{\frac{2\,m\,g}{\rho\,A\,C_d}} \]
          Verifiquemos las dimensiones del lado derecho. El numerador tiene dimensiones \([m \cdot g] = M \cdot LT^{-2} = MLT^{-2}\). El denominador tiene \([\rho \cdot A \cdot C_d] = ML^{-3} \cdot L^2 \cdot 1 = ML^{-1}\) (pues \(C_d\) es adimensional). Entonces:
          \[ \left[\frac{2mg}{\rho A C_d}\right] = \frac{MLT^{-2}}{ML^{-1}} = L^2 T^{-2} \]
          La raÃ­z cuadrada da \([v] = LT^{-1}\), que corresponde a una velocidad. âœ“ La ecuaciÃ³n es dimensionalmente consistente.
        </div>
        <div style="display: flex; justify-content: center; align-items: center; gap: 2em; margin: 2em 0;">
          <div class="video-frame">
            <iframe src="https://www.youtube.com/embed/eBML4oHcUXQ?si=TByBOrhgT31Rt7YL" title="Importancia del anÃ¡lisis dimensional" allowfullscreen></iframe>
            <figcaption style="color:#2563eb; font-size:1em; margin-top:0.5em;">Video 1. No seas un pend#$%#$%: la importancia del anÃ¡lisis dimensional para hablar de fÃ­sica</figcaption>
          </div>
          <div class="video-frame">
            <iframe src="https://www.youtube.com/embed/87pGTT68izY?si=R4-DMAYCatFUFrnG" title="Video adicional" allowfullscreen></iframe>
            <figcaption style="color:#2563eb; font-size:1em; margin-top:0.5em;">Video 2. Por quÃ© es tan peligroso ver estas pendej"#$$"#$</figcaption>
          </div>
        </div>
      </section>
      <!-- =============== VECTORES =============== -->
      <section id="vectores">
        <h2 class="subtitulo">RepresentaciÃ³n espacial y vectores</h2>
        <p class="parrafo">Para poder representar los fenÃ³menos fÃ­sicos reales, las cantidades fÃ­sicas necesitan incluir la direcciÃ³n en la que se presenta la propiedad. Un aviÃ³n, por ejemplo, se desplaza con una velocidad que tiene una direcciÃ³n especÃ­fica. Para incluir la direcciÃ³n como una propiedad de la cantidad, la fÃ­sica diferencia entre cantidades escalares o vectoriales.</p>
        <div class="definicion">
          <strong>Cantidad escalar:</strong> cualquier propiedad de un objeto o fenÃ³meno que puede ser expresada numÃ©ricamente con un solo valor, como el Ã¡rea (\(A\)), el tiempo (\(t\)), la masa (\(m\)) o la temperatura (\(T\)).
        </div>
        <div class="definicion">
          <strong>Cantidad vectorial:</strong> son las que requieren aÃ±adir una direcciÃ³n ademÃ¡s de su magnitud, como la velocidad (\(\vec{v}\)), la aceleraciÃ³n (\(\vec{a}\)), la velocidad angular (\(\vec{\omega}\)), la aceleraciÃ³n angular (\(\vec{\alpha}\)), el momento lineal (\(\vec{p}\)), la fuerza (\(\vec{F}\)), el torque (\(\vec{\tau}\)) y el momento angular (\(\vec{L}\)).
        </div>
        <p class="parrafo">Los vectores se pueden representar mediante la suma de sus proyecciones rectangulares (Figura 1). AsÃ­, los vectores tienen una magnitud (\(|\vec{r}|\)) y una direcciÃ³n (\(\text{dir}(\vec{r})\)). Para sumar dos o mÃ¡s vectores, se requiere sumar sus direcciones y su magnitud (Figura 2).</p>
        <p class="parrafo">Una propiedad fÃ­sica, como la velocidad, se puede representar a partir de vectores (Figura 3). En este caso, la velocidad se representa como el cambio &mdash; de aquÃ­ en adelante representado por la letra delta mayÃºscula \(\Delta\) &mdash; de la posiciÃ³n o desplazamiento (\(\Delta\vec{r}\)), en relaciÃ³n al cambio del tiempo (\(\Delta t\)) &mdash; como podemos ver, en este caso el tiempo lo definimos como un escalar y no un vector, porque el tiempo no tiene una direcciÃ³n. El desplazamiento, en este ejemplo, tiene una magnitud (\(|\Delta\vec{r}|\)) y una direcciÃ³n (\(\text{dir}(\Delta\vec{r})\)). A la magnitud de la velocidad, la llamamos rapidez y la podemos expresar en el sistema internacional como m/s.</p>
        <div class="nota">
          <strong>Nota:</strong> En notaciÃ³n vectorial, la velocidad se expresa como:
          \[ \vec{v} = \frac{\Delta\vec{r}}{\Delta t} \]
          donde \(\Delta\vec{r}\) es el desplazamiento y \(\Delta t\) es el intervalo de tiempo.
        </div>
        <figure style="text-align:center; margin:2em 0;">
          <a href="res/vector.jpeg" target="_blank">
            <img src="res/vector.jpeg" alt="Vectores" style="max-width:300px; width:100%; border-radius:10px; box-shadow:0 2px 8px #e0e7ef;">
          </a>
          <figcaption style="color:#2563eb; font-size:1em; margin-top:0.5em;">Figura 1: Componentes rectangulares de un vector. El vector \(\vec{a}\) se expresa como la suma de sus componentes rectangulares \(\vec{a} = \vec{a}_x + \vec{a}_y + \vec{a}_z\).</figcaption>
        </figure>
        <figure style="text-align:center; margin:2em 0;">
          <a href="res/opVectores.jpg" target="_blank">
            <img src="res/opVectores.jpg" alt="Ejemplo de vector" style="max-width:300px; width:100%; border-radius:10px; box-shadow:0 2px 8px #e0e7ef;">
          </a>
          <figcaption style="color:#2563eb; font-size:1em; margin-top:0.5em;">Figura 2: Suma de vectores.</figcaption>
        </figure>
        <figure style="text-align:center; margin:2em 0;">
          <a href="res/aplicaciÃ³n de vectores a la fÃ­sica.png" target="_blank">
            <img src="res/aplicaciÃ³n de vectores a la fÃ­sica.png" alt="AplicaciÃ³n de vectores a la fÃ­sica" style="max-width:300px; width:100%; border-radius:10px; box-shadow:0 2px 8px #e0e7ef;">
          </a>
          <figcaption style="color:#2563eb; font-size:1em; margin-top:0.5em;">Figura 3: AplicaciÃ³n de vectores a la fÃ­sica.</figcaption>
        </figure>
      </section>
      <!-- =============== TAMAÃ‘O Y FORMA =============== -->
      <section id="tamano-forma">
        <h2 class="subtitulo">TamaÃ±o y forma</h2>
        <p class="parrafo">Una propiedad fÃ­sica que es muy importante en los procesos biolÃ³gicos es el tamaÃ±o y la forma. La enorme diversidad de formas y tamaÃ±os en los seres vivos, determinan la estructura, funciÃ³n y supervivencia de un organismo, ya que estÃ¡n Ã­ntimamente afectados por fenÃ³menos fÃ­sicos que veremos mÃ¡s adelante, como: la gravedad, la difusiÃ³n, el transporte de calor, las propiedades elÃ¡sticas de los materiales, la dinÃ¡mica del movimiento o la tensiÃ³n superficial.</p>
        <ul>
          <li><strong>No ExtrapolaciÃ³n Simple:</strong> No es posible simplemente extrapolar las funciones vitales de un organismo si sus dimensiones cambian, ya que su configuraciÃ³n corporal, metabolismo, reproducciÃ³n y otras funciones vitales se modifican profundamente con el tamaÃ±o.</li>
          <li><strong>Forma y TamaÃ±o Interrelacionados:</strong> La forma es, con frecuencia, una funciÃ³n del tamaÃ±o. Por ejemplo, las patas de una ardilla y una vaca no pueden tener la misma estructura debido a sus masas distintas. Un exoesqueleto es eficaz para animales pequeÃ±os, pero inviable para los grandes, que necesitan un endoesqueleto. La difusiÃ³n directa de oxÃ­geno es suficiente para una ameba, pero organismos grandes y complejos requieren un sistema circulatorio.</li>
          <li><strong>Discontinuidades Evolutivas:</strong> Hay formas que son posibles para un tamaÃ±o determinado, pero inviables para otros, lo que ha llevado a discontinuidades en el diseÃ±o de los organismos, forzÃ¡ndolos a cambiar evolutivamente forma y tamaÃ±o de manera conjunta para ser viables.</li>
          <li><strong>EvoluciÃ³n del TamaÃ±o:</strong> HistÃ³ricamente, los organismos grandes aparecieron tardÃ­amente. Se observa una tendencia al aumento en las dimensiones de los seres vivos mÃ¡s grandes a lo largo de la historia. Este crecimiento en volumen se logra aumentando el nÃºmero y la variedad de cÃ©lulas, no el tamaÃ±o individual de estas. El aumento de tamaÃ±o exige, y a la vez posibilita, una mayor complejidad y especializaciÃ³n celular.</li>
          <li><strong>Ventajas y Desventajas del TamaÃ±o:</strong> Ser grande puede ofrecer ventajas competitivas (ej. Ã¡rboles altos para captar luz solar), pero tambiÃ©n inconvenientes en entornos cambiantes, ya que requiere un consumo continuo de grandes cantidades de recursos. Los organismos mÃ¡s pequeÃ±os (microorganismos, artrÃ³podos, mamÃ­feros primitivos) han demostrado mayor supervivencia en extinciones masivas.</li>
          <li><strong>LÃ­mites de TamaÃ±o:</strong> Existe un lÃ­mite inferior (tamaÃ±o de molÃ©culas complejas, virus, micoplasmas, que requieren interacciones de muchas molÃ©culas para la autonomÃ­a) y un lÃ­mite superior. El animal terrestre mÃ¡s pesado conocido fue el Baluchitherium (~30 toneladas), mientras que la ballena azul supera las 100 toneladas, beneficiÃ¡ndose de la sustentaciÃ³n en el agua. Las secuoyas gigantes pueden superar las 10 veces la masa de una ballena azul, pero gran parte es tejido muerto. La diferencia de masa entre un micoplasma y una ballena azul abarca 21 Ã³rdenes de magnitud.</li>
        </ul>
        <div style="display: flex; justify-content: center; align-items: center; gap: 2em; margin: 2em 0;">
          <div class="video-frame">
            <iframe src="https://www.youtube.com/embed/vB68awp37Us?si=Sjpu2C-L1CjYcoxw" title="ComparaciÃ³n de tamaÃ±o" allowfullscreen></iframe>
            <figcaption style="color:#2563eb; font-size:1em; margin-top:0.5em;">Video 3. ComparaciÃ³n del tamaÃ±o y forma entre organismos</figcaption>
          </div>
        </div>
      </section>
      <!-- =============== LEYES DE ESCALA =============== -->
      <section id="leyes-escala">
        <h2 class="subtitulo">Leyes de escala</h2>
        <p class="parrafo">Las leyes de escala, o relaciones de escala, se definen como la expresiÃ³n de los cambios funcionales y estructurales que tienen lugar como consecuencia de los cambios de tamaÃ±o (cambios de escala) en los organismos. Aunque se suele pensar que al cambiar la escala de un sistema se mantienen las proporciones entre sus partes, esto no es asÃ­, incluso en sistemas sencillos, como una cuerda que eventualmente se romperÃ¡ por su propio peso si aumenta de tamaÃ±o manteniendo sus proporciones. Los seres vivos deben ajustar su organizaciÃ³n interna si su tamaÃ±o aumenta o disminuye para seguir siendo viables, lo que ha llevado a discontinuidades evolutivas en el diseÃ±o de los organismos.</p>
        <p class="parrafo">Se distinguen dos tipos principales de relaciones de escala:</p>
        <!-- IsomÃ©tricas -->
        <h3 class="subtitulo2">Relaciones isomÃ©tricas o semejanza geomÃ©trica</h3>
        <div class="definicion">
          <strong>Ley de escala isomÃ©trica:</strong> un cuerpo es isomÃ©trico a otro si mantiene las mismas proporciones al cambiar de tamaÃ±o. Si las dimensiones lineales de un cuerpo aumentan en un factor \(k\), las relaciones entre todas sus dimensiones lineales se mantienen constantes.
        </div>
        <p class="parrafo">Relaciones fundamentales:</p>
        <ul>
          <li>La longitud (\(L\)) escala linealmente: \(L \propto k\).</li>
          <li>La superficie (\(S\)) escala con el cuadrado de la longitud:
            \[ S \propto L^2 \propto k^2 \]
          </li>
          <li>El volumen (\(V\)) escala con el cubo de la longitud:
            \[ V \propto L^3 \propto k^3 \]
          </li>
          <li>Si la densidad del organismo es constante (aproximadamente la del agua para los animales), la masa (\(M\)) tambiÃ©n escala con el cubo de la longitud: \(M \propto L^3\).</li>
          <li>De esto se deduce que la superficie es proporcional al volumen (o masa) elevado a la potencia de 2/3:
            \[ S \propto V^{2/3} \quad\text{o}\quad S \propto M^{2/3} \]
          </li>
        </ul>
        <p class="parrafo"><strong>Ejemplos en seres vivos:</strong></p>
        <ul>
          <li><strong>Humanos:</strong> La longitud de los brazos es proporcional a la altura total para mayores de 7 aÃ±os, con una pendiente de 1 en un grÃ¡fico logarÃ­tmico, indicando isometrÃ­a. En edades mÃ¡s tempranas, esta relaciÃ³n se rompe, reflejando cambios en la forma corporal.</li>
          <li><strong>Fuerza muscular:</strong> La fuerza muscular es proporcional a la secciÃ³n transversal de los mÃºsculos (una superficie). Para organismos isomÃ©tricos:
            \[ F_{\text{musc}} \propto M^{2/3} \]
            lo cual se verifica con los rÃ©cords mundiales de halterofilia en funciÃ³n de la masa corporal de los atletas.</li>
          <li><strong>Longitud de los miembros:</strong> En animales isomÃ©tricos, la longitud de los miembros (o segmentos) es proporcional a \(M^{1/3}\), como se observa en segmentos de patas de cucarachas.</li>
          <li><strong>Mohos del fango:</strong> Son organismos diminutos que mantienen las mismas proporciones independientemente de su tamaÃ±o, comportÃ¡ndose isomÃ©tricamente, lo que sugiere que las cargas que soportan no son significativas.</li>
        </ul>
        <!-- AlomÃ©tricas -->
        <h3 class="subtitulo2">Relaciones de escala alomÃ©tricas</h3>
        <div class="definicion">
          <strong>Ley alomÃ©trica:</strong> las relaciones alomÃ©tricas son expresiones que relacionan parÃ¡metros caracterÃ­sticos de los organismos con un exponente diferente al de la semejanza geomÃ©trica. Se expresan generalmente como:
          \[ y = y_0 \, x^a \]
          donde \(y\) es un parÃ¡metro, \(x\) suele ser la masa corporal (\(M\)), \(y_0\) es una constante que depende de la especie o grupo, y \(a\) es el exponente alomÃ©trico.
        </div>
        <ul>
          <li><strong>RepresentaciÃ³n grÃ¡fica:</strong> Al igual que las isomÃ©tricas, se representan como lÃ­neas rectas en diagramas logarÃ­tmicos, donde la pendiente de la recta es el exponente \(a\).</li>
          <li><strong>Significado y relevancia:</strong> Son de interÃ©s si el exponente \(a\) es constante para un rango amplio de masas o un grupo grande de organismos, o si las discontinuidades en \(a\) revelan cambios cualitativos en la organizaciÃ³n del ser vivo. Su interpretaciÃ³n ayuda a comprender la influencia de las leyes fÃ­sicas y del entorno en la organizaciÃ³n biolÃ³gica.</li>
        </ul>
        <p class="parrafo"><strong>Valores de los exponentes y ejemplos:</strong></p>
        <ul>
          <li><strong>Exponente negativo (\(a < 0\)):</strong> El parÃ¡metro disminuye con la masa corporal. Ejemplo: el ritmo cardÃ­aco de un animal (\(a \approx -0.25\)):
            \[ f_c \propto M^{-0.25} \]
            La frecuencia respiratoria (\(M^{-0.26}\)) y la tasa metabÃ³lica especÃ­fica (\(M^{-0.25}\)) tambiÃ©n disminuyen con la masa. El coste energÃ©tico por unidad de masa y distancia en la locomociÃ³n terrestre escala como \(M^{-0.33}\).</li>
          <li><strong>Exponente cero (\(a = 0\)):</strong> El parÃ¡metro no depende de la masa. Ejemplos: la masa de hemoglobina por unidad de volumen de sangre, o el tamaÃ±o de la mayorÃ­a de las cÃ©lulas. La presiÃ³n arterial y la velocidad de la sangre en la aorta tambiÃ©n muestran exponentes cercanos a 0.</li>
          <li><strong>Exponente positivo y menor que uno (\(0 < a < 1\)):</strong> Aumenta con la masa, pero a un ritmo menor que proporcional.
            <ul>
              <li>Superficie corporal: \(S \propto M^{0.67}\).</li>
              <li><strong>Ritmo metabÃ³lico (Ley de Kleiber):</strong> La tasa metabÃ³lica en reposo (\(P_B\)) escala como:
                \[ P_B \propto M^{0.75} \]
                Esta es una ley fundamental en biologÃ­a, cuya universalidad sugiere principios bÃ¡sicos comunes a todos los seres vivos.</li>
              <li>Masa del cerebro: Escala como \(M^{0.67}\) en mamÃ­feros, similar a la superficie corporal. Aunque la constante de proporcionalidad varÃ­a entre grupos (humanos vs. monos, reptiles), el exponente es universal, sugiriendo mecanismos comunes para adaptar el tamaÃ±o del cerebro a la escala corporal.</li>
              <li>Tasa metabÃ³lica mÃ¡xima: \(P_{\text{mÃ¡x}} \propto M^{0.81}\) o \(M^{0.85}\).</li>
              <li>Tiempos biolÃ³gicos: El "tiempo fisiolÃ³gico" (gestaciÃ³n, vida media, etc.) suele ser proporcional a \(M^{0.25}\). La vida media en mamÃ­feros y aves escala con exponentes cercanos a:
                \[ t_{\text{vida}} \propto M^{0.20} \]
                y \(M^{0.19}\) respectivamente.</li>
            </ul>
          </li>
          <li><strong>Exponente uno (\(a = 1\)):</strong> El parÃ¡metro es estrictamente proporcional a la masa. Ejemplos: la masa del corazÃ³n o el volumen de la sangre en mamÃ­feros, que son una fracciÃ³n fija de la masa corporal.</li>
          <li><strong>Exponente mayor que uno (\(a > 1\)):</strong> El parÃ¡metro aumenta mÃ¡s rÃ¡pidamente que la masa. Ejemplo: el peso del esqueleto en mamÃ­feros:
            \[ M_{\text{esq}} \approx 0.09\,M^{1.09} \]
            En aves, es \(M^{1.07}\).</li>
        </ul>
        <div class="ejemplo">
          <strong>Ejemplo &mdash; CÃ¡lculo alomÃ©trico: tasa metabÃ³lica del cerebro</strong><br>
          La masa del cerebro en mamÃ­feros escala como \(M_{\text{cerebro}} = c \, M^{0.67}\). Si un ratÃ³n de \(M = 20\,\text{g}\) tiene un cerebro de \(0.4\,\text{g}\), podemos estimar la constante: \(c = 0.4 / (20)^{0.67} = 0.4 / 7.37 \approx 0.054\). Para un humano de \(M = 70\,\text{kg} = 70{,}000\,\text{g}\):
          \[ M_{\text{cerebro}} = 0.054 \times (70{,}000)^{0.67} \approx 0.054 \times 1{,}695 \approx 91.5\,\text{g} \]
          El valor real es ~1400&thinsp;g, muy superior al predicho, lo cual refleja que los humanos poseen un cerebro desproporcionadamente grande para su masa corporal (alto <em>cociente de encefalizaciÃ³n</em>).
        </div>
        <div class="nota">
          <strong>Nota:</strong> Las leyes alomÃ©tricas son aproximaciones estadÃ­sticas obtenidas a partir de regresiones logarÃ­tmicas sobre grandes conjuntos de datos. Especies individuales pueden desviarse significativamente de la lÃ­nea de tendencia general. Estas desviaciones son, en sÃ­ mismas, fuente de informaciÃ³n biolÃ³gica valiosa.
        </div>
      </section>
      <!-- =============== EJERCICIOS RESUELTOS =============== -->
      <section id="ejercicios">
        <h2 class="subtitulo">Ejercicios resueltos</h2>
        <!-- Ejercicio 1 -->
        <div class="ejemplo">
          <strong>Ejercicio 1: AnÃ¡lisis dimensional &mdash; Fuerza de arrastre</strong><br><br>
          <strong>Enunciado:</strong> La fuerza de arrastre que experimenta un organismo moviÃ©ndose a travÃ©s de un fluido se expresa como:
          \[ F_d = \tfrac{1}{2}\,C_d\,\rho\,A\,v^2 \]
          donde \(C_d\) es el coeficiente de arrastre (adimensional), \(\rho\) es la densidad del fluido, \(A\) es el Ã¡rea de referencia y \(v\) es la velocidad del organismo. Verificar que la ecuaciÃ³n es dimensionalmente consistente.<br><br>
          <strong>SoluciÃ³n:</strong><br>
          Identificamos las dimensiones de cada cantidad:
          <ul>
            <li>\([C_d] = 1\) (adimensional)</li>
            <li>\([\rho] = M L^{-3}\)</li>
            <li>\([A] = L^2\)</li>
            <li>\([v^2] = L^2 T^{-2}\)</li>
          </ul>
          Calculamos las dimensiones del lado derecho:
          \[ \left[\tfrac{1}{2}\,C_d\,\rho\,A\,v^2\right] = 1 \cdot (ML^{-3}) \cdot L^2 \cdot (L^2 T^{-2}) \]
          \[ = M \cdot L^{-3+2+2} \cdot T^{-2} = M L T^{-2} \]
          La dimensiÃ³n del lado izquierdo es la de una fuerza:
          \[ [F_d] = M L T^{-2} \]
          Ambos lados coinciden. âœ“ <strong>La ecuaciÃ³n es dimensionalmente consistente.</strong>
        </div>
        <!-- Ejercicio 2 -->
        <div class="ejemplo">
          <strong>Ejercicio 2: Ley de Kleiber &mdash; PredicciÃ³n de la tasa metabÃ³lica</strong><br><br>
          <strong>Enunciado:</strong> Un ratÃ³n de \(20\,\text{g}\) tiene una tasa metabÃ³lica en reposo de \(P_B = 0.2\,\text{W}\). Usando la ley de Kleiber, \(P_B \propto M^{0.75}\), predecir la tasa metabÃ³lica en reposo de un caballo de \(500\,\text{kg}\).<br><br>
          <strong>SoluciÃ³n:</strong><br>
          La ley de Kleiber establece:
          \[ P_B = P_0 \, M^{0.75} \]
          <strong>Paso 1:</strong> Determinamos la constante \(P_0\) usando los datos del ratÃ³n (\(M_r = 0.020\,\text{kg}\)):
          \[ P_0 = \frac{P_{B,r}}{M_r^{0.75}} = \frac{0.2\,\text{W}}{(0.020)^{0.75}} \]
          Calculamos \((0.020)^{0.75}\):
          \[ (0.020)^{0.75} = e^{0.75 \ln(0.020)} = e^{0.75 \times (-3.912)} = e^{-2.934} \approx 0.0531 \]
          \[ P_0 = \frac{0.2}{0.0531} \approx 3.77\,\text{W/kg}^{0.75} \]
          <strong>Paso 2:</strong> Calculamos la tasa metabÃ³lica del caballo (\(M_c = 500\,\text{kg}\)):
          \[ P_{B,c} = 3.77 \times (500)^{0.75} \]
          Calculamos \((500)^{0.75}\):
          \[ (500)^{0.75} = e^{0.75 \ln(500)} = e^{0.75 \times 6.215} = e^{4.661} \approx 105.7 \]
          \[ P_{B,c} = 3.77 \times 105.7 \approx 398\,\text{W} \]
          <strong>Resultado:</strong> La tasa metabÃ³lica en reposo predicha para el caballo es aproximadamente \(\boxed{398\,\text{W}}\), es decir unas \(1990\) veces mayor que la del ratÃ³n, a pesar de que su masa es \(25{,}000\) veces mayor. Esto ilustra la economÃ­a metabÃ³lica de los organismos grandes: la tasa metabÃ³lica por unidad de masa <em>disminuye</em> al aumentar el tamaÃ±o.
        </div>
        <div class="nota">
          <strong>Nota:</strong> La ley de Kleiber (\(P_B \propto M^{0.75}\)) se cumple notablemente bien a lo largo de mÃ¡s de 20 Ã³rdenes de magnitud en masa, desde bacterias hasta ballenas. El exponente \(0.75\) en lugar de \(0.67\) (que se esperarÃ­a por argumentos puramente geomÃ©tricos de superficie/volumen) sigue siendo objeto de investigaciÃ³n activa y se ha relacionado con la estructura fractal de las redes de distribuciÃ³n de recursos en los organismos.
        </div>
      </section>
    </div>
  </main>
</body>
</html>
