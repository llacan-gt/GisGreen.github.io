<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Lluis Lacán – GeoAnalytics & Geomática</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background: #111;
      color: #fff;
    }

    .grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      grid-template-rows: auto auto;
    }

    .grid-item {
      position: relative;
      overflow: hidden;
    }

    .grid-item img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      display: block;
      filter: brightness(70%);
      transition: transform 0.5s ease;
    }

    .grid-item:hover img {
      transform: scale(1.1);
      filter: brightness(60%);
    }

    .label {
      position: absolute;
      bottom: 20px;
      left: 20px;
      background: rgba(0,0,0,0.7);
      padding: 10px 15px;
      border-radius: 5px;
      color: cyan;
      font-weight: bold;
      font-size: 1.2rem;
    }

    footer {
      text-align: center;
      background: #222;
      padding: 2rem 1rem;
    }

    footer h2 {
      margin: 0;
      font-size: 2rem;
      color: cyan;
    }

    footer p {
      margin: 0.5rem 0 1.5rem;
      font-size: 1rem;
      color: #aaa;
    }

    .socials {
      display: flex;
      justify-content: center;
      gap: 1.5rem;
      font-size: 2rem;
    }

    .socials a {
      color: cyan;
      text-decoration: none;
      transition: color 0.3s;
    }

    .socials a:hover {
      color: #1abc9c;
    }
  </style>
</head>
<body>
  <div class="grid">
    <div class="grid-item">
      <img src="https://picsum.photos/id/1011/800/600" alt="Spatial Analysis">
      <div class="label">Geomática</div>
    </div>
    <div class="grid-item">
      <img src="https://picsum.photos/id/1015/800/600" alt="Data Engineering">
      <div class="label">Ingeniería de Datos</div>
    </div>
    <div class="grid-item">
      <img src="https://picsum.photos/id/1025/800/600" alt="Remote Sensing">
      <div class="label">Sensores Remotos</div>
    </div>
    <div class="grid-item">
      <img src="https://picsum.photos/id/1035/800/600" alt="AI & Predictions">
      <div class="label">AI & Predicciones</div>
    </div>
  </div>

  <footer>
    <h2>Lluis Lacán</h2>
    <p>Especialista en Geomática | Análisis Espacial | Innovación con IA</p>
    <div class="socials">
      <a href="https://linkedin.com" target="_blank">in</a>
      <a href="https://github.com" target="_blank">GH</a>
      <a href="https://twitter.com" target="_blank">X</a>
      <a href="mailto:luis.lacan@gmail.com">✉</a>
    </div>
  </footer>
</body>
</html>
