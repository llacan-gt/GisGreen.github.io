<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Lluis Lacán - Análisis Geoespacial</title>
  <style>
    /* Estilos generales */
    body {
      margin: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      line-height: 1.6;
      color: #333;
      background: #f9f9f9;
    }

    .container {
      width: 90%;
      max-width: 1000px;
      margin: auto;
      padding: 1rem;
    }

    /* Encabezado */
    header {
      background: linear-gradient(135deg, #2c3e50, #34495e);
      color: white;
      padding: 2rem 1rem;
      text-align: center;
    }
    header h1 {
      margin: 0;
      font-size: 2.5rem;
    }
    header p {
      font-size: 1.2rem;
      opacity: 0.9;
    }

    /* Navegación */
    nav {
      background: #2c3e50;
      padding: 0.8rem;
    }
    nav .container {
      display: flex;
      justify-content: center;
      gap: 2rem;
    }
    nav a {
      color: white;
      text-decoration: none;
      font-weight: bold;
    }
    nav a:hover {
      text-decoration: underline;
    }

    /* Secciones */
    main h2 {
      color: #2c3e50;
      margin-top: 2rem;
      border-left: 5px solid #2c3e50;
      padding-left: 0.5rem;
    }
    ul {
      list-style: none;
      padding-left: 0;
    }
    ul li {
      margin: 0.5rem 0;
    }

    /* Botón */
    .btn {
      display: inline-block;
      padding: 0.6rem 1.2rem;
      background: #2c3e50;
      color: white;
      border-radius: 5px;
      text-decoration: none;
    }
    .btn:hover {
      background: #1abc9c;
      transition: 0.3s;
    }

    /* Pie de página */
    footer {
      background: #34495e;
      color: white;
      text-align: center;
      padding: 1rem;
      margin-top: 2rem;
    }
  </style>
</head>
<body>
  <!-- Encabezado -->
  <header>
    <div class="container">
      <h1>Lluis Lacán</h1>
      <p>Explora el fascinante mundo del análisis de información geoespacial</p>
    </div>
  </header>

  <!-- Navegación -->
  <nav>
    <div class="container">
      <a href="#inicio">Inicio</a>
      <a href="#geomatica">Geomática</a>
      <a href="#personalizacion">Personalización</a>
      <a href="#contacto">Contacto</a>
    </div>
  </nav>

  <!-- Contenido principal -->
  <main class="container">
    <section id="inicio">
      <h2>Bienvenido</h2>
      <p>
        Aquí encontrarás recursos, guías y herramientas que te ayudarán a aprender y aplicar la 
        <strong>geomática</strong> en distintos ámbitos, así como técnicas creativas de 
        <strong>personalización de prendas</strong>.
      </p>
    </section>

    <section id="geomatica">
      <h2>Geomática</h2>
      <p>Descubre y aprende sobre:</p>
      <ul>
        <li>🌍 ArcGIS Online</li>
        <li>💻 Google Colab</li>
        <li>🗄️ Bases de datos geoespaciales</li>
        <li>📷 Fotogrametría</li>
        <li>🛰️ Google Earth Engine</li>
      </ul>
    </section>

    <section id="personalizacion">
      <h2>Personalización de Prendas</h2>
      <p>Servicios creativos para darle un toque único a tus prendas:</p>
      <ul>
        <li>🧵 Bordado computarizado</li>
        <li>🎨 Vinil textil</li>
      </ul>
    </section>

    <section id="contacto">
      <h2>Contacto</h2>
      <p>Puedes escribirme a:</p>
      <p><a href="mailto:luis.lacan@gmail.com" class="btn">📩 luis.lacan@gmail.com</a></p>
    </section>
  </main>

  <!-- Pie de página -->
  <footer>
    <p>&copy; 2025 Lluis Lacán | Creado con ❤️ y publicado en GitHub Pages</p>
  </footer>
</body>
</html>
