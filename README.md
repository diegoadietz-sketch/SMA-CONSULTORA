[index.html](https://github.com/user-attachments/files/24363700/index.html)
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SMA Consultora | Seguridad e Higiene</title>
    
    <link href="https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Roboto:wght@300;400&display=swap" rel="stylesheet">
    
    <style>
        /* --- CONFIGURACIÓN DINÁMICA Y GENERAL --- */
        html {
            scroll-behavior: smooth; /* Movimiento fluido al navegar */
        }

        * { margin: 0; padding: 0; box-sizing: border-box; }
        
        body { 
            font-family: 'Roboto', sans-serif; 
            line-height: 1.6; 
            color: #333; 
            background-color: #fff; 
        }

        /* --- ENCABEZADO (Menú) --- */
        header {
            background-color: #333333;
            padding: 15px 50px;
            position: sticky;
            top: 0;
            z-index: 1000;
            font-family: 'Bebas Neue', sans-serif;
            letter-spacing: 1px;
        }

        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            max-width: 1200px;
            margin: 0 auto;
        }

        .logo { 
            color: white; 
            font-size: 2.2rem; 
            line-height: 0.9; 
        }

        .logo span { 
            display: block; 
            font-size: 1rem; 
            color: #f39c12; /* Naranja de seguridad */
        }

        nav ul { 
            display: flex; 
            list-style: none; 
            gap: 30px; 
        }

        nav ul li a { 
            color: white; 
            text-decoration: none; 
            font-size: 1.4rem; 
            transition: 0.3s; 
        }

        nav ul li a:hover { 
            color: #f39c12; 
        }

        /* --- SECCIÓN HERO (Bienvenida) --- */
        .hero {
            background-color: #f9f9f9;
            padding: 120px 20px;
            text-align: center;
            border-bottom: 5px solid #f39c12;
        }

        .hero h1 { 
            font-family: 'Bebas Neue', sans-serif; 
            font-size: 4rem; 
            margin-bottom: 20px; 
            letter-spacing: 2px;
        }

        .hero p { 
            max-width: 700px; 
            margin: 0 auto 30px; 
            font-size: 1.2rem; 
            color: #666; 
        }
        
        /* Botón WhatsApp */
        .btn-primario {
            display: inline-block;
            background-color: #f39c12;
            color: white;
            padding: 15px 35px;
            text-decoration: none;
            font-family: 'Bebas Neue', sans-serif;
            font-size: 1.6rem;
            border-radius: 5px;
            transition: all 0.3s ease;
        }

        .btn-primario:hover {
            background-color: #25d366; /* Color WhatsApp */
            transform: scale(1.05);
            box-shadow: 0 5px 15px rgba(37, 211, 102, 0.4);
        }

        /* --- SECCIÓN SERVICIOS --- */
        .servicios { 
            padding: 100px 20px; 
            text-align: center; 
        }

        .titulo-seccion { 
            font-family: 'Bebas Neue', sans-serif; 
            font-size: 3rem; 
            margin-bottom: 50px; 
            color: #333;
        }

        .contenedor-tarjetas {
            display: flex;
            justify-content: center;
            gap: 25px;
            flex-wrap: wrap;
            max-width: 1200px;
            margin: 0 auto;
        }

        .tarjeta {
            background: #fff;
            border: 1px solid #eee;
            padding: 30px;
            width: 300px;
            border-radius: 8px;
            transition: 0.3s;
        }

        .tarjeta:hover { 
            transform: translateY(-10px); 
            border-color: #f39c12; 
            box-shadow: 0 10px 20px rgba(0,0,0,0.05); 
        }

        .icono { 
            font-size: 3rem; 
            margin-bottom: 15px; 
        }

        .tarjeta h3 { 
            font-family: 'Bebas Neue', sans-serif; 
            font-size: 1.6rem; 
            margin-bottom: 10px; 
        }

        /* --- FOOTER (Contacto) --- */
        footer { 
            background-color: #222; 
            color: white; 
            padding: 80px 20px 20px; 
        }

        .contenedor-footer {
            display: flex;
            justify-content: space-between;
            flex-wrap: wrap;
            max-width: 1200px;
            margin: 0 auto;
            gap: 30px;
        }

        .footer-col h4 { 
            font-family: 'Bebas Neue', sans-serif; 
            color: #f39c12; 
            margin-bottom: 15px; 
            font-size: 1.5rem; 
        }

        .footer-copyright { 
            text-align: center; 
            margin-top: 40px; 
            padding-top: 20px; 
            border-top: 1px solid #444; 
            color: #888; 
            font-size: 0.8rem; 
        }

        /* --- ADAPTACIÓN PARA CELULARES --- */
        @media (max-width: 768px) {
            header { padding: 15px 20px; }
            nav { flex-direction: column; gap: 15px; }
            nav ul { gap: 15px; flex-wrap: wrap; justify-content: center; }
            nav ul li a { font-size: 1.1rem; }
            .hero h1 { font-size: 2.5rem; }
            .tarjeta { width: 100%; max-width: 350px; }
        }
    </style>
</head>
<body>

    <header>
        <nav>
            <div class="logo">SMA <span>CONSULTORA</span></div>
            <ul>
                <li><a href="#inicio">INICIO</a></li>
                <li><a href="#servicios">SERVICIOS</a></li>
                <li><a href="#contacto">CONTACTO</a></li>
            </ul>
        </nav>
    </header>

    <section class="hero" id="inicio">
        <h1>BIENVENIDOS A SMA CONSULTORA</h1>
        <p>Expertos en prevención de riesgos, seguridad e higiene industrial. Protegemos lo más valioso de su empresa: su gente.</p>
        <a href="https://wa.me/5491157730424?text=Hola!%20Me%20interesa%20solicitar%20asesoramiento%20con%20SMA%20Consultora" 
           class="btn-primario" target="_blank">SOLICITAR ASESORAMIENTO</a>
    </section>

    <section class="servicios" id="servicios">
        <h2 class="titulo-seccion">NUESTROS SERVICIOS</h2>
        <div class="contenedor-tarjetas">
            <div class="tarjeta">
                <div class="icono">🔍</div>
                <h3>Relevamiento de Riesgos</h3>
                <p>Identificación y evaluación detallada de peligros en los puestos de trabajo.</p>
            </div>
            <div class="tarjeta">
                <div class="icono">🚨</div>
                <h3>Planes de Emergencia</h3>
                <p>Diseño de protocolos de actuación y planes de evacuación eficientes.</p>
            </div>
            <div class="tarjeta">
                <div class="icono">🎓</div>
                <h3>Capacitaciones</h3>
                <p>Formación específica en seguridad e higiene para concientizar al equipo.</p>
            </div>
            <div class="tarjeta">
                <div class="icono">🌿</div>
                <h3>Gestión Ambiental</h3>
                <p>Soluciones sostenibles y cumplimiento de normativas ambientales.</p>
            </div>
            <div class="tarjeta">
                <div class="icono">📏</div>
                <h3>Estudios y Mediciones</h3>
                <p>Mediciones de iluminación, ruido y contaminantes en el ambiente laboral.</p>
            </div>
        </div>
    </section>

    <footer id="contacto">
        <div class="contenedor-footer">
            <div class="footer-col">
                <div class="logo" style="font-size: 1.8rem;">SMA <span style="font-size: 0.8rem;">CONSULTORA</span></div>
                <p style="color: #ccc; margin-top: 10px;">Profesionales al servicio de la industria.</p>
            </div>
            <div class="footer-col">
                <h4>CONTACTO</h4>
                <p>📍 Buenos Aires, Argentina</p>
                <p>📞 11 5773-0424</p>
                <p>✉️ info@smaconsultora.com.ar</p>
            </div>
            <div class="footer-col">
                <h4>REDES SOCIALES</h4>
                <p>LinkedIn | Instagram</p>
            </div>
        </div>
        <div class="footer-copyright">
            &copy; 2024 SMA Consultora - Seguridad e Higiene.
        </div>
    </footer>

</body>
</html>
