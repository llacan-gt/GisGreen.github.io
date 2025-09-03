<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Geoanálisis - Luis Lacán</title>
  <style>
    /* Estilos generales */
    body {
      margin: 0;
      font-family: 'Segoe UI', Aharoni, Geneva, Verdana, sans-serif;
      background: url("https://github.com/llacan-gt/geoimagenes/blob/main/Fondo%20de%20pantalla.png?raw=true") 
                  no-repeat center center fixed;
      background-size: cover;
      color: #f5f5f5;
      line-height: 1.6;
      overflow-x: hidden;
    }
    h1, h2, h3 {
      color: #38bdf8;
      text-align: center;
    }
    a {
      color: #38bdf8;
      text-decoration: none;
      transition: color 0.3s ease;
    }
    a:hover {
      color: #0ea5e9;
    }
    /* Header */
    header {
      background: rgba(15, 23, 42, 0.95);
      padding: 30px;
      text-align: center;
      box-shadow: 0 4px 12px rgba(0,0,0,0.6);
      border-radius: 0 0 20px 20px;
    }
    /* Footer */
    footer {
      text-align: center;
      padding: 20px;
      background: rgba(15, 23, 42, 0.95);
      color: #94a3b8;
      margin-top: 40px;
      border-radius: 20px 20px 0 0;
      box-shadow: 0 -4px 12px rgba(0,0,0,0.6);
    }
    /* Secciones homogéneas */
    section {
      padding: 60px 20px;
      max-width: 1100px;
      margin: 40px auto;
      opacity: 0;
      transform: translateY(30px);
      animation: fadeUp 1s ease forwards;
      background: rgba(30, 41, 59, 0.95);
      border-radius: 15px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.6);
    }
    /* Cards */
    .card-container {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 20px;
      margin-top: 20px;
    }
    .card {
      background: rgba(51, 65, 85, 0.9);
      padding: 20px;
      border-radius: 15px;
      width: 300px;
      text-align: center;
      transition: transform 0.3s ease, background 0.3s ease;
      box-shadow: 0 4px 10px rgba(0,0,0,0.5);
    }
    .card:hover {
      transform: translateY(-8px);
      background: rgba(59, 130, 246, 0.9);
    }
    .card h3 {
      margin-bottom: 15px;
      color: #f8fafc;
    }
    /* Animaciones */
    @keyframes fadeUp {
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }
  </style>
</head>
<body>
  <header>
    <h1>Geoanálisis - Luis Lacán</h1>
    <p>Explorando datos espaciales, teledetección y SIG</p>
  </header>

  <section>
    <h2>Google Colab</h2>
    <p>Ejemplos de procesamiento geoespacial en Python:</p>
    <div class="card-container">
      <div class="card">
        <h3>Ejemplo 1</h3>
        <p>Análisis de datos climáticos en Google Colab.</p>
      </div>
      <div class="card">
        <h3>Ejemplo 2</h3>
        <p>Procesamiento de imágenes satelitales en Python.</p>
      </div>
    </div>
  </section>

  <section>
    <h2>Google Earth Engine</h2>
    <p>Visualizaciones y análisis en la nube:</p>
    <div class="card-container">
      <div class="card">
        <h3>Mapa 1</h3>
        <p>Clasificación de coberturas terrestres.</p>
      </div>
      <div class="card">
        <h3>Mapa 2</h3>
        <p>Series temporales de NDVI.</p>
      </div>
    </div>
  </section>

  <section>
    <h2>Sensores Remotos</h2>
    <p>Ejemplos de teledetección aplicada:</p>
    <div class="card-container">
      <div class="card">
        <h3>Satélite 1</h3>
        <p>Análisis multiespectral.</p>
      </div>
      <div class="card">
        <h3>Satélite 2</h3>
        <p>Estudios de cambio de uso de suelo.</p>
      </div>
    </div>
  </section>

  <footer>
    <p>© 2024 Luis Lacán - Geoanálisis</p>
  </footer>
</body>
</html>
