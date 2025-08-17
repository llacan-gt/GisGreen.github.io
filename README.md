<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>GeoAnalytics - Luis Lacán</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background: #f5f6fa;
      color: #2f3640;
    }
    header {
      background: #273c75;
      color: white;
      padding: 20px;
      text-align: center;
    }
    header h1 {
      margin: 0;
      font-size: 2em;
    }
    nav {
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      background: #192a56;
    }
    nav a {
      color: white;
      padding: 14px 20px;
      text-decoration: none;
      transition: background 0.3s;
    }
    nav a:hover {
      background: #718093;
    }
    section {
      padding: 50px 20px;
      max-width: 1000px;
      margin: auto;
    }
    section h2 {
      text-align: center;
      margin-bottom: 20px;
      font-size: 2em;
      color: #192a56;
    }
    .card-container {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
    }
    .card {
      background: white;
      border-radius: 10px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
      padding: 20px;
      text-align: center;
      transition: transform 0.3s;
    }
    .card:hover {
      transform: translateY(-8px);
    }
    .card h3 {
      margin: 10px 0;
      color: #273c75;
    }
    .card p {
      font-size: 0.95em;
      color: #555;
    }
    footer {
      background: #273c75;
      color: white;
      text-align: center;
      padding: 15px;
      margin-top: 40px;
    }
  </style>
</head>
<body>
  <header>
    <h1>GeoAnalytics - Luis Lacán</h1>
    <p>Explorando datos geoespaciales, Machine Learning y más</p>
  </header>

  <nav>
    <a href="#colab">Google Colab</a>
    <a href="#gee">Google Earth Engine</a>
    <a href="#basedatos">Bases de Datos Espaciales</a>
    <a href="#ingenieria">Ingeniería de Datos</a>
    <a href="#sensores">Sensores Remotos</a>
    <a href="#ml">Machine Learning</a>
    <a href="#dl">Deep Learning</a>
  </nav>

  <section id="colab">
    <h2>Google Colab</h2>
    <div class="card-container">
      <div class="card">
        <h3>Ejemplo 1</h3>
        <p>Notebook de introducción al análisis espacial en Google Colab.</p>
      </div>
      <div class="card">
        <h3>Ejemplo 2</h3>
        <p>Procesamiento de imágenes satelitales en Python.</p>
      </div>
    </div>
  </section>

  <section id="gee">
    <h2>Google Earth Engine</h2>
    <div class="card-container">
      <div class="card">
        <h3>Mapas dinámicos</h3>
        <p>Ejemplo de clasificación supervisada con Sentinel-2.</p>
      </div>
      <div class="card">
        <h3>Visualización</h3>
        <p>Uso de colecciones de imágenes para análisis temporal.</p>
      </div>
    </div>
  </section>

  <section id="basedatos">
    <h2>Bases de Datos Espaciales</h2>
    <div class="card-container">
      <div class="card">
        <h3>PostgreSQL + PostGIS</h3>
        <p>Gestión de datos espaciales en bases de datos relacionales.</p>
      </div>
      <div class="card">
        <h3>Consultas Espaciales</h3>
        <p>Ejemplos de SQL para análisis geoespacial.</p>
      </div>
    </div>
  </section>

  <section id="ingenieria">
    <h2>Ingeniería de Datos</h2>
    <div class="card-container">
      <div class="card">
        <h3>ETL Geoespacial</h3>
        <p>Procesos de extracción, transformación y carga de datos.</p>
      </div>
      <div class="card">
        <h3>Big Data</h3>
        <p>Gestión de datos geográficos a gran escala.</p>
      </div>
    </div>
  </section>

  <section id="sensores">
    <h2>Sensores Remotos</h2>
    <div class="card-container">
      <div class="card">
        <h3>Satélites</h3>
        <p>Uso de Sentinel, Landsat y otros satélites.</p>
      </div>
      <div class="card">
        <h3>Drones</h3>
        <p>Aplicaciones de UAV para monitoreo ambiental.</p>
      </div>
    </div>
  </section>

  <section id="ml">
    <h2>Machine Learning</h2>
    <div class="card-container">
      <div class="card">
        <h3>Clasificación</h3>
        <p>Aplicación de Random Forest en detección de coberturas.</p>
      </div>
      <div class="card">
        <h3>Predicciones</h3>
        <p>Modelos predictivos aplicados a datos geográficos.</p>
      </div>
    </div>
  </section>

  <section id="dl">
    <h2>Deep Learning</h2>
    <div class="card-container">
      <div class="card">
        <h3>Redes Neuronales</h3>
        <p>Aplicación de CNN en imágenes satelitales.</p>
      </div>
      <div class="card">
        <h3>Detección Avanzada</h3>
        <p>Uso de modelos de deep learning en detección de objetos.</p>
      </div>
    </div>
  </section>

  <footer>
    <p>© 2025 Luis Lacán - GeoAnalytics</p>
  </footer>
</body>
</html>
