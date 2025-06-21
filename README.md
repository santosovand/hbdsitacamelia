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

    .container {
      padding: 20px;
      max-width: 800px;
      margin: auto;
    }

    .love {
      color: #ff69b4;
    }

    footer {
      text-align: center;
      padding: 20px;
      font-size: 0.9em;
      color: #555;
    }

    .slideshow {
      position: relative;
      width: 100%;
      max-width: 800px;
      margin: 40px auto;
      border-radius: 12px;
      overflow: hidden;
    }

    .slideshow .slide {
      position: absolute;
      width: 100%;
      opacity: 0;
      transition: opacity 1.5s ease-in-out;
      object-fit: cover;
      border-radius: 12px;
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.2);
    }

    .slideshow .slide.active {
      opacity: 1;
      z-index: 1;
    }

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
      animation: fall linear infinite;
      z-index: 999;
    }

    /* Tombol Musik */
    #playMusic {
      position: fixed;
      top: 10px;
      right: 10px;
      padding: 10px 15px;
      background: #ff69b4;
      color: white;
      border: none;
      border-radius: 10px;
      box-shadow: 0 2px 6px rgba(0,0,0,0.2);
      font-size: 16px;
      z-index: 9999;
    }
  </style>
</head>
<body>
  <header>
    <button id="playMusic" onclick="document.getElementById('bgm').play()">🎵 Putar Musik</button>
    <audio id="bgm" loop>
      <source src="Nadhif_Basalamah_-_bergema_sampai_selamanya__Official_Lyric_Video_(128k).mp3" type="audio/mpeg" />
      Browser kamu tidak mendukung audio.
    </audio>
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
      <img class="slide.active" src="foto1.jpg" alt="Foto 1" />
      <img class="slide" src="foto5.jpg" alt="Foto 5" />
      <img class="slide" src="foto6.jpg" alt="Foto 6" />
      <img class="slide" src="foto8.jpg" alt="Foto 8" />
      <img class="slide" src="Foto7.jpg" alt="Foto 7" />
      <img class="slide" src="foto9.jpg" alt="Foto 9" />
      <img class="slide" src="foto10.jpg" alt="Foto 10" />
</div>

<footer>
    Dibuat dengan <span class="love">&#10084;</span> oleh Van Danu untuk Sita - 30 Juni 2025
</footer>

  <!-- Musik Otomatis Alternatif (jika mau auto tanpa tombol) -->
  <!--
  <audio autoplay loop hidden>
    <source src="https://cdn.pixabay.com/download/audio/2022/03/15/audio_3db4cc90d7.mp3?filename=romantic-melody-11743.mp3" type="audio/mpeg">
    Browser kamu tidak mendukung pemutar musik.
  </audio>
  -->

  <script>
    // Efek Hati Warna-warni
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
<script>
  let slideIndex = 0;
  const slides = document.querySelectorAll(".slideshow .slide");

  function showSlides() {
    slides.forEach((slide, i) => {
      slide.classList.remove("active");
    });

    slides[slideIndex].classList.add("active");

    slideIndex = (slideIndex + 1) % slides.length;
    setTimeout(showSlides, 7000); // Ganti setiap 7 detik
  }

  window.onload = function () {
    showSlides();
  };
</script>
<script>
  window.onload = function () {
    let slideIndex = 0;
    const slides = document.querySelectorAll(".slideshow .slide");

    function showSlides() {
      slides.forEach(slide => slide.classList.remove("active"));
      slides[slideIndex].classList.add("active");
      slideIndex = (slideIndex + 1) % slides.length;
      setTimeout(showSlides, 7000);
    }

    showSlides();
  };
</script>
</body>
</html>
