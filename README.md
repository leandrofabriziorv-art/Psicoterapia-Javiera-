<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Psic. Javiera Ortiz</title>
    <style>
        /* Colores y tipografía */
        :root {
            --amarillo: #FFC629;
            --rosa: #F25A79;
            --verde: #23A455;
            --texto: #333;
            --fondo: #fff;
            --fuente-titulo: 'Arial', sans-serif;
            --fuente-texto: 'Verdana', sans-serif;
        }

        * { margin: 0; padding: 0; box-sizing: border-box; }

        body {
            font-family: var(--fuente-texto);
            color: var(--texto);
            background-color: var(--fondo);
            line-height: 1.6;
        }

        a { text-decoration: none; color: inherit; }

        header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px;
            background-color: var(--amarillo);
        }

        header img {
            height: 60px;
        }

        nav a {
            margin-left: 20px;
            font-weight: bold;
            color: var(--texto);
        }

        .hero {
            text-align: center;
            padding: 60px 20px;
            background-color: #fdf2e3;
        }

        .hero h1 {
            font-family: var(--fuente-titulo);
            font-size: 2.5rem;
            color: var(--rosa);
            margin-bottom: 20px;
        }

        .hero p {
            font-size: 1.2rem;
            margin-bottom: 30px;
        }

        .btn {
            padding: 12px 25px;
            background-color: var(--rosa);
            color: #fff;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-weight: bold;
            transition: 0.3s;
        }

        .btn:hover {
            background-color: var(--verde);
        }

        section {
            padding: 60px 20px;
        }

        .sobre-mi img {
            max-width: 200px;
            border-radius: 50%;
            margin-bottom: 20px;
        }

        .servicios ul {
            list-style: none;
        }

        .servicios li {
            background-color: #f9f9f9;
            padding: 15px;
            margin-bottom: 10px;
            border-left: 5px solid var(--rosa);
        }

        .contacto form {
            max-width: 500px;
            margin: auto;
            display: flex;
            flex-direction: column;
        }

        .contacto input, .contacto textarea {
            padding: 10px;
            margin-bottom: 15px;
            border-radius: 5px;
            border: 1px solid #ccc;
        }

        .contacto button {
            align-self: flex-start;
        }

        footer {
            text-align: center;
            padding: 20px;
            background-color: #f3f3f3;
            margin-top: 40px;
        }

        /* Responsive */
        @media(max-width: 768px) {
            header { flex-direction: column; }
            nav { margin-top: 10px; }
        }
    </style>
</head>
<body>

    <!-- Header -->
    <header>
        <img src="logo.png" alt="Logo Psic. Javiera Ortiz">
        <nav>
            <a href="#inicio">Inicio</a>
            <a href="#sobre-mi">Sobre mí</a>
            <a href="#servicios">Servicios</a>
            <a href="#contacto">Contacto</a>
        </nav>
    </header>

    <!-- Hero / Inicio -->
    <section class="hero" id="inicio">
        <h1>Acompañamiento terapéutico para mujeres +21 años</h1>
        <p>Psicoterapia relacional centrada en el vínculo terapéutico, para tu bienestar emocional y crecimiento personal.</p>
        <button class="btn" onclick="window.location.href='#contacto'">Agendar cita</button>
    </section>

    <!-- Sobre mí -->
    <section class="sobre-mi" id="sobre-mi">
        <h2>Sobre mí</h2>
        <img src="foto.jpg" alt="Foto Psic. Javiera Ortiz">
        <p>Trabajo desde la psicoterapia relacional, priorizando el vínculo terapéutico como base de todo el proceso. En nuestro espacio podrás reflexionar sobre tu historia familiar, relaciones, emociones y descubrir una nueva versión de ti alineada con tus objetivos.</p>
    </section>

    <!-- Servicios -->
    <section class="servicios" id="servicios">
        <h2>Servicios y Temáticas</h2>
        <ul>
            <li>Ansiedad · Depresión · Estrés · Autoexigencia</li>
            <li>Procesos de reparación · Elaboración de experiencias traumáticas</li>
            <li>Diagnóstico tardío de autismo en mujeres adultas · Fortalecimiento de la autoestima</li>
            <li>Síndrome del cuidador · Pérdidas y duelos</li>
        </ul>
    </section>

    <!-- Contacto -->
    <section class="contacto" id="contacto">
        <h2>Contacto</h2>
        <form action="mailto:tuemail@correo.com" method="post" enctype="text/plain">
            <input type="text" name="nombre" placeholder="Nombre" required>
            <input type="email" name="correo" placeholder="Correo" required>
            <textarea name="mensaje" rows="5" placeholder="Mensaje" required></textarea>
            <button type="submit" class="btn">Enviar mensaje</button>
        </form>
        <p>Sígueme en Instagram: <a href="https://instagram.com/psic.javieraortiz" target="_blank">@psic.javieraortiz</a></p>
    </section>

    <!-- Footer -->
    <footer>
        &copy; 2025 Psic. Javiera Ortiz. Todos los derechos reservados.
    </footer>

</body>
</html>
