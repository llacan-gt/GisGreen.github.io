<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Lluis Lacán – GeoAnalytics & Geomática</title>
  <meta name="description" content="Lluis Lacán – Especialista en Geomática, Análisis Espacial e Innovación con IA.">
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">

  <style>
    body {
      margin: 0;
      font-family: 'Poppins', sans-serif;
      background: #0e0e0e;
      color: #fff;
      line-height: 1.6;
    }

    main {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      gap: 0;
    }

    .grid-item {
      position: relative;
      overflow: hidden;
      height: 300px;
    }

    .grid-item img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      display: block;
      filter: brightness(70%);
      transition: transform 0.6s ease, filter 0.4s ease;
    }

    .grid-item:hover img {
      transform: scale(1.1);
      filter: brightness(55%);
    }

    .label {
      position: absolute;
      bottom: 20px;
      left: 20px;
      background: rgba(0,0,0,0.65);
      padding: 10px 18px;
      border-radius: 8px;
      color: cyan;
      font-weight: 600;
      font-size: 1.2rem;
      letter-spacing: 0.5px;
    }

    footer {
      text-align: center;
      background: #1a1a1a;
      padding: 2rem 1rem;
      margin-top: 2rem;
    }

    footer h2 {
      margin: 0;
      font-size: 2rem;
      color: cyan;
      font-weight: 600;
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
      font-size: 1.6rem;
    }

    .socials a {
      color: cyan;
      transition: transform 0.3s ease, color 0.3s ease;
    }

    .socials a:hover {
      color: #1abc9c;
      transform: scale(1.2);
    }
  </style>
</head>
<body>
  <main>
    <section class="grid-item">
      <img src="https://picsum.photos/id/1011/800/600" alt="Mapa digital interactivo para geomática">
      <div class="label">Geomática</div>
    </section>
    <section class="grid-item">
      <img src="https://picsum.photos/id/1015/800/600" alt="Pantalla de ingeniería de datos en ciudad inteligente">
      <div class="label">Ingeniería de Datos</div>
    </section>
    <section class="grid-item">
      <img src="https://picsum.photos/id/1025/800/600" alt="Imagen satelital de sensores remotos">
      <div class="label">Sensores Remotos</div>
    </section>
    <section class="grid-item">
      <img src="https://picsum.photos/id/1035/800/600" alt="IA y predicciones aplicadas a transporte urbano">
      <div class="label">IA & Predicciones</div>
    </section>
  </main>

  <footer>
    <h2>Lluis Lacán</h2>
    <p>Especialista en Geomática | Análisis Espacial | Innovación con IA</p>
    <div class="socials">
      <a href="https://linkedin.com" target="_blank" aria-label="LinkedIn"><i class="fab fa-linkedin"></i></a>
      <a href="https://github.com" target="_blank" aria-label="GitHub"><i class="fab fa-github"></i></a>
      <a href="https://twitter.com" target="_blank" aria-label="Twitter"><i class="fab fa-x-twitter"></i></a>
      <a href="mailto:luis.lacan@gmail.com" aria-label="Email"><i class="fas fa-envelope"></i></a>
    </div>
  </footer>
</body>
</html>
