<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Geoanálisis - Luis Lacán</title>
  <style>
    html, body {
      margin: 0;
      padding: 0;
      width: 100%;
      height: 100%;
      font-family: 'Segoe UI', Aharoni, Geneva, Verdana, sans-serif;
      background: url('https://github.com/llacan-gt/geoimagenes/blob/main/Fondo_4.png?raw=true') no-repeat center center fixed;
      background-size: cover;
      color: #ffffff;
      line-height: 1.6;
      overflow-x: hidden;
    }
    header {
      background: linear-gradient(270deg, #0d1b2a, #1b263b, #0d1b2a);
      background-size: 600% 600%;
      animation: gradientShift 12s ease infinite;
      padding: 40px 20px;
      text-align: center;
      width: 100%;
      position: relative;
    }
    @keyframes gradientShift {
      0% {background-position: 0% 50%;}
      50% {background-position: 100% 50%;}
      100% {background-position: 0% 50%;}
    }
    header h1 {
      margin: 0;
      color: #ffffff;
      font-size: 2.5em;
      animation: glow 2s ease-in-out infinite alternate;
    }
    @keyframes glow {
      from { text-shadow: 0 0 5px #00eaff, 0 0 10px #00eaff; }
      to { text-shadow: 0 0 20px #00eaff, 0 0 40px #00eaff; }
    }
    header p {
      margin: 10px 0 0;
      font-size: 1.2em;
      color: #aaa;
    }
    /* Contador de visitas en posición estratégica */
    .visitor-counter {
      position: fixed;
      top: 20px;
      right: 20px;
      padding: 10px 15px;
      background: rgba(30, 41, 59, 0.9);
      border-radius: 10px;
      box-shadow: 0 4px 15px rgba(0, 0, 0, 0.6);
      z-index: 1000;
      backdrop-filter: blur(5px);
      border: 1px solid rgba(0, 234, 255, 0.3);
      text-align: center;
      transition: transform 0.3s, box-shadow 0.3s;
    }
    .visitor-counter:hover {
      transform: translateY(-3px);
      box-shadow: 0 6px 20px rgba(0, 234, 255, 0.4);
    }
    .visitor-counter h3 {
      margin: 0 0 5px;
      color: #00eaff;
      font-size: 0.9em;
    }
    .counter-number {
      font-size: 1.5em;
      font-weight: bold;
      color: #ffffff;
      text-shadow: 0 0 10px rgba(0, 234, 255, 0.7);
    }
    .counter-label {
      font-size: 0.7em;
      color: #aaa;
      margin-top: 3px;
    }
    
  nav {
      background: #1b263b;
      padding: 12px;
      text-align: center;
      position: sticky;
      top: 0;
      z-index: 10;
      width: 100%;
    }
    nav a {
      color: #eee;
      margin: 0 15px;
      text-decoration: none;
      font-weight: bold;
      transition: color 0.3s, transform 0.3s;
      display: inline-block;
    }
    nav a:hover {
      color: #00eaff;
      transform: scale(1.1);
    }
    
   /* Estilos para el carrusel */
    .carousel-container {
      width: 100%;
      max-width: 1200px;
      margin: 40px auto;
      position: relative;
      overflow: hidden;
      border-radius: 15px;
      box-shadow: 0 6px 20px rgba(0, 0, 0, 0.8);
    }
    .carousel {
      display: flex;
      transition: transform 0.5s ease;
      height: 450px;
    }
    .carousel-item {
      min-width: 100%;
      height: 100%;
      position: relative;
    }
    .carousel-item img {
      width: 100%;
      height: 100%;
      object-fit: cover;
    }
    .carousel-caption {
      position: absolute;
      bottom: 0;
      left: 0;
      right: 0;
      background: rgba(13, 27, 42, 0.85);
      padding: 20px;
      text-align: center;
    }
    .carousel-caption h3 {
      margin: 0 0 10px;
      color: #00eaff;
    }
    .carousel-caption p {
      margin: 0;
      color: #eee;
    }
    .carousel-control {
      position: absolute;
      top: 50%;
      transform: translateY(-50%);
      background: rgba(0, 234, 255, 0.3);
      color: white;
      border: none;
      width: 50px;
      height: 50px;
      border-radius: 50%;
      font-size: 24px;
      cursor: pointer;
      z-index: 10;
      transition: background 0.3s;
    }
    .carousel-control:hover {
      background: rgba(0, 234, 255, 0.7);
    }
    .carousel-control.prev {
      left: 15px;
    }
    .carousel-control.next {
      right: 15px;
    }
    .carousel-indicators {
      position: absolute;
      bottom: 15px;
      left: 50%;
      transform: translateX(-50%);
      display: flex;
      gap: 10px;
    }
    .carousel-indicator {
      width: 12px;
      height: 12px;
      border-radius: 50%;
      background: rgba(255, 255, 255, 0.5);
      cursor: pointer;
      transition: background 0.3s;
    }
    .carousel-indicator.active {
      background: #00eaff;
    }
    
  section {
      padding: 60px 20px;
      max-width: 1100px;
      margin: 40px auto;
      opacity: 0;
      transform: translateY(30px);
      animation: fadeUp 1s ease forwards;
      background: rgba(30, 41, 59, 0.85);
      border-radius: 15px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.6);
      width: 90%;
    }
    @keyframes fadeUp {
      to { opacity: 1; transform: translateY(0); }
    }
    section h2 {
      text-align: center;
      margin-bottom: 30px;
      color: #ffffff;
      font-size: 2em;
      position: relative;
    }
    section h2::after {
      content: "";
      display: block;
      width: 80px;
      height: 3px;
      background: #00eaff;
      margin: 10px auto 0;
      border-radius: 3px;
      animation: pulse 2s infinite;
    }
    @keyframes pulse {
      0%, 100% { transform: scaleX(1); opacity: 0.7; }
      50% { transform: scaleX(1.5); opacity: 1; }
    }
    .cards {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
      gap: 25px;
    }
    .card {
      background: #1e293b;
      padding: 20px;
      border-radius: 12px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.7);
      transition: transform 0.4s ease, box-shadow 0.4s, background 0.4s;
      cursor: pointer;
      position: relative;
      overflow: hidden;
      text-decoration: none;
      color: inherit;
      display: block;
    }
    .card::before {
      content: "";
      position: absolute;
      top: -50%;
      left: -50%;
      width: 200%;
      height: 200%;
      background: radial-gradient(circle, rgba(0,234,255,0.70), transparent 70%);
      transform: rotate(25deg);
      transition: opacity 0.4s;
      opacity: 0;
    }
    .card:hover::before { opacity: 1; }
    .card:hover {
      transform: translateY(-8px) scale(1.02);
      background: #243447;
      box-shadow: 0 6px 20px rgba(0,234,255,0.7);
    }
    .card h3 { margin: 10px 0; color: #ffffff; }
    .card p { color: #ccc; font-size: 0.95em; }
    .card img {
      width: 100%;
      height: 160px;
      object-fit: cover;
      border-radius: 10px;
      margin-bottom: 10px;
      border: 1px solid rgba(0,234,255,0.7);
    }
    .social-icons {
      display: flex;
      justify-content: center;
      gap: 25px;
      margin: 30px 0;
    }
    .social-icons a {
      color: #ffffff;
      font-size: 30px;
      transition: all 0.3s;
    }
    .social-icons a:hover {
      color: #ffffff;
      transform: scale(1.2);
    }
    footer {
      background: #1e1e1e;
      color: #ffffff;
      padding: 40px 20px;
      text-align: center;
      width: 100%;
    }
  </style>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
</head>
<body>

<!-- Contador de visitas en posición estratégica -->
<div class="visitor-counter">
  <h3>VISITAS</h3>
  <div class="counter-number" id="visitCount">0</div>
  <div class="counter-label">Total</div>
</div>

<header>
  <h1>GisGreen</h1>
  <p>"Bienvenido al fascinante mundo del análisis de información geoespacial! Aquí encontrarás notebooks y recursos de aprendizaje sobre ArcGIS Online, Google Colab, Google Earth Engine y bases de datos espaciales."</p>
</header>

<nav>
  <a href="#carrusel">Inicio</a>
  <a href="#colab">Google Colab</a>
  <a href="#gee">Google Earth Engine</a>
  <a href="#bases">Sensores Remotos</a>
  <a href="#datos">Bases de Datos</a>
  <a href="#sensores">Ingenieria</a>
  <a href="#ml">Machine Learning</a>
  <a href="#dl">Deep Learning</a>
</nav>

<!-- Carrusel de imágenes -->
<div class="carousel-container" id="carrusel">
  <div class="carousel">
    <div class="carousel-item">
      <img src="https://images.unsplash.com/photo-1542744095-fcf48d80b0fd?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1200&q=80" alt="Análisis Geoespacial">
      <div class="carousel-caption">
        <h3>Análisis Geoespacial</h3>
        <p>Exploración de técnicas avanzadas para el análisis de información geográfica</p>
      </div>
    </div>
    <div class="carousel-item">
      <img src="https://images.unsplash.com/photo-1589652717521-10c0d092dea9?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1200&q=80" alt="Google Earth Engine">
      <div class="carousel-caption">
        <h3>Google Earth Engine</h3>
        <p>Procesamiento de imágenes satelitales a escala planetaria</p>
      </div>
    </div>
    <div class="carousel-item">
      <img src="https://images.unsplash.com/photo-1544197150-b99a580bb7a8?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1200&q=80" alt="Machine Learning">
      <div class="carousel-caption">
        <h3>Machine Learning Geoespacial</h3>
        <p>Aplicación de algoritmos de IA para el análisis de datos espaciales</p>
      </div>
    </div>
  </div>
  <button class="carousel-control prev" onclick="moveCarousel(-1)">&#10094;</button>
  <button class="carousel-control next" onclick="moveCarousel(1)">&#10095;</button>
  <div class="carousel-indicators">
    <span class="carousel-indicator active" onclick="goToSlide(0)"></span>
    <span class="carousel-indicator" onclick="goToSlide(1)"></span>
    <span class="carousel-indicator" onclick="goToSlide(2)"></span>
  </div>
</div>

<!-- Google Colab -->
<section id="colab">
  <h2>Google Colab</h2>
  <div class="cards">
    <a href="https://nbviewer.org/github/llacan-gt/GisGreen.github.io/blob/main/Mapas_interactivos_con_python.ipynb" target="_blank" class="card">
      <img src="https://github.com/llacan-gt/GisGreen.github.io/blob/main/imagenes/Maps.png?raw=true">
      <h3>Visualización de Mapas Interactivos</h3>
      <p>Exploración de mapas interactivos creados con Python en Google Colab.</p>
    </a>
    <a href="https://github.com/llacan-gt/notebooks.geoespacial/blob/main/Geometry_operations.ipynb" target="_blank" class="card">
      <img src="https://github.com/llacan-gt/geoimagenes/blob/main/Gemini_Generated_Image_rjawemrjawemrjaw.png?raw=true" alt="Python Notebook">
      <h3>datos Vectoriales</h3>
      <p>Manejo y Visualizacion de datos Vectoriales.</p>
    </a>
    <a href="https://colab.research.google.com/tu_otro_notebook.ipynb" target="_blank" class="card">
      <img src="https://images-assets.nasa.gov/image/iss073e0509720/iss073e0509720~medium.jpg" alt="Clasificación RF">
      <h3>Ejemplo 3</h3>
      <p>Clasificación de imágenes satelitales con Random Forest.</p>
    </a>
  </div>
</section>

<!-- Google Earth Engine -->
<section id="gee">
  <h2>Google Earth Engine</h2>
  <div class="cards">
    <a href="https://code.earthengine.google.com/c7c033c19f9598ccc9ed6a1a0112955a" target="_blank" class="card">
      <img src="https://github.com/llacan-gt/geoimagenes/blob/main/GEE_2.jpg?raw=true" alt="Coberturas">
      <h3>Ejemplo 1</h3>
      <p>Clasificación de coberturas terrestres usando GEE.</p>
    </a>
    <a href="https://developers.google.com/earth-engine/datasets" target="_blank" class="card">
      <img src="https://github.com/llacan-gt/geoimagenes/blob/main/Imagenes%20Sentinel.jpg?raw=true" alt="Monitoreo forestal">
      <h3>Ejemplo 2</h3>
      <p>Monitoreo de cambios forestales con Landsat/Sentinel.</p>
    </a>
  </div>
</section>

<!-- Sensores Remotos -->
<section id="bases">
  <h2>Sensores Remotos</h2>
  <div class="cards">
    <a href="https://postgis.net/" target="_blank" class="card">
      <img src="https://github.com/llacan-gt/geoimagenes/blob/main/academiacopernicus.jpg?raw=true" alt="PostGIS">
      <h3>Programa COOPERNICUS</h3>
      <p>Acceso al programa de Coopernicus para la obtencion de imagenes satelitales.</p>
    </a>
    <a href="https://www.microsoft.com/en-us/sql-server" target="_blank" class="card">
      <img src="https://www.sqldatapartners.com/wp-content/uploads/2019/01/sql-server-logo.png" alt="SQL Server">
      <h3>Programa LANDSAT</h3>
      <p>Acceso al programa NASA/USGS para la obtencion de imagenes satelitales.</p>
    </a>
  </div>
</section>

<!-- Base de Datos Espaciales -->
<section id="datos">
  <h2>Bases de Datos Espaciales</h2>
  <div class="cards">
    <a href="#" target="_blank" class="card">
      <img src="https://images.unsplash.com/photo-1551288049-bebda4e38f71" alt="Automatización">
      <h3>Ejemplo 1</h3>
      <p>Consultas SQL y ArcGis Pro.</p>
    </a>
    <a href="#" target="_blank" class="card">
      <img src="https://images.unsplash.com/photo-1460925895917-afdab827c52f" alt="Optimización">
      <h3>Ejemplo 2</h3>
      <p>Consultas en PostGis.</p>
    </a>
  </div>
</section>

<!-- Ingenieria de Datos -->
<section id="sensores">
  <h2>Ingenieria de Datos</h2>
  <div class="cards">
    <a href="#" target="_blank" class="card">
      <img src="https://images.unsplash.com/photo-1502134249126-9f3755a50d78" alt="Multiespectral">
      <h3>Ejemplo 1</h3>
      <p>Programa COOPERNICUS.</p>
    </a>
    <a href="#" target="_blank" class="card">
      <img src="https://images.unsplash.com/photo-1500382017468-9049fed747ef" alt="SAR">
      <h3>Ejemplo 2</h3>
      <p>Programa LANDSAT.</p>
    </a>
  </div>
</section>

<!-- Machine Learning -->
<section id="ml">
  <h2>Machine Learning</h2>
  <div class="cards">
    <a href="#" target="_blank" class="card">
      <img src="https://images.unsplash.com/photo-1504868584819-f8e8b4b6d7e3" alt="ML">
      <h3>Ejemplo 1</h3>
      <p>Predicción de uso del suelo con modelos supervisados.</p>
    </a>
    <a href="#" target="_blank" class="card">
      <img src="https://images.unsplash.com/photo-1485827404703-89b55fcc595e" alt="Clasificación">
      <h3>Ejemplo 2</h3>
      <p>Clasificación automática de coberturas terrestres.</p>
    </a>
  </div>
</section>

<!-- Deep Learning -->
<section id="dl">
  <h2>Deep Learning</h2>
  <div class="cards">
    <a href="#" target="_blank" class="card">
      <img src="https://images.unsplash.com/photo-1620712943543-bcc4688e7485" alt="CNN">
      <h3>Ejemplo 1</h3>
      <p>Redes convolucionales aplicadas a imágenes satelitales.</p>
    </a>
    <a href="#" target="_blank" class="card">
      <img src="https://images.unsplash.com/photo-1629909613654-28e377c0b8e0" alt="YOLO">
      <h3>Ejemplo 2</h3>
      <p>Detección de objetos geoespaciales con YOLO.</p>
    </a>
  </div>
</section>

<footer>
  <h2>Luis Lacán</h2>
  <p>Geomática | Especialista SIG | Innovación con IA</p>
  <div class="social-icons">
    <a href="https://linkedin.com/in/luis-joel-lacan-lacan-5a959b56" target="_blank"><i class="fab fa-linkedin"></i></a>
    <a href="https://github.com" target="_blank"><i class="fab fa-github"></i></a>
    <a href="mailto:luis.lacan@gmail.com"><i class="fas fa-envelope"></i></a>
    <a href="https://wa.me/50231767274" target="_blank"><i class="fab fa-whatsapp"></i></a>
  </div>
  <p style="color:#888; font-size:14px;">© 2025 Luis Lacán - GisGreen - luis.lacan@gmail.com</p>
</footer>

<script>
  // Carrusel de imágenes
  let currentSlide = 0;
  const slides = document.querySelectorAll('.carousel-item');
  const indicators = document.querySelectorAll('.carousel-indicator');
  const carousel = document.querySelector('.carousel');
  
  function showSlide(n) {
    currentSlide = (n + slides.length) % slides.length;
    carousel.style.transform = `translateX(-${currentSlide * 100}%)`;
    
    // Actualizar indicadores
    indicators.forEach((indicator, index) => {
      indicator.classList.toggle('active', index === currentSlide);
    });
  }
  
  function moveCarousel(n) {
    showSlide(currentSlide + n);
  }
  
  function goToSlide(n) {
    showSlide(n);
  }
  
  // Auto-avance del carrusel
  setInterval(() => {
    moveCarousel(1);
  }, 5000);
  
  // Contador de visitas mejorado
  function updateVisitorCounter() {
    // Intentar obtener el contador del localStorage
    let count = localStorage.getItem('visitorCount');
    
    if (count) {
      count = parseInt(count) + 1;
    } else {
      count = 1;
    }
    
    // Guardar el nuevo contador
    localStorage.setItem('visitorCount', count);
    
    // Mostrar el contador con animación
    const counterElement = document.getElementById('visitCount');
    counterElement.textContent = count;
    
    // Pequeña animación al actualizar
    counterElement.style.transform = 'scale(1.2)';
    setTimeout(() => {
      counterElement.style.transform = 'scale(1)';
    }, 300);
  }
  
  // Inicializar
  document.addEventListener('DOMContentLoaded', function() {
    updateVisitorCounter();
  });
</script>
</body>
</html>
