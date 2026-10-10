index.html
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Fire Alert | Alertas de emergencia</title>

  <style>
    :root {
      --fondo: #07111f;
      --fondo-2: #0d1b2e;
      --rojo: #ef3340;
      --naranja: #ff8a00;
      --blanco: #ffffff;
      --texto: #b9c5d6;
      --borde: rgba(255,255,255,.12);
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      font-family: Arial, sans-serif;
      color: var(--blanco);
      background: var(--fondo);
      line-height: 1.6;
    }

    a {
      color: inherit;
      text-decoration: none;
    }

    .contenedor {
      width: min(1120px, 92%);
      margin: auto;
    }

    header {
      position: sticky;
      top: 0;
      z-index: 10;
      background: rgba(7,17,31,.9);
      border-bottom: 1px solid var(--borde);
      backdrop-filter: blur(12px);
    }

    nav {
      min-height: 72px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 20px;
    }

    .logo {
      display: flex;
      align-items: center;
      gap: 10px;
      font-size: 1.25rem;
      font-weight: bold;
    }

    .logo-icono {
      display: grid;
      place-items: center;
      width: 40px;
      height: 40px;
      border-radius: 12px;
      background: linear-gradient(135deg, var(--rojo), var(--naranja));
      font-size: 1.4rem;
    }

    .menu {
      display: flex;
      gap: 25px;
      color: var(--texto);
      font-size: .95rem;
    }

    .menu a:hover {
      color: white;
    }

    .boton {
      display: inline-block;
      padding: 13px 20px;
      border-radius: 10px;
      font-weight: bold;
      transition: .2s;
    }

    .boton-principal {
      color: white;
      background: linear-gradient(135deg, var(--rojo), var(--naranja));
      box-shadow: 0 10px 25px rgba(239,51,64,.25);
    }

    .boton-principal:hover {
      transform: translateY(-2px);
    }

    .boton-secundario {
      border: 1px solid var(--borde);
      color: var(--texto);
    }

    .hero {
      padding: 95px 0 75px;
      background:
        radial-gradient(circle at 80% 20%, rgba(239,51,64,.2), transparent 30%),
        radial-gradient(circle at 20% 70%, rgba(255,138,0,.12), transparent 30%);
    }

    .hero-grid {
      display: grid;
      grid-template-columns: 1.1fr .9fr;
      align-items: center;
      gap: 60px;
    }

    .etiqueta {
      display: inline-block;
      margin-bottom: 18px;
      padding: 7px 12px;
      border: 1px solid rgba(255,138,0,.35);
      border-radius: 30px;
      color: #ffb04d;
      background: rgba(255,138,0,.08);
      font-size: .85rem;
    }

    h1 {
      max-width: 650px;
      margin-bottom: 20px;
      font-size: clamp(2.5rem, 6vw, 5rem);
      line-height: 1.05;
    }

    h1 span {
      color: var(--rojo);
    }

    .hero p {
      max-width: 570px;
      margin-bottom: 30px;
      color: var(--texto);
      font-size: 1.1rem;
    }

    .botones {
      display: flex;
      flex-wrap: wrap;
      gap: 14px;
    }

    .telefono {
      width: 270px;
      margin: auto;
      padding: 12px;
      border: 8px solid #17283d;
      border-radius: 35px;
      background: #050b13;
      box-shadow: 0 25px 70px rgba(0,0,0,.45);
      transform: rotate(3deg);
    }

    .pantalla {
      min-height: 500px;
      padding: 22px 16px;
      border-radius: 23px;
      background: linear-gradient(180deg, #162a42, #091321);
    }

    .barra {
      display: flex;
      justify-content: space-between;
      margin-bottom: 25px;
      color: var(--texto);
      font-size: .8rem;
    }

    .alerta {
      margin-bottom: 15px;
      padding: 18px;
      border-radius: 16px;
      background: linear-gradient(135deg, #e52d3b, #9e1723);
    }

    .alerta strong {
      display: block;
      margin-bottom: 5px;
      font-size: 1.2rem;
    }

    .tarjeta {
      margin-top: 15px;
      padding: 16px;
      border: 1px solid var(--borde);
      border-radius: 15px;
      background: rgba(255,255,255,.06);
    }

    .tarjeta small {
      color: var(--texto);
    }

    section {
      padding: 85px 0;
    }

    .titulo-seccion {
      max-width: 650px;
      margin: 0 auto 45px;
      text-align: center;
    }

    .titulo-seccion h2 {
      margin-bottom: 12px;
      font-size: 2.3rem;
    }

    .titulo-seccion p {
      color: var(--texto);
    }

    .funciones {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 20px;
    }

    .funcion {
      padding: 28px;
      border: 1px solid var(--borde);
      border-radius: 18px;
      background: var(--fondo-2);
    }

    .funcion-icono {
      display: grid;
      place-items: center;
      width: 50px;
      height: 50px;
      margin-bottom: 18px;
      border-radius: 14px;
      background: rgba(239,51,64,.15);
      font-size: 1.5rem;
    }

    .funcion h3 {
      margin-bottom: 10px;
    }

    .funcion p {
      color: var(--texto);
    }

    .descarga {
      text-align: center;
      background: linear-gradient(135deg, #a91d2a, #ef3340);
    }

    .descarga p {
      max-width: 600px;
      margin: 15px auto 25px;
      color: #ffe5e5;
    }

    footer {
      padding: 30px 0;
      color: var(--texto);
      border-top: 1px solid var(--borde);
      text-align: center;
      font-size: .9rem;
    }

    @media (max-width: 800px) {
      .menu {
        display: none;
      }

      .hero-grid {
        grid-template-columns: 1fr;
        text-align: center;
      }

      .hero p {
        margin-right: auto;
        margin-left: auto;
      }

      .botones {
        justify-content: center;
      }

      .funciones {
        grid-template-columns: 1fr;
      }

      .telefono {
        transform: none;
      }
    }
  </style>
</head>

<body>

  <header>
    <div class="contenedor">
      <nav>
        <a href="#" class="logo">
          <span class="logo-icono">🔥</span>
          Fire Alert
        </a>

        <div class="menu">
          <a href="#funciones">Funciones</a>
          <a href="#nosotros">Sobre la app</a>
          <a href="#descarga">Descargar</a>
        </div>

        <a href="#descarga" class="boton boton-principal">Comenzar</a>
      </nav>
    </div>
  </header>

  <main>

    <section class="hero">
      <div class="contenedor hero-grid">
        <div>
          <span class="etiqueta">🚨 Respuesta rápida ante emergencias</span>

          <h1>La alerta correcta en el <span>momento indicado.</span></h1>

          <p>
            Fire Alert ayuda a comunicar y coordinar alertas de emergencia
            de forma rápida, clara y organizada.
          </p>

          <div class="botones">
            <a href="#descarga" class="boton boton-principal">Descargar APK</a>
            <a href="#funciones" class="boton boton-secundario">Conocer más</a>
          </div>
        </div>

        <div class="telefono">
          <div class="pantalla">
            <div class="barra">
              <span>Fire Alert</span>
              <span>● En línea</span>
            </div>

            <div class="alerta">
              <strong>🚨 Nueva alerta</strong>
              Incendio detectado en zona norte.
            </div>

            <div class="tarjeta">
              <small>Ubicación</small>
              <strong>📍 Avenida Central 245</strong>
            </div>

            <div class="tarjeta">
              <small>Estado del equipo</small>
              <strong>✅ Unidad asignada</strong>
            </div>

            <div class="tarjeta">
              <small>Tiempo estimado</small>
              <strong>⏱ 04 minutos</strong>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section id="funciones">
      <div class="contenedor">
        <div class="titulo-seccion">
          <h2>Todo bajo control</h2>
          <p>Herramientas pensadas para mejorar la comunicación durante una emergencia.</p>
        </div>

        <div class="funciones">
          <article class="funcion">
            <div class="funcion-icono">🚨</div>
            <h3>Alertas inmediatas</h3>
            <p>Recibí avisos importantes en tiempo real y sin complicaciones.</p>
          </article>

          <article class="funcion">
            <div class="funcion-icono">📍</div>
            <h3>Ubicación precisa</h3>
            <p>Consultá rápidamente el lugar exacto de cada emergencia.</p>
          </article>

          <article class="funcion">
            <div class="funcion-icono">👨‍🚒</div>
            <h3>Equipos coordinados</h3>
            <p>Organizá mejor las tareas y mantené informado a tu equipo.</p>
          </article>
        </div>
      </div>
    </section>

    <section id="nosotros">
      <div class="contenedor">
        <div class="titulo-seccion">
          <h2>Una solución simple para situaciones críticas</h2>
          <p>
            Fire Alert fue creada para facilitar la comunicación,
            reducir demoras y ayudar a tomar mejores decisiones.
          </p>
        </div>
      </div>
    </section>

    <section id="descarga" class="descarga">
      <div class="contenedor">
        <h2>Preparado para responder</h2>
        <p>Descargá Fire Alert y mantené tus alertas organizadas en un solo lugar.</p>
        <a href="#" class="boton boton-secundario">Descargar APK</a>
      </div>
    </section>

  </main>

  <footer>
    <div class="contenedor">
      © 2026 Fire Alert. Todos los derechos reservados.
    </div>
  </footer>

</body>
</html>
