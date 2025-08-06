<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Mi Sitio Web Profesional</title>

  <!-- Google Fonts -->
  <link href="https://media.istockphoto.com/id/1389962390/es/vector/dise%C3%B1o-isom%C3%A9trico-de-desarrollo-web.jpg?s=612x612&w=0&k=20&c=Cx2n3gzoicyB740ecyh--kB1Qdlue6WHB5NXn23-tdU=" rel="stylesheet">

  <style>
   * {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: 'Poppins', sans-serif;
  background: lab(94.62% -1.03 1.8);
  color: #212529;
  line-height: 1.6;
  scroll-behavior: smooth;
}

header {
  background: linear-gradient(90deg, #0d6efd, #0a58ca);
  color: white;
  padding: 20px 30px;
  position: sticky;
  top: 0;
  z-index: 1000;
  box-shadow: 0 4px 6px rgba(0,0,0,0.1);
  transition: all 0.3s ease;
}

header h1 {
  font-size: 28px;
}

#menu-toggle {
  display: none;
  font-size: 28px;
  background: none;
  border: none;
  color: white;
  position: absolute;
  top: 25px;
  right: 30px;
  cursor: pointer;
}

nav {
  margin-top: 15px;
  display: flex;
  gap: 20px;
  justify-content: center;
  flex-wrap: wrap;
  transition: all 0.3s ease;
}

nav a {
  color: white;
  text-decoration: none;
  font-weight: 600;
  padding: 10px 18px;
  border-radius: 5px;
  transition: background 0.3s ease, transform 0.2s;
}

nav a:hover {
  background: rgba(255, 255, 255, 0.2);
  transform: scale(1.05);
}

section {
  padding: 70px 20px;
  text-align: center;
}

.inicio {
  background: url('https://media.istockphoto.com/id/1503858430/es/vector/concepto-de-desarrollo-de-software-de-sitios-web-sitio-de-dise%C3%B1o-web-y-aplicaci%C3%B3n-m%C3%B3vil-en.jpg?s=612x612&w=0&k=20&c=mZoL9erxzcblOQHoprcasZSo1hKHTQq1-lnu2n_9Pto=') no-repeat center center/cover;
  color: rgb(245, 181, 7);
  padding: 130px 20px;
}

.inicio h2 {
  font-size: 48px;
  font-weight: 700;
  margin-bottom: 20px;
  text-shadow: 1px 1px 4px rgba(0,0,0,0.4);
}

.inicio p {
  font-size: 20px;
  max-width: 700px;
  margin: 0 auto;
}

.servicios {
  background: #ffffff;
}

.servicios h2 {
  margin-bottom: 40px;
  font-size: 36px;
}

.servicios .items {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 30px;
}

.servicio {
  width: 260px;
  background: #f1f1f1;
  border-radius: 15px;
  padding: 25px;
  box-shadow: 0 6px 12px rgba(0,0,0,0.05);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.servicio:hover {
  transform: translateY(-5px);
  box-shadow: 0 10px 20px rgba(0,0,0,0.1);
}

.servicio img {
  width: 100%;
  border-radius: 10px;
  margin-bottom: 15px;
}

.galeria {
  background: #e9ecef;
}

.galeria h2 {
  margin-bottom: 35px;
  font-size: 36px;
}

.galeria-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
  gap: 15px;
}

.galeria-grid img {
  width: 100%;
  border-radius: 12px;
  height: 180px;
  object-fit: cover;
  transition: transform 0.3s ease;
}

.galeria-grid img:hover {
  transform: scale(1.03);
}

.nosotros {
  background: #ffffff;
}

.nosotros h2 {
  margin-bottom: 25px;
  font-size: 36px;
}

.nosotros p {
  max-width: 850px;
  margin: 0 auto 20px;
  font-size: 18px;
  color: #555;
}

.formulario {
  max-width: 600px;
  background: white;
  margin: 0 auto;
  padding: 40px 30px;
  border-radius: 20px;
  box-shadow: 0 0 25px rgba(0,0,0,0.05);
}

.formulario h2 {
  margin-bottom: 25px;
  font-size: 30px;
}

.formulario label {
  display: block;
  margin-top: 18px;
  font-weight: 600;
}

.formulario input {
  width: 100%;
  padding: 12px 15px;
  border: 1px solid #ccc;
  border-radius: 10px;
  margin-top: 6px;
  font-size: 16px;
}

.formulario button {
  background: #0d6efd;
  color: white;
  padding: 14px;
  border: none;
  border-radius: 10px;
  font-size: 18px;
  margin-top: 25px;
  width: 100%;
  cursor: pointer;
  transition: background 0.3s ease;
}

.formulario button:hover {
  background: #084298;
}

.mensaje {
  color: red;
  font-size: 14px;
  margin-top: 5px;
  display: block;
}

@media (max-width: 768px) {
  #menu-toggle {
    display: block;
  }

  nav {
    display: none;
    flex-direction: column;
    background: #0a58ca;
    padding: 10px 0;
  }

  nav.mostrar {
    display: flex;
  }

  .servicios .items {
    flex-direction: column;
    align-items: center;
  }

  .servicio {
    width: 90%;
  }

  .galeria-grid {
    grid-template-columns: 1fr 1fr;
  }
}

  </style>
</head>

<body>
  <header>
    <h1>Mi Sitio Web Profesional</h1>
    <button id="menu-toggle">☰</button>
    <nav id="menu">
      <a href="#inicio">Inicio</a>
      <a href="#servicios">Servicios</a>
      <a href="#galeria">Galería</a>
      <a href="#nosotros">Nosotros</a>
      <a href="#contacto">Contacto</a>
    </nav>
  </header>

  <!-- INICIO -->
  <section id="inicio" class="inicio">
    <h2>Bienvenido a Nuestro Sitio</h2>
    <p>Descubre soluciones únicas para potenciar tu negocio y transformar tu visión en realidad. Calidad, innovación y confianza nos definen.</p>
  </section>

  <!-- SERVICIOS -->
  <section id="servicios" class="servicios">
    <h2>Nuestros Servicios</h2>
    <div class="items">
      <div class="servicio">
        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQPTidbPinPzlrOPBCK0iM_BdI6-6gNG62TAg&s" alt="Desarrollo Web">
        <h3>Desarrollo Web</h3>
        <p>Creación de sitios modernos, rápidos y responsivos.</p>
      </div>
      <div class="servicio">
        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRUDAxLf0uUS-mOIoQ3ubeE8-EaLB3KldbbAg&s" alt="Marketing Digital">
        <h3>Marketing Digital</h3>
        <p>Publicidad en redes, SEO y crecimiento de marca.</p>
      </div>
      <div class="servicio">
        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTA2MjafhOAliOkMGOlsh74Qvlatr3rLIwF_Q&s" alt="Consultoría">
        <h3>Consultoría</h3>
        <p>Asesoría estratégica para tu emprendimiento.</p>
      </div>
    </div>
  </section>

  <!-- GALERÍA -->
  <section id="galeria" class="galeria">
    <h2>Galería</h2>
    <div class="galeria-grid">
      <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRGOMjMgLnIIimWkfcJmFStjKgnA_m24QpyTA&s" alt="Galería 1">
      <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRTSRscuvrS88HwkJIU3XJV-xs1QJgfJLMm-Q&s" alt="Galería 2">
      <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQAKPYvqC5Dxwz48Ejb-7FlQ8QYi1w6En_mQw&s" alt="Galería 3">
      <img src="https://www.exfo.com/contentassets/dff4900dcfe3476eb10996a227af97cf/20190171_sa_value-added-services-top-banner_2000x800.jpg?rxy=0.5,0.5&rmode=crop" alt="Galería 4">
    </div>
  </section>

  <!-- NOSOTROS -->
  <section id="nosotros" class="nosotros">
    <h2>Sobre Nosotros</h2>
    <p>Somos un equipo apasionado por la tecnología, el diseño y la innovación. Ayudamos a emprendedores y empresas a alcanzar sus metas mediante soluciones digitales personalizadas.</p>
    <p><strong>Misión:</strong> Brindar servicios de alta calidad que impacten positivamente a nuestros clientes.</p>
    <p><strong>Visión:</strong> Ser líderes en transformación digital en Latinoamérica.</p>
  </section>

  <!-- CONTACTO -->
  <section id="contacto" class="formulario">
    <h2>Contáctanos</h2>
    <form id="contacto-form">
      <label for="nombre">Nombre:</label>
      <input type="text" id="nombre">
      <span class="mensaje" id="nombreMsg"></span>

      <label for="correo">Correo electrónico:</label>
      <input type="email" id="correo">
      <span class="mensaje" id="correoMsg"></span>

      <button type="submit">Enviar</button>
    </form>
  </section>

  <script>
    // Menú responsive
    document.getElementById("menu-toggle").addEventListener("click", () => {
      document.getElementById("menu").classList.toggle("mostrar");
    });

    // Validación del formulario
    document.getElementById("contacto-form").addEventListener("submit", function(e) {
      e.preventDefault();
      let nombre = document.getElementById("nombre").value.trim();
      let correo = document.getElementById("correo").value.trim();
      let esValido = true;

      if (nombre === "") {
        document.getElementById("nombreMsg").textContent = "Por favor ingresa tu nombre.";
        esValido = false;
      } else {
        document.getElementById("nombreMsg").textContent = "";
      }

      const regexCorreo = /^[^@\s]+@[^@\s]+\.[^@\s]+$/;
      if (!regexCorreo.test(correo)) {
        document.getElementById("correoMsg").textContent = "Ingresa un correo válido.";
        esValido = false;
      } else {
        document.getElementById("correoMsg").textContent = "";
      }

      if (esValido) {
        alert("Formulario enviado correctamente ✅");
        this.reset();
      }
    });
  </script>
</body>
</html>

