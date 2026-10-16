# landing
voy hacer una landing
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>ROALDIX Technologies | Desarrollo de Software a Medida</title>
  <meta name="description" content="Especialistas en desarrollo de aplicaciones móviles, sistemas ERP/CRM, automatización de procesos y páginas web.">
  
  <style>
    /* Variables de color para mantener la identidad de la marca */
    :root {
      --bg-dark: #070b14;
      --bg-card: #111827;
      --accent-blue: #2563eb;
      --accent-cyan: #06b6d4;
      --text-main: #f8fafc;
      --text-muted: #94a3b8;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      font-family: system-ui, -apple-system, sans-serif;
      background-color: var(--bg-dark);
      color: var(--text-main);
      line-height: 1.6;
    }

    /* Navegación */
    header {
      background: rgba(17, 24, 39, 0.9);
      backdrop-filter: blur(10px);
      position: fixed;
      width: 100%;
      top: 0;
      z-index: 100;
      border-bottom: 1px solid rgba(255, 255, 255, 0.1);
    }

    .nav-container {
      max-width: 1200px;
      margin: 0 auto;
      padding: 20px;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    .logo { font-size: 1.5rem; font-weight: bold; background: linear-gradient(90deg, #60a5fa, #22d3ee); -webkit-background-clip: text; -webkit-text-fill-color: transparent; }
    
    .nav-links a {
      color: var(--text-main);
      text-decoration: none;
      margin-left: 20px;
      font-size: 0.9rem;
      transition: color 0.3s;
    }
    .nav-links a:hover { color: var(--accent-cyan); }

    /* Secciones generales */
    section { padding: 100px 20px; max-width: 1200px; margin: 0 auto; }
    .section-title { text-align: center; font-size: 2.5rem; margin-bottom: 50px; }
    .section-title span { color: var(--accent-cyan); }

    /* Sección Hero (Inicio) */
    .hero {
      height: 100vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      text-align: center;
      background: radial-gradient(circle at center, #1e293b 0%, var(--bg-dark) 80%);
    }

    .hero h1 { font-size: 3.5rem; margin-bottom: 20px; max-width: 800px; line-height: 1.2; }
    .hero p { font-size: 1.2rem; color: var(--text-muted); max-width: 600px; margin-bottom: 40px; }
    
    .btn-primary {
      background: var(--accent-blue);
      color: white;
      padding: 15px 30px;
      border-radius: 8px;
      text-decoration: none;
      font-weight: bold;
      transition: background 0.3s;
    }
    .btn-primary:hover { background: #1d4ed8; }

    /* Portafolio / Servicios (Grid) */
    .services-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      gap: 30px;
    }

    .service-card {
      background: var(--bg-card);
      padding: 30px;
      border-radius: 12px;
      border: 1px solid rgba(255,255,255,0.05);
      transition: transform 0.3s;
    }
    .service-card:hover { transform: translateY(-5px); border-color: var(--accent-cyan); }
    .service-card h3 { font-size: 1.5rem; margin-bottom: 15px; }
    .service-card p { color: var(--text-muted); font-size: 0.95rem; }

    /* Metodología (Paso a paso) */
    .timeline {
      display: flex;
      flex-direction: column;
      gap: 30px;
      max-width: 800px;
      margin: 0 auto;
    }
    .step {
      display: flex;
      gap: 20px;
      background: rgba(255,255,255,0.03);
      padding: 20px;
      border-radius: 12px;
    }
    .step-number {
      font-size: 2rem;
      font-weight: bold;
      color: var(--accent-cyan);
      opacity: 0.8;
    }

    /* Footer / Contacto */
    footer {
      background: var(--bg-card);
      padding: 50px 20px;
      text-align: center;
      border-top: 1px solid rgba(255,255,255,0.1);
    }
    footer h2 { margin-bottom: 20px; }
    
    @media (max-width: 768px) {
      .hero h1 { font-size: 2.5rem; }
      .nav-links { display: none; /* Para móvil se puede implementar un menú hamburguesa después */ }
    }
  </style>
</head>
<body>

  <!-- Encabezado de Navegación -->
  <header>
    <div class="nav-container">
      <div class="logo">ROALDIX</div>
      <nav class="nav-links">
        <a href="#servicios">Servicios</a>
        <a href="#metodologia">Metodología</a>
        <a href="#contacto" class="btn-primary" style="padding: 10px 20px;">Contactar</a>
      </nav>
    </div>
  </header>

  <!-- Sección Principal (Hero) -->
  <section class="hero" id="inicio">
    <h1>Transformamos la operativa de tu negocio en <span>Código y Resultados</span></h1>
    <p>Desarrollo de software a medida, aplicaciones móviles nativas y sistemas de automatización inteligente para empresas que buscan escalar.</p>
    <a href="#contacto" class="btn-primary">Cotizar mi Proyecto Tecnológico</a>
  </section>

  <!-- Sección de Servicios / Arquitectura -->
  <section id="servicios">
    <h2 class="section-title">Nuestras <span>Soluciones</span></h2>
    <div class="services-grid">
      <div class="service-card">
        <h3>📱 Desarrollo Móvil Nativo</h3>
        <p>Creamos aplicaciones para iOS y Android utilizando arquitecturas escalables, garantizando rendimiento y excelente experiencia de usuario (UX/UI).</p>
      </div>
      <div class="service-card">
        <h3>📊 Sistemas ERP & CRM</h3>
        <p>Centralizamos tu contabilidad, inventario y ventas. Desarrollamos módulos a la medida que se conectan en tiempo real a tus bases de datos.</p>
      </div>
      <div class="service-card">
        <h3>⚡ Automatización de Procesos</h3>
        <p>Eliminamos tareas repetitivas conectando sistemas a través de APIs, scripts avanzados y automatización inteligente con herramientas de IA.</p>
      </div>
    </div>
  </section>

  <!-- Sección de Metodología de Trabajo -->
  <section id="metodologia">
    <h2 class="section-title">Cómo <span>Trabajamos</span></h2>
    <div class="timeline">
      <div class="step">
        <div class="step-number">01</div>
        <div>
          <h3>Levantamiento de Requerimientos</h3>
          <p>Analizamos tus flujos operativos actuales y definimos la arquitectura del sistema, la base de datos y los objetivos técnicos del proyecto.</p>
        </div>
      </div>
      <div class="step">
        <div class="step-number">02</div>
        <div>
          <h3>Prototipado y Diseño</h3>
          <p>Creamos los esquemas (wireframes) y el diseño visual de las interfaces para que apruebes cómo se verá y funcionará el software antes de programar.</p>
        </div>
      </div>
      <div class="step">
        <div class="step-number">03</div>
        <div>
          <h3>Desarrollo e Implementación</h3>
          <p>Escribimos código limpio y optimizado. Realizamos pruebas de QA (Quality Assurance) para garantizar que el sistema es seguro y no tiene errores.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Footer y Contacto -->
  <footer id="contacto">
    <h2>¿Listo para digitalizar tu empresa?</h2>
    <p style="color: var(--text-muted); margin-bottom: 30px;">Envíanos un mensaje directo para agendar una reunión técnica de evaluación.</p>
    <!-- Aquí puedes conectar el mismo enlace de WhatsApp de tu postal -->
    <a href="https://wa.me/523231960575?text=Hola,%20visité%20su%20página%20web%20y%20me%20interesa%20agendar%20una%20evaluación%20técnica%20para%20un%20desarrollo." target="_blank" class="btn-primary" style="background: #25D366; color: #051b0d;">
      Agendar reunión vía WhatsApp
    </a>
    <p style="margin-top: 50px; font-size: 0.8rem; color: var(--text-muted);">
      &copy; 2026 ROALDIX Technologies. Todos los derechos reservados.
    </p>
  </footer>

</body>
</html>
