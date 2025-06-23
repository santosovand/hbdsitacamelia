
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
      background: linear-gradient(135deg, #6a9ff8,   #a68df5);
      color: white;
      padding: 30px 20px;
      text-align: center;
      max-width: 800px;
      margin: 30px auto; /* posisi tengah */
      border-radius: 16px;
      box-shadow: 0 6px 20px rgba(0, 0, 0, 0.25);
      transition: all 0.5s ease-in-out;
    }

    .love {
      color: #ff69b4;
    }

    .container {
      background: linear-gradient(135deg, #6a9ff8, #a68df5);
  padding: 25px;
  color: white;
  border-radius: 16px;
  box-shadow: 0 4px 16px rgba(0, 0, 0, 0.2);
  margin-top: 30px;
  text-align: center;
  font-size: 1.1em;
  animation: fadeInUp 1s ease forwards;
    }

    .slideshow {
  position: relative;
  width: 100%;
  max-width: 800px;
  aspect-ratio: 4 / 3; /* atau 16 / 9 sesuai bentuk gambar kamu */
  margin: 40px auto;
  border-radius: 12px;
  overflow: hidden;
  background: #eee; /* fallback agar gak putih kosong saat loading */
}

.slideshow .slide {
  position: absolute;
  width: 100%;
  height: 100%;
  object-fit: cover;
  opacity: 0;
  transition: opacity 1s ease-in-out;
  z-index: 0;
  top: 0;
  left: 0;
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
    @keyframes fadeInUp {
  from {
    opacity: 0;
    transform: translateY(30px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
     }
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

<!-- Musik -->
<audio id="bgm" autoplay loop>
  <source <source src="Nadhif_Basalamah_-_bergema_sampai_selamanya__Official_Lyric_Video_(128k).mp3" type="audio/mpeg">
  Browser kamu tidak mendukung pemutar musik.
</audio>


  <header>
    <h1>Selamat Ulang Tahun ke-18 <span class="love">Sita Camelia Azzahra</span> 🎉</h1>
  </header>

  <div class="container">
    <p>
      Di usia baru ini, aku ingin mengucapkan selamat ulang tahun yang paling tulus untukmu.<br><br>
      Semoga segala doamu dikabulkan oleh Allah, terutama harapanmu untuk masuk ke universitas impianmu.<br>
      Di usia 18 ini, semoga kamu menjadi pribadi yang lebih dewasa, kuat, dan penuh semangat dalam menggapai cita-cita.
      Jangan takut bermimpi besar, karena kamu layak mendapatkan yang terbaik.<br><br>
      Dari aku yang selalu mendoakanmu dengan tulus.
      Maaf jika selama ini aku sering membuatmu terluka.
Aku tahu, sikap dan perkataanku kadang tak seperti yang seharusnya — bukan karena aku tak sayang, tapi karena aku terlalu takut kehilanganmu.

Ada kalanya aku merasa tidak disayang, terlalu cepat berprasangka, dan akhirnya bertindak berdasarkan sakit hati yang kupendam sendiri.
Mungkin aku mencoba membalas, padahal yang aku butuhkan sebenarnya adalah pelukan dan pengertian darimu.

Aku sadar, itu bukan cara yang benar mencintaimu.
Aku seharusnya melindungi hatimu, bukan justru menyakitinya.
Aku minta maaf, dari hati yang benar-benar ingin berubah.

Aku ingin memperbaiki semuanya, bukan sekadar meminta maaf lalu mengulanginya lagi.
Aku ingin jadi seseorang yang lebih dewasa — yang mencintaimu dengan sabar, dengan percaya, dan dengan hati yang tidak mudah goyah.

Terima kasih karena masih bersamaku.
Maaf untuk luka-luka kecil yang mungkin terasa besar.
Hari ini, aku hanya ingin kamu tahu:
Aku sungguh menyayangimu. Dan aku minta maaf.
<br>
      <strong>Van Danu</strong>
    </p>

    <h2 style="text-align:center;">📸♥️🫶🏻 Kenangan Manis Kita</h2>
  <div class="slideshow">
      <img class="slide active" src="foto8.jpg" alt="Foto 8" />
      <img class="slide" src="foto5.jpg" alt="Foto 5" />
      <img class="slide" src="foto6.jpg" alt="Foto 6" />
    <img class="slide" src="foto1.jpg" alt="Foto 1" /> 
     <img class="slide" src="foto9.jpg" alt="Foto 9" />
    <img class="slide" src="foto10.jpg" alt="Foto 10" />
    <img class="slide" src="Foto7.jpg" alt="Foto 7" />
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
        setTimeout(showSlides, 3500);
      }

      showSlides();
    });
  </script>

</body>
</html>
