<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Selamat Ulang Tahun Sita</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background: linear-gradient(135deg, #d0e8ff, #f5e1ff, #fff0f5);
      color: #333;
      overflow-x: hidden;
    }

    header {
      background-color: #4682B4;
      color: white;
      padding: 20px;
      text-align: center;
    }

    .love {
      color: #ff69b4;
    }

    .container {
      padding: 20px;
      max-width: 800px;
      margin: auto;
    }

    .slideshow {
      position: relative;
      width: 100%;
      max-width: 800px;
      height: 400px;
      margin: 40px auto;
      border-radius: 12px;
      overflow: hidden;
    }

 .slideshow .slide {
      position: absolute;
      width: 100%;
      height: 100%;
      object-fit: cover;
      opacity: 0;
      transition: opacity 1s ease-in-out;
      z-index: 0;
    }

    .slideshow .slide.active {
      opacity: 1;
      z-index: 1;
    }

    footer {
      text-align: center;
      padding: 20px;
      font-size: 0.9em;
      color: #555;
    }

    /* Hiasan love jatuh */
    @keyframes fall {
      to {
        transform: translateY(100vh) rotate(360deg);
        opacity: 0;
      }
    }

    .heart {
      position: fixed;
      top: -50px;
      font-size: 24px;
      color: pink;
      animation: fall linear infinite;
    }
  </style>
</head>
<body>

  <header>
    <h1>Selamat Ulang Tahun ke-18 <span class="love">Sita Camelia Azzahra</span> 🎉</h1>
  </header>

  <div class="container">
    <p>
      Di usia baru ini, aku ingin mengucapkan selamat ulang tahun yang paling tulus untukmu.<br><br>
      Semoga segala doamu dikabulkan oleh Allah, terutama harapanmu untuk masuk ke universitas impianmu.<br>
      Di usia 18 ini, semoga kamu menjadi pribadi yang lebih dewasa, kuat, dan penuh semangat dalam menggapai cita-cita.
      Jangan takut bermimpi besar, karena kamu layak mendapatkan yang terbaik.<br><br>
      Dari aku yang selalu mendoakanmu dengan tulus,<br>
      <strong>Van Danu</strong>
    </p>

    <h2 style="text-align:center;">📸 Kenangan Manis Kita</h2>
  <div class="slideshow">
      <img class="slide active" src="foto8.jpg" alt="Foto 8" />
      <img class="slide" src="foto5.jpg" alt="Foto 5" />
      <img class="slide" src="foto6.jpg" alt="Foto 6" />
    <img class="slide" src="foto1.jpg" alt="Foto 1" /> 
     <img class="slide" src="foto9.jpg" alt="Foto 9" />
    </div>
  </div>

  <footer>
    Dibuat dengan <span class="love">&#10084;</span> oleh Van Danu untuk Sita - 30 Juni 2025
  </footer>

  <!-- Musik -->
  <audio autoplay loop hidden>
    <source src="https://cdn.pixabay.com/download/audio/2022/03/15/audio_3db4cc90d7.mp3?filename=romantic-melody-11743.mp3" type="audio/mpeg">
    Browser kamu tidak mendukung pemutar musik.
  </audio>

  <!-- Efek love jatuh -->
  <script>
    function createHeart() {
      const colors = ["#ff4d4d", "#ff66cc", "#ffcc00", "#66ff66", "#66ccff", "#9966ff"];
      const heart = document.createElement("div");
      heart.className = "heart";
      heart.style.left = Math.random() * 100 + "vw";
      heart.style.animationDuration = (Math.random() * 2 + 3) + "s";
      heart.style.color = colors[Math.floor(Math.random() * colors.length)];
      heart.innerText = "❤";
      document.body.appendChild(heart);
      setTimeout(() => heart.remove(), 5000);
    }
    setInterval(createHeart, 300);
  </script>

  <!-- Slideshow JS -->
  <script>
    window.addEventListener('load', function () {
      let slideIndex = 0;
      const slides = document.querySelectorAll('.slideshow .slide');

      function showSlides() {
        slides.forEach(slide => slide.classList.remove('active'));
        slides[slideIndex].classList.add('active');
        slideIndex = (slideIndex + 1) % slides.length;
        setTimeout(showSlides, 7000);
      }

      showSlides();
    });
  </script>

</body>
</html>
