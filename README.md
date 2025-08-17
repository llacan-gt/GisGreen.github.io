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
    }

    header {
      background: linear-gradient(to right, #0077b6, #00b4d8);
      color: white;
      padding: 20px;
      text-align: center;
    }

    section {
      padding: 40px 20px;
    }

    h2 {
      text-align: center;
      margin-bottom: 20px;
      color: #0077b6;
    }

    .cards {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
      margin-top: 20px;
    }

    .card {
      background: white;
      border-radius: 12px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
      padding: 20px;
      text-align: center;
      transition: transform 0.2s;
    }

    .card:hover {
      transform: scale(1.05);
    }

    .card h3 {
      margin-top: 0;
      color: #023e8a;
    }

    .card a {
      text-decoration: none;
      color: #0077b6;
      font-weight: bold;
      display: inline-block;
      margin-top: 10px;
    }

    footer {
      background-color: #023e8a;
      color: white;
      text-align: center;
      padding: 10px;
      margin-top: 20px;
    }
  </style>
</head>
<body>
  <header>
    <h1>Geoanálisis - Luis Lacán</h1>
    <p>Explora ejemplos prácticos en distintas plataformas de análisis geoespacial</p>
  </header>

  <!-- Google Earth Engine -->
  <section>
    <h2>Google Earth Engine</h2>
    <div class="cards">
      <div class="card">
        <h3>Ejemplo 1</h3>
        <p>Clasificación de coberturas con Random Forest.</p>
        <a href="https://code.earthengine.google.com/c7c033c19f9598ccc9ed6a1a0112955a" target="_blank">Abrir en Earth Engine</a>
      </div>
      <div class="card">
        <h3>Ejemplo 2</h3>
        <p>Procesamiento temporal de imágenes satelitales.</p>
      </div>
    </div>
  </section>

  <!-- Google Colab -->
  <section>
    <h2>Google Colab</h2>
    <div class="cards">
      <div class="card">
        <h3>Ejemplo 1</h3>
        <p>Análisis de índices espectrales en Python.</p>
      </div>
      <div class="card">
        <h3>Ejemplo 2</h3>
        <p>Procesamiento de imágenes satelitales en Python.</p>
      </div>
    </div>
  </section>

  <!-- QGIS -->
  <section>
    <h2>QGIS</h2>
    <div class="cards">
      <div class="card">
        <h3>Ejemplo 1</h3>
        <p>Generación de mapas temáticos.</p>
      </div>
      <div class="card">
        <h3>Ejemplo 2</h3>
        <p>Integración de datos raster y vectoriales.</p>
      </div>
    </div>
  </section>

  <footer>
    <p>© 2025 Geoanálisis - Luis Lacán</p>
  </footer>
</body>
</html>
