<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Feliz Cumpleaños Marisol</title>

  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;500;700&display=swap" rel="stylesheet">

  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      font-family: 'Poppins', sans-serif;
      background: black;
      overflow: hidden;
    }

    .slide {
      position: fixed;
      inset: 0;
      background-size: cover;
      background-position: center;
      display: none;
    }

    .overlay {
      position: absolute;
      inset: 0;
      background: rgba(0,0,0,0.55);
      display: flex;
      justify-content: center;
      align-items: center;
      padding: 32px 20px;
      text-align: center;
    }

    .text {
      color: white;
      font-size: 15px;
      line-height: 1.7;
      max-width: 95%;
      animation: fadeUp 1.2s ease;
    }

    @keyframes fadeUp {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }
  </style>
</head>
<body>

<!-- SLIDE 1 -->
<div class="slide" style="background-image:url('imagen1.jpg')">
  <div class="overlay"><div class="text">
    Querida Marisol, bueno futura profesora xddd. El día de hoy no me olvidé de tu cumpleaños, más bien esperé a que sea un momento más lindo para poder enviarte esto.
  </div></div>
</div>

<!-- SLIDE 2 -->
<div class="slide" style="background-image:url('imagen2.jpg')">
  <div class="overlay"><div class="text">
    Quería decirte gracias por muchas cosas: por ayudarme en algunos momentos donde sufría ataques de ansiedad y por orientarme cuando tenía dudas sobre mi futuro. Me da gusto haber pasado este año contigo.
  </div></div>
</div>

<!-- SLIDE 3 -->
<div class="slide" style="background-image:url('imagen3.jpg')">
  <div class="overlay"><div class="text">
    Tú ahora graduándote y convirtiéndote en un alma mater, y yo pisando una nueva etapa de fósil xddd. Gracias también porque por tu culpa conocí a tu hermana, que es una gran persona.
  </div></div>
</div>

<!-- SLIDE 4 -->
<div class="slide" style="background-image:url('imagen4.jpg')">
  <div class="overlay"><div class="text">
    Aunque hoy me hice el tonto diciendo que me había olvidado, en realidad solo esperaba el momento perfecto para escribirte esto y agradecerte todo lo que hiciste por mí; más que una practicante fuiste una guía de verdad.
  </div></div>
</div>

<!-- SLIDE 5 FINAL -->
<div class="slide" style="background-image:url('imagen4.jpg')">
  <div class="overlay"><div class="text">
    Feliz cumpleaños, Marisol, gracias por tu apoyo, tu paciencia y por marcar de forma tan bonita esta etapa de mi vida.
  </div></div>
</div>

<script>
  const slides = document.querySelectorAll('.slide');
  let index = 0;

  function showSlide() {
    slides.forEach(s => s.style.display = 'none');
    slides[index].style.display = 'block';
    index = (index + 1) % slides.length;
  }

  showSlide();
  setInterval(showSlide, 6500);
</script>
<!-- IMAGEN 1 -->
<div class="slide" style="background-image:url('imagen1.jpeg')">

<!-- IMAGEN 2 -->
<div class="slide" style="background-image:url('imagen2.jpeg')">

<!-- IMAGEN 3 -->
<div class="slide" style="background-image:url('imagen3.jpeg')">

<!-- IMAGEN 4 (FINAL) -->
<div class="slide" style="background-image:url('imagen4.jpeg')">
</body>
</html>
