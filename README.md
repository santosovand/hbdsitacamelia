# hbdsitacamelia
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Selamat Ulang Tahun Sita</title>
<style>
.slideshow {
  max-width: 100%;
  height: auto;
  position: relative;
  margin-top: 30px;
  overflow: hidden;
  border-radius: 12px;
}

.slideshow .slide {
  position: absolute;
  width: 100%;
  opacity: 0;
  transition: opacity 1.5s ease-in-out;
  object-fit: cover;
  border-radius: 12px;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
}

.slideshow .active {
  opacity: 1;
  z-index: 2;
}
</style>
}
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
    .gallery {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(120px, 1fr));
  gap: 12px;
  margin-top: 20px;
}

.gallery img {
  width: 100%;
  aspect-ratio: 1 / 1;
  object-fit: cover;
  border-radius: 12px;
  box-shadow: 0 3px 10px rgba(0, 0, 0, 0.15);
}
    footer {
      text-align: center;
      padding: 20px;
      font-size: 0.9em;
      color: #555;
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
      color: pink;
      animation: fall linear infinite;
    }
  </style>
</head>
<body>
  <header>
    <!-- Tombol Musik --> 
    <button onclick="document.getElementById('bgm').play()" style="
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
">🎵 Putar Musik</button>

<!-- Pemutar Musik -->
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
      <img class="slide active" src="foto1.jpg" alt="Foto 1" />
      <img class="slide" src="foto5.jpg" alt="Foto 5" />
      <img class="slide" src="foto6.jpg" alt="Foto 6" />
      <img class="slide" src="foto8.jpg" alt="Foto 8" />
      <img class="slide" src="Foto7.jpg" alt="Foto 7" />
      <img class="slide" src="foto9.jpg" alt="Foto 9" />
      <img class="slide" src="foto10.jpg" alt="Foto 10" />
    </div>
  </div>
  <footer>
    Dibuat dengan <span class="love">&#10084;</span> oleh Van Danu untuk Sita - 30 Juni 2025
  </footer>

  <audio autoplay loop hidden>
    <source src="https://cdn.pixabay.com/download/audio/2022/03/15/audio_3db4cc90d7.mp3?filename=romantic-melody-11743.mp3" type="audio/mpeg">
    Browser kamu tidak mendukung pemutar musik.
  </audio>

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
<script>
  let slideIndex = 0;
  const slides = document.querySelectorAll('.slideshow .slide');

  function showSlides() {
    slides.forEach((slide, index) => {
      slide.classList.remove("active");
    });

    slideIndex = (slideIndex + 1) % slides.length;
    slides[slideIndex].classList.add("active");
    setTimeout(showSlides, 7000); // 7 detik
  }

  slides[0].classList.add("active"); // tampilkan slide pertama saat awal
  setTimeout(showSlides, 7000);
</script>
</body>
</html>
