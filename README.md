<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>GeoAnalytics - Luis Lacán</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: #111;
      color: #f5f6fa;
    }
    header {
      background: #000;
      color: #00aaff;
      padding: 20px;
      text-align: center;
      font-size: 1.8em;
    }
    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      gap: 15px;
      padding: 20px;
    }
    .card {
      position: relative;
      overflow: hidden;
      border-radius: 10px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.5);
      cursor: pointer;
      transition: transform 0.3s ease;
    }
    .card:hover {
      transform: scale(1.03);
    }
    .card img {
      width: 100%;
      height: 250px;
      object-fit: cover;
      display: block;
      filter: brightness(70%);
      transition: filter 0.3s ease;
    }
    .card:hover img {
      filter: brightness(50%);
    }
    .overlay {
      position: absolute;
      bottom: 20px;
      left: 20px;
      background: rgba(0,0,0,0.6);
      padding: 10px 15px;
      border-radius: 8px;
    }
    .overlay h3 {
      margin: 0;
      color: #00eaff;
      font-size: 1.2em;
    }
    footer {
      text-align: center;
      padding: 15px;
      background: #000;
      color: #888;
      margin-top: 30px;
    }
  </style>
</head>
<body>

  <header>
    GeoAnalytics - Luis Lacán
  </header>

  <div class="grid">
    <div class="card">
      <img src="https://source.unsplash.com/800x600/?code,python" alt="Google Colab">
      <div class="overlay"><h3>Google Colab</h3></div>
    </div>
    <div class="card">
      <img src="https://source.unsplash.com/800x600/?earth,satellite" alt="Google Earth Engine">
      <div class="overlay"><h3>Google Earth Engine</h3></div>
    </div>
    <div class="card">
      <img src="https://source.unsplash.com/800x600/?database,data" alt="Bases de Datos Espaciales">
      <div class="overlay"><h3>Bases de Datos Espaciales</h3></div>
    </div>
    <div class="card">
      <img src="https://source.unsplash.com/800x600/?technology,data" alt="Ingeniería de Datos">
      <div class="overlay"><h3>Ingeniería de Datos</h3></div>
    </div>
    <div class="card">
      <img src="https://source.unsplash.com/800x600/?drone,aerial" alt="Sensores Remotos">
      <div class="overlay"><h3>Sensores Remotos</h3></div>
    </div>
    <div class="card">
      <img src="https://source.unsplash.com/800x600/?ai,machinelearning" alt="Machine Learning">
      <div class="overlay"><h3>Machine Learning</h3></div>
    </div>
    <div class="card">
      <img src="https://source.unsplash.com/800x600/?deep,neuralnetwork" alt="Deep Learning">
      <div class="overlay"><h3>Deep Learning</h3></div>
    </div>
  </div>

  <footer>
    © 2025 Luis Lacán - GeoAnalytics
  </footer>

</body>
</html>
