# hbdsitacamelia
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
      background: linear-gradient(to bottom, #d0e8ff, #ffffff);
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
      grid-template-columns: repeat(auto-fill, minmax(150px, 1fr));
      gap: 10px;
      margin-top: 20px;
    }
    .gallery img {
      width: 100%;
      border-radius: 15px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
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
    <div class="gallery">
      <img src="foto1.jpg" alt="Foto 1" />
      <img src="foto2.jpg" alt="Foto 2" />
      <img src="foto3.jpg" alt="Foto 3" />
      <img src="foto4.jpg" alt="Foto 4" />
      <img src="foto5.jpg" alt="Foto 5" />
      <img src="foto6.jpg" alt="Foto 6" />
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
      const heart = document.createElement("div");
      heart.className = "heart";
      heart.style.left = Math.random() * 100 + "vw";
      heart.style.animationDuration = (Math.random() * 2 + 3) + "s";
      heart.innerText = "❤";
      document.body.appendChild(heart);
      setTimeout(() => heart.remove(), 5000);
    }
    setInterval(createHeart, 300);
  </script>
</body>
</html>
