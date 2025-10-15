<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>My Kind of Woman 💖</title>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Great+Vibes&display=swap');

  body {
    margin: 0;
    padding: 0;
    background: radial-gradient(circle at center, #111 0%, #000 100%);
    overflow: hidden;
    height: 100vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    color: #fff;
    font-family: 'Great Vibes', cursive;
    text-align: center;
  }

  h1 {
    font-size: 2.8em;
    color: #ffb6c1;
    text-shadow: 0 0 10px #ffb6c1, 0 0 30px #ff69b4;
    animation: pulse 3s infinite alternate;
  }

  p {
    width: 80%;
    margin: 30px auto;
    font-size: 1.6em;
    line-height: 1.8em;
    color: #fff8f8;
    text-shadow: 0 0 10px #ffb6c1;
    animation: fadeIn 4s ease forwards;
    opacity: 0.9;
  }

  @keyframes pulse {
    from { text-shadow: 0 0 10px #ffb6c1; }
    to { text-shadow: 0 0 25px #ff69b4; }
  }

  @keyframes fadeIn {
    from {opacity: 0; transform: translateY(20px);}
    to {opacity: 1; transform: translateY(0);}
  }

  .foto {
    width: 250px;
    height: 250px;
    border-radius: 20px;
    border: 3px solid #ffb6c1;
    box-shadow: 0 0 20px #ff69b4;
    object-fit: cover;
    margin-bottom: 20px;
    animation: pulse 4s infinite alternate;
  }

  .heart, .sparkle {
    position: absolute;
    opacity: 0.8;
    pointer-events: none;
  }

  .heart {
    color: #ff69b4;
    font-size: 25px;
    animation: float 8s linear infinite;
  }

  .sparkle {
    color: #ffe4e1;
    font-size: 15px;
    animation: float 6s linear infinite;
  }

  @keyframes float {
    0% { transform: translateY(100vh) scale(1); opacity: 0; }
    20% { opacity: 1; }
    100% { transform: translateY(-10vh) scale(1.5); opacity: 0; }
  }
</style>
</head>
<body>
  <h1>💌 Para ti, mi amor 💌</h1>

  <img src="foto.png" alt="Nuestra foto" class="foto">

  <p>
  Aunque estemos lejos, siento tu presencia en cada instante.  
  Tu voz, tus risas, tus palabras — todo se queda conmigo.  
  Eres mi paz, mi refugio, y la razón por la que cada día sonrío.  
  <br><br>
  No hay distancia que apague lo que siento.  
  Esta canción es mi manera de decirte que te amo,  
  que eres y siempre serás...  
  <br><br>
  ✨ <strong>My kind of woman.</strong> 💖  
  </p>

  <audio autoplay loop>
    <source src="https://dl.dropboxusercontent.com/scl/fi/awq5u3j23k9s0x6c7d4mt/MyKindOfWoman.mp3?rlkey=smw7a2cb7zkp7fd3fsvd2u9q4&dl=0" type="audio/mp3">
  </audio>

  <script>
    function createElement(symbol, className, count) {
      for (let i = 0; i < count; i++) {
        let el = document.createElement('div');
        el.innerHTML = symbol;
        el.classList.add(className);
        el.style.left = Math.random() * 100 + 'vw';
        el.style.animationDuration = 5 + Math.random() * 7 + 's';
        el.style.fontSize = 15 + Math.random() * 20 + 'px';
        document.body.appendChild(el);
      }
    }

    createElement('❤️', 'heart', 25);
    createElement('✨', 'sparkle', 20);

    document.addEventListener('mousemove', e => {
      document.body.style.backgroundPositionX = e.clientX / 40 + 'px';
      document.body.style.backgroundPositionY = e.clientY / 40 + 'px';
    });
  </script>
</body>
</html>
