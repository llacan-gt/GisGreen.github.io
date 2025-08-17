<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Geoanálisis - Luis Lacán</title>
  <style>
    /* Estilos generales */
    body {
      margin: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background-color: #0a0a0a;
      color: #f5f5f5;
      line-height: 1.6;
      overflow-x: hidden;
    }
    header {
      background: linear-gradient(270deg, #0d1b2a, #1b263b, #0d1b2a);
      background-size: 600% 600%;
      animation: gradientShift 12s ease infinite;
      padding: 40px 20px;
      text-align: center;
    }
    @keyframes gradientShift {
      0% {background-position: 0% 50%;}
      50% {background-position: 100% 50%;}
      100% {background-position: 0% 50%;}
    }
    header h1 {
      margin: 0;
      color: #00eaff;
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
    nav {
      background: #1b263b;
      padding: 12px;
      text-align: center;
      position: sticky;
      top: 0;
      z-index: 10;
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
    section {
      padding: 60px 20px;
      max-width: 1100px;
      margin: auto;
      opacity: 0;
      transform: translateY(30px);
      animation: fadeUp 1s ease forwards;
    }
    section:nth-child(even) {
      background: #111827;
    }
    @keyframes fadeUp {
      to { opacity: 1; transform: translateY(0); }
    }
    section h2 {
      text-align: center;
      margin-bottom: 30px;
      color: #00eaff;
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
      padding: 25px;
      border-radius: 12px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.6);
      transition: transform 0.4s ease, box-shadow 0.4s, background 0.4s;
      cursor: pointer;
      position: relative;
      overflow: hidden;
    }
    .card::before {
      content: "";
      position: absolute;
      top: -50%;
      left: -50%;
      width: 200%;
      height: 200%;
      background: radial-gradient(circle, rgba(0,234,255,0.1), transparent 60%);
      transform: rotate(25deg);
      transition: opacity 0.4s;
      opacity: 0;
    }
    .card:hover::before { opacity: 1; }
    .card:hover {
      transform: translateY(-8px) scale(1.02);
      background: #243447;
      box-shadow: 0 6px 20px rgba(0,234,255,0.4);
    }
    .card h3 { margin: 0 0 10px; color: #00eaff; }
    .card p { color: #ccc; font-size: 0.95em; }
    .card img {
      width: 100%;
      height: 160px;
      object-fit: cover;
      border-radius: 10px;
      margin-bottom: 10px;
      border: 1px solid rgba(0,234,255,0.2);
    }
    /* Estilos redes sociales */
    .socials a {
      margin: 0 10px;
      color: #00bcd4;
      font-size: 28px;
      text-decoration: none;
      transition: all 0.3s ease-in-out;
    }
    .socials a:hover {
      color: #fff;
      text-shadow: 0 0 10px #00eaff, 0 0 20px #00eaff, 0 0 30px #00eaff;
      transform: scale(1.2);
    }
  </style>

  <!-- Font Awesome actualizado -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css"
        integrity="sha512-SnH5WK+bZxgPHs44uWIX+LLJAJ9zUqFqUuZ2ZCkxzgv2Fne5DE5FCDJ/NzNw2K6JqqPiR+jYwIVlY5PjaVXrUg=="
        crossorigin="anonymous" referrerpolicy="no-referrer" />
</head>
<body>

<header>
  <h1>GisGreen</h1>
  <p>"Bienvenido al fascinante mundo del análisis de información geoespacial! Aquí encontrarás notebooks y recursos de aprendizaje sobre ArcGIS Online, Google Colab, Google Earth Engine y bases de datos espaciales."</p>
</header>

<nav>
  <a href="#colab">Google Colab</a>
  <a href="#gee">Google Earth Engine</a>
  <a href="#bases">Bases de Datos Espaciales</a>
  <a href="#datos">Ingeniería de Datos</a>
  <a href="#sensores">Sensores Remotos</a>
  <a href="#ml">Machine Learning</a>
  <a href="#dl">Deep Learning</a>
</nav>

<!-- Secciones (mantengo igual tu estructura) -->
<section id="colab"> ... </section>
<section id="gee"> ... </section>
<section id="bases"> ... </section>
<section id="datos"> ... </section>
<section id="sensores"> ... </section>
<section id="ml"> ... </section>
<section id="dl"> ... </section>

<!-- Footer -->
<footer style="background:#1e1e1e; color:#00bcd4; padding:40px 20px; text-align:center;">
  <h2 style="margin-bottom:10px;">Luis Lacán</h2>
  <p style="margin-bottom:25px; color:#ccc;">Especialista en Geomática | Análisis Espacial | Innovación con IA</p>
  
  <div class="socials" style="margin-bottom:25px;">
    <a href="https://linkedin.com/in/luis-joel-lacan-lacan-5a959b56" target="_blank"><i class="fab fa-linkedin"></i></a>
    <a href="https://github.com" target="_blank"><i class="fab fa-github"></i></a>
    <a href="https://twitter.com" target="_blank"><i class="fab fa-twitter"></i></a>
    <a href="mailto:luis.lacan@gmail.com"><i class="fas fa-envelope"></i></a>
    <a href="https://wa.me/50231767274" target="_blank"><i class="fab fa-whatsapp"></i></a>
  </div>

  <p style="color:#888; font-size:14px;">© 2025 Luis Lacán - GisGreen - luis.lacan@gmail.com</p>
</footer>

</body>
</html>
