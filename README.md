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
      background-color: #111;
      color: #f5f5f5;
      line-height: 1.6;
    }

    /* Encabezado */
    header {
      background: #0d1b2a;
      padding: 20px;
      text-align: center;
    }
    header h1 {
      margin: 0;
      color: #00eaff;
      font-size: 2em;
    }
    header p {
      margin: 5px 0 0;
      font-size: 1.1em;
      color: #aaa;
    }

    /* Barra de navegación */
    nav {
      background: #1b263b;
      padding: 12px;
      text-align: center;
    }
    nav a {
      color: #eee;
      margin: 0 15px;
      text-decoration: none;
      font-weight: bold;
      transition: color 0.3s;
    }
    nav a:hover {
      color: #00eaff;
    }

    /* Secciones */
    section {
      padding: 40px 20px;
      max-width: 1100px;
      margin: auto;
    }
    section h2 {
      text-align: center;
      margin-bottom: 20px;
      color: #00eaff;
      font-size: 1.8em;
    }

    /* Tarjetas */
    .cards {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
    }
    .card {
      background: #1e293b;
      padding: 20px;
      border-radius: 10px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.5);
      transition: transform 0.3s ease, background 0.3s;
    }
    .card:hover {
      transform: translateY(-5px);
      background: #243447;
    }
    .card h3 {
      margin: 0 0 10px;
      color: #00eaff;
    }
    .card p {
      color: #ccc;
      font-size: 0.95em;
    }

    /* Footer */
    footer {
      text-align: center;
      padding: 20px;
      background: #0d1b2a;
      color: #888;
      margin-top: 40px;
    }
  </style>
</head>
<body>

  <header>
    <h1>Geoanálisis - Luis Lacán</h1>
    <p>Explorando datos geoespaciales, Machine Learning y más</p>
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

  <section id="colab">
    <h2>Google Colab</h2>
    <div class="cards">
      <div class="card">
        <h3>Ejemplo 1</h3>
        <p>Cuaderno de introducción al análisis espacial en Google Colab.</p>
      </div>
      <div class="card">
        <h3>Ejemplo 2</h3>
        <p>Procesamiento de imágenes satelitales en Python.</p>
      </div>
    </div>
  </section>

  <section id="gee">
    <h2>Google Earth Engine</h2>
    <div class="cards">
      <div class="card">
        <h3>Ejemplo 1</h3>
        <p>Clasificación de coberturas terrestres usando GEE.</p>
      </div>
      <div class="card">
        <h3>Ejemplo 2</h3>
        <p>Monitoreo de cambios forestales con imágenes Landsat.</p>
      </div>
    </div>
  </section>

  <section id="bases">
    <h2>Bases de Datos Espaciales</h2>
    <div class="cards">
      <div class="card">
        <h3>Ejemplo 1</h3>
        <p>Uso de PostGIS para almacenar y consultar datos geoespaciales.</p>
      </div>
      <div class="card">
        <h3>Ejemplo 2</h3>
        <p>Visualización de capas espaciales desde bases de datos.</p>
      </div>
    </div>
  </section>

  <footer>
    © 2025 Luis Lacán - Geoanálisis
  </footer>

</body>
</html>
