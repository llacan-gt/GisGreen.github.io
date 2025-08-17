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
      background-color: #f4f4f9;
      color: #333;
      line-height: 1.6;
    }

    header {
      background: #2c3e50;
      color: white;
      padding: 20px 0;
      text-align: center;
    }

    header h1 {
      margin: 0;
      font-size: 2.5rem;
    }

    nav {
      margin-top: 10px;
    }

    nav a {
      margin: 0 15px;
      text-decoration: none;
      color: white;
      font-weight: bold;
    }

    section {
      padding: 40px 20px;
      max-width: 1200px;
      margin: auto;
    }

    h2 {
      color: #2c3e50;
      margin-bottom: 20px;
    }

    .cards {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
    }

    .card {
      background: white;
      padding: 20px;
      border-radius: 12px;
      box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
      text-align: center;
      transition: transform 0.3s, box-shadow 0.3s;
    }

    .card:hover {
      transform: translateY(-5px);
      box-shadow: 0 8px 12px rgba(0, 0, 0, 0.2);
    }

    .card img {
      width: 100%;
      border-radius: 12px;
      margin-bottom: 15px;
    }

    /* Redes sociales */
    .social {
      text-align: center;
      margin-top: 40px;
    }

    .social a {
      margin: 0 15px;
      display: inline-block;
    }

    .social img {
      width: 40px;
      height: 40px;
      transition: transform 0.3s;
    }

    .social img:hover {
      transform: scale(1.2);
    }

    footer {
      text-align: center;
      padding: 20px;
      background: #2c3e50;
      color: white;
      margin-top: 40px;
    }
  </style>
</head>
<body>
  <!-- Encabezado -->
  <header>
    <h1>Geoanálisis - Luis Lacán</h1>
    <nav>
      <a href="#colab">Google Colab</a>
      <a href="#gee">Google Earth Engine</a>
      <a href="#procesamiento">Procesamiento</a>
      <a href="#redes">Redes Sociales</a>
    </nav>
  </header>

  <!-- Sección Google Colab -->
  <section id="colab">
    <h2>Ejemplos en Google Colab</h2>
    <div class="cards">
      <!-- Ejemplo 1 -->
      <div class="card">
        <a href="https://colab.research.google.com/" target="_blank">
          <img src="https://miro.medium.com/v2/resize:fit:1400/format:webp/1*Hq-3Zm7pC1RrO2D96aDqTg.png" alt="Google Colab">
        </a>
        <h3>Ejemplo 1</h3>
        <p>Ejecutar notebooks en Google Colab.</p>
      </div>
    </div>
  </section>

  <!-- Sección Google Earth Engine -->
  <section id="gee">
    <h2>Ejemplos en Google Earth Engine</h2>
    <div class="cards">
      <!-- Ejemplo 1 modificado con tu link -->
      <div class="card">
        <a href="https://code.earthengine.google.com/c7c033c19f9598ccc9ed6a1a0112955a" target="_blank">
          <img src="https://earthengine.google.com/static/images/earth-engine-logo.png" alt="Google Earth Engine">
        </a>
        <h3>Ejemplo 1</h3>
        <p>Ejemplo de clasificación supervisada en Google Earth Engine.</p>
      </div>

      <!-- Ejemplo 2 -->
      <div class="card">
        <a href="https://developers.google.com/earth-engine/tutorials" target="_blank">
          <img src="https://storage.googleapis.com/gweb-cloudblog-publish/original_images/DataCloud_1.png" alt="Procesamiento">
        </a>
        <h3>Ejemplo 2</h3>
        <p>Procesamiento de imágenes satelitales en Google Earth Engine.</p>
      </div>
    </div>
  </section>

  <!-- Sección Procesamiento -->
  <section id="procesamiento">
    <h2>Procesamiento de Imágenes</h2>
    <div class="cards">
      <div class="card">
        <img src="https://miro.medium.com/v2/resize:fit:1200/format:webp/1*4VHK3uKxR271GGBqBPdZiQ.png" alt="Procesamiento en Python">
        <h3>Python</h3>
        <p>Procesamiento de imágenes satelitales en Python usando librerías como Rasterio, Numpy y Scikit-Learn.</p>
      </div>
      <div class="card">
        <img src="https://qgis.org/en/_static/logo.png" alt="QGIS">
        <h3>QGIS</h3>
        <p>Análisis espacial con QGIS para la gestión de datos geográficos.</p>
      </div>
    </div>
  </section>

  <!-- Redes Sociales -->
  <section id="redes">
    <h2>Conéctate conmigo</h2>
    <div class="social">
      <a href="https://www.linkedin.com/in/luis-joel-lacan-lacan-5a959b56" target="_blank">
        <img src="https://cdn-icons-png.flaticon.com/512/174/174857.png" alt="LinkedIn">
      </a>
      <a href="https://github.com/" target="_blank">
        <img src="https://cdn-icons-png.flaticon.com/512/25/25231.png" alt="GitHub">
      </a>
      <a href="https://twitter.com/" target="_blank">
        <img src="https://cdn-icons-png.flaticon.com/512/733/733579.png" alt="Twitter">
      </a>
    </div>
  </section>

  <!-- Footer -->
  <footer>
    <p>&copy; 2025 Luis Lacán - Geoanálisis</p>
  </footer>
</body>
</html>

