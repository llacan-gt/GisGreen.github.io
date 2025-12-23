<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>GisGreen | Geomática & Análisis Ambiental</title>

  <meta name="description" content="Servicios profesionales en geomática, SIG, sensores remotos, análisis ambiental, machine learning y apoyo a investigación científica.">
  <meta name="author" content="Luis Lacán">

  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">

  <style>
    html, body {
      margin: 0;
      padding: 0;
      font-family: 'Segoe UI', Geneva, Verdana, sans-serif;
      background: url('https://github.com/llacan-gt/geoimagenes/blob/main/Fondo_4.png?raw=true') no-repeat center center fixed;
      background-size: cover;
      color: #ffffff;
      line-height: 1.6;
      overflow-x: hidden;
    }

    header {
      background: linear-gradient(270deg, #0d1b2a, #1b263b, #0d1b2a);
      animation: gradientShift 12s ease infinite;
      padding: 50px 20px;
      text-align: center;
    }

    @keyframes gradientShift {
      0% {background-position: 0% 50%;}
      50% {background-position: 100% 50%;}
      100% {background-position: 0% 50%;}
    }

    header h1 {
      font-size: 2.6em;
      margin: 0;
      text-shadow: 0 0 15px #00eaff;
    }

    header p {
      max-width: 900px;
      margin: 15px auto 0;
      color: #ccc;
    }

    nav {
      background: #1b263b;
      padding: 12px;
      text-align: center;
      position: sticky;
      top: 0;
      z-index: 100;
    }

    nav a {
      color: #eee;
      margin: 0 14px;
      text-decoration: none;
      font-weight: bold;
    }

    nav a:hover {
      color: #00eaff;
    }

    section {
      padding: 60px 20px;
      max-width: 1100px;
      margin: 50px auto;
      background: rgba(30, 41, 59, 0.85);
      border-radius: 15px;
      box-shadow: 0 4px 15px rgba(0,0,0,0.6);
    }

    section h2 {
      text-align: center;
      margin-bottom: 30px;
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
      transition: transform 0.3s, box-shadow 0.3s;
    }

    .card:hover {
      transform: translateY(-6px);
      box-shadow: 0 6px 20px rgba(0,234,255,0.6);
    }

    .card img {
      width: 100%;
      height: 160px;
      object-fit: cover;
      border-radius: 10px;
      margin-bottom: 10px;
    }

    footer {
      background: #111;
      text-align: center;
      padding: 40px 20px;
    }

    .social-icons a {
      color: white;
      font-size: 28px;
      margin: 0 15px;
    }
  </style>
</head>

<body>

<header>
  <h1>GisGreen</h1>
  <p>
    Servicios profesionales en <strong>Geomática, SIG, Sensores Remotos, Análisis Ambiental</strong>,
    asistencia en investigación científica y apoyo técnico para trámites del sector ambiental.
  </p>
</header>

<nav>
  <a href="#servicios">Servicios</a>
  <a href="#sobre-mi">Sobre mí</a>
  <a href="#colab">Portafolio</a>
  <a href="#gee">GEE</a>
  <a href="#ml">ML</a>
  <a href="#dl">DL</a>
</nav>

<section id="servicios">
  <h2>Servicios Profesionales</h2>
  <div class="cards">
    <div class="card">
      <h3>🌍 Análisis Geoespacial</h3>
      <p>Mapas temáticos, análisis territorial, planificación y apoyo técnico ambiental.</p>
    </div>
    <div class="card">
      <h3>🛰️ Sensores Remotos</h3>
      <p>Procesamiento Sentinel y Landsat, detección de cambios y monitoreo ambiental.</p>
    </div>
    <div class="card">
      <h3>📊 Asistencia en Investigación</h3>
      <p>Apoyo técnico para tesis, artículos científicos y análisis de datos.</p>
    </div>
    <div class="card">
      <h3>📑 Trámites Ambientales</h3>
      <p>Cartografía y análisis SIG para procesos y documentación ambiental.</p>
    </div>
  </div>
</section>

<section id="sobre-mi">
  <h2>Sobre mí</h2>
  <p style="text-align:center; max-width:850px; margin:auto;">
    Soy <strong>Luis Lacán</strong>, especialista en geomática y análisis geoespacial.
    Tras varios años de experiencia en proyectos SIG, sensores remotos y análisis ambiental,
    decidí emprender ofreciendo servicios técnicos y asesoría especializada para el sector ambiental.
  </p>
</section>

<section id="colab">
  <h2>Portafolio Técnico</h2>
  <div class="cards">
    <div class="card">
      <h3>Google Colab</h3>
      <p>Notebooks de análisis geoespacial y visualización interactiva.</p>
    </div>
    <div class="card">
      <h3>Google Earth Engine</h3>
      <p>Clasificación y monitoreo ambiental con imágenes satelitales.</p>
    </div>
  </div>
</section>

<footer>
  <h2>Luis Lacán</h2>
  <p>Geomática | SIG | Análisis Ambiental</p>

  <div class="social-icons">
    <a href="https://linkedin.com/in/luis-joel-lacan-lacan-5a959b56" target="_blank"><i class="fab fa-linkedin"></i></a>
    <a href="https://github.com/llacan-gt" target="_blank"><i class="fab fa-github"></i></a>
    <a href="mailto:luis.lacan@gmail.com"><i class="fas fa-envelope"></i></a>
    <a href="https://wa.me/50231767274" target="_blank"><i class="fab fa-whatsapp"></i></a>
  </div>

  <p style="font-size:14px;color:#888;">© 2025 GisGreen | Luis Lacán</p>
</footer>

<!-- Botón WhatsApp fijo -->
<a href="https://wa.me/50231767274" target="_blank"
   style="position:fixed;bottom:20px;right:20px;background:#25D366;color:white;
   padding:15px;border-radius:50%;font-size:28px;z-index:1000;">
  <i class="fab fa-whatsapp"></i>
</a>
</body>
</html>
