<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />

  <style>
    @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;700&display=swap');

    * {
      margin: 0; padding: 0; box-sizing: border-box;
    }

    body {
      background: #ffffff;
      color: #000000;
      font-family: 'Poppins', sans-serif;
      min-height: 100vh;
      display: flex;
      flex-direction: column;
      align-items: center;
      padding: 50px 20px;
      user-select: none;
    }

    header {
      width: 100%;
      max-width: 1200px;
      display: flex;
      justify-content: flex-start;
      align-items: center;
      margin-bottom: 60px;
    }

    .logo {
      height: 80px;
      filter: drop-shadow(0 0 6px #888);
      transition: transform 0.4s ease;
      cursor: pointer;
    }

    .logo:hover {
      transform: scale(1.15) rotate(-7deg);
      filter: drop-shadow(0 0 12px #aaa);
    }

    h1 {
      font-size: 3.6rem;
      font-weight: 700;
      text-align: center;
      color: #000;
      margin-bottom: 18px;
      letter-spacing: 2px;
      user-select: text;
    }

    p.subtitle {
      max-width: 720px;
      font-size: 1.3rem;
      color: #333;
      text-align: center;
      margin-bottom: 70px;
      line-height: 1.6;
      user-select: text;
    }

    .platforms {
      display: grid;
      grid-template-columns: repeat(auto-fit,minmax(240px,1fr));
      gap: 38px;
      width: 100%;
      max-width: 1100px;
      padding: 0 10px;
    }

    .card {
      background: #f7f7f7;
      border-radius: 20px;
      padding: 30px 25px;
      box-shadow: 0 0 20px #ddd;
      color: #000;
      cursor: pointer;
      transition: transform 0.4s ease, box-shadow 0.4s ease;
      display: flex;
      flex-direction: column;
      align-items: center;
      text-align: center;
      user-select: none;
      position: relative;
      border: 2px solid transparent;
    }

    .card:hover {
      transform: translateY(-18px) rotateX(9deg) rotateY(14deg);
      box-shadow: 0 0 35px #ccc;
      border-color: #999;
      z-index: 20;
    }

    .card img {
      max-width: 140px;
      margin-bottom: 22px;
      filter: drop-shadow(0 0 10px #bbb);
      height: auto;
      object-fit: contain;
      transition: filter 0.4s ease;
    }

    .card:hover img {
      filter: drop-shadow(0 0 15px #aaa);
    }

    .card h3 {
      font-size: 1.7rem;
      color: #222;
      margin-bottom: 8px;
      user-select: text;
    }

    .price {
      font-size: 1.3rem;
      font-weight: 700;
      color: #ff9900;
      margin-bottom: 15px;
      user-select: text;
    }

    .card p {
      font-size: 1.05rem;
      line-height: 1.5;
      color: #555;
      min-height: 80px;
      user-select: text;
    }

    .btn-cta {
      margin-top: 75px;
      background: linear-gradient(90deg, #333, #666);
      border: none;
      padding: 20px 65px;
      border-radius: 50px;
      font-size: 1.45rem;
      font-weight: 700;
      color: #fff;
      cursor: pointer;
      box-shadow: 0 0 25px #aaa;
      transition: all 0.5s ease;
      text-transform: uppercase;
      letter-spacing: 2px;
      user-select: none;
      position: relative;
      overflow: hidden;
    }

    .btn-cta::before {
      content: '';
      position: absolute;
      top: -50%;
      left: -50%;
      width: 200%;
      height: 200%;
      background: linear-gradient(45deg, rgba(255,255,255,0.5), rgba(255,255,255,0));
      transform: rotate(45deg);
      transition: all 0.6s ease;
      pointer-events: none;
      filter: blur(20px);
      animation: shine 3.5s infinite linear;
      z-index: 1;
    }

    @keyframes shine {
      0% { transform: translateX(-100%) rotate(45deg); }
      100% { transform: translateX(100%) rotate(45deg); }
    }

    .btn-cta:hover {
      background: linear-gradient(90deg, #555, #888);
      box-shadow: 0 0 35px #bbb;
    }

    footer {
      margin-top: 90px;
      font-size: 0.9rem;
      color: #666;
      text-align: center;
      user-select: none;
    }

    @media (max-width: 720px) {
      h1 { font-size: 2.8rem; }
      p.subtitle { font-size: 1.1rem; }
      .card { padding: 25px 18px; }
      .card img { max-width: 110px; }
      .card h3 { margin-bottom: 5px; }
      .price { margin-bottom: 12px; }
    }
  </style>
</head>
<body>

<header>
  <img src="logo.png" alt="Logo Vendo" class="logo" />
</header>

<h1>Tu Portal Premium de Streaming</h1>
<p class="subtitle">
  Netflix, HBO Max, Prime Video, Disney+, Star+, Paramount+, Apple TV+, Hulu, Peacock y más en un solo lugar.
</p>

<div class="platforms">
  <article class="card">
    <img src="https://upload.wikimedia.org/wikipedia/commons/0/08/Netflix_2015_logo.svg" alt="Netflix" />
    <h3>Netflix</h3>
    <div class="price">L80</div>
    <p>Accede a series y películas exclusivas en una plataforma líder mundial.</p>
  </article>

  <article class="card">
    <img src="https://upload.wikimedia.org/wikipedia/commons/1/17/HBO_Max_Logo.svg" alt="HBO Max" />
    <h3>HBO Max</h3>
    <div class="price">L80</div>
    <p>Disfruta contenido premium de Warner Bros, DC, y mucho más.</p>
  </article>

  <article class="card">
    <img src="https://upload.wikimedia.org/wikipedia/commons/f/f1/Prime_Video.png" alt="Prime Video" />
    <h3>Prime Video</h3>
    <div class="price">L80</div>
    <p>Explora un catálogo extenso con estrenos y clásicos del cine y TV.</p>
  </article>

  <article class="card">
    <img src="https://upload.wikimedia.org/wikipedia/commons/3/3e/Disney%2B_logo.svg" alt="Disney+" />
    <h3>Disney+</h3>
    <div class="price">L130</div>
    <p>Los mejores universos de Disney, Marvel, Star Wars y Pixar a tu alcance.</p>
  </article>

  <article class="card">
    <img src="star.png" alt="Star+" />
    <h3>Star+</h3>
    <div class="price">L130</div>
    <p>Series y películas exclusivas para toda la familia y adultos.</p>
  </article>

  <article class="card">
    <img src="paramount.png" alt="Paramount+" />
    <h3>Paramount+</h3>
    <div class="price">L80</div>
    <p>Grandes franquicias, noticias y deportes en vivo.</p>
  </article>
</div>

<button class="btn-cta">¡Suscríbete Ya!</button>

<footer>
  © 2025 TuPortalStreaming.com - Todos los derechos reservados
</footer>

</body>
</html>
