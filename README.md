<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Website Dalam Pemeliharaan</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600&display=swap" rel="stylesheet" />
  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: 'Inter', sans-serif;
      background: linear-gradient(135deg, #f2f4f8, #dbe4f0);
      display: flex;
      justify-content: center;
      align-items: center;
      min-height: 100vh;
      padding: 20px;
    }

    .container {
      background: #fff;
      padding: 40px 30px;
      border-radius: 20px;
      box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
      text-align: center;
      max-width: 520px;
      width: 100%;
      animation: fadeIn 1.2s ease;
    }

    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }

    .emoji {
      font-size: 60px;
      margin-bottom: 15px;
    }

    h1 {
      font-size: 26px;
      color: #e74c3c;
      margin-bottom: 15px;
    }

    p {
      font-size: 16px;
      color: #333;
      margin-bottom: 10px;
      line-height: 1.5;
    }

    #countdown {
      font-size: 28px;
      font-weight: 600;
      color: #2c3e50;
      margin-top: 25px;
    }

    .social {
      font-size: 14px;
      color: #666;
      margin-top: 25px;
    }

    .icons {
      margin-top: 10px;
    }

    .icons a {
      margin: 0 8px;
      color: #666;
      text-decoration: none;
      font-size: 20px;
      transition: color 0.3s;
    }

    .icons a:hover {
      color: #3498db;
    }

    @media (min-width: 768px) {
      h1 {
        font-size: 30px;
      }

      p {
        font-size: 18px;
      }

      .emoji {
        font-size: 70px;
      }

      #countdown {
        font-size: 32px;
      }
    }
  </style>
  <script>
    document.addEventListener("DOMContentLoaded", () => {
      const targetTime = new Date().getTime() + 5 * 60 * 60 * 1000;
      const countdownElement = document.getElementById("countdown");

      const updateCountdown = () => {
        const now = new Date().getTime();
        const distance = targetTime - now;

        if (distance < 0) {
          countdownElement.textContent = "00:00:00";
          clearInterval(interval);
          return;
        }

        const hours = Math.floor(distance / (1000 * 60 * 60));
        const minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
        const seconds = Math.floor((distance % (1000 * 60)) / 1000);

        countdownElement.textContent =
          hours.toString().padStart(2, '0') + ':' +
          minutes.toString().padStart(2, '0') + ':' +
          seconds.toString().padStart(2, '0');
      };

      const interval = setInterval(updateCountdown, 1000);
      updateCountdown();
    });
  </script>
</head>
<body>
  <div class="container">
    <div class="emoji">🔧</div>
    <h1>Website Dalam Pemeliharaan</h1>
    <p>Mohon maaf atas ketidaknyamanan ini. Kami sedang melakukan <strong>pemeliharaan sistem</strong> untuk meningkatkan kualitas layanan.</p>
    <p>⏳ Harap bersabar, website akan kembali dapat diakses dalam waktu:</p>
    <div id="countdown">00:00:00</div>
    <div class="social">
      📢 Dapatkan pembaruan melalui media sosial kami:
      <div class="icons">
        <a href="https://instagram.com/namabrand" target="_blank">📷</a>
        <a href="https://twitter.com/namabrand" target="_blank">🐦</a>
        <a href="https://facebook.com/namabrand" target="_blank">📘</a>
      </div>
    </div>
  </div>
</body>
</html> Teknologi • Kreativitas</p>
  </section>

  <div class="marquee-container" id="marquee">
    <div class="marquee-text">
      Selamat Datang di CarlandsCompanyID! Hai, Sobat Carlanders! 👋 Terima kasih sudah bergabung bersama kami...
    </div>
  </div>

  <section>
    <h2>🎯 Misi Kami</h2>
    <p>Mengembangkan game berkualitas tinggi dengan cerita, gameplay, dan fitur yang orisinal serta menarik bagi berbagai kalangan.
       Mendukung kreativitas dan talenta lokal dalam industri game melalui kolaborasi, pelatihan, dan pengembangan tim internal.
       Membangun komunitas game yang inklusif dan sehat, di mana pemain merasa dihargai, aman, dan memiliki ruang untuk berekspresi.
       Menggunakan teknologi terbaru untuk menciptakan pengalaman bermain yang responsif, realistis, dan inovatif.
       Mewujudkan pertumbuhan berkelanjutan baik dari sisi produk maupun kontribusi terhadap industri kreatif di Indonesia.</p>
    <h2>🚀 Apa yang Kami Tawarkan</h2>
    <ul class="ml-4 list-disc">
      <li>🌟 Pengembangan Game & Roleplay Server</li>
      <li>💼 Layanan Digital & Kreatif</li>
      <li>🛠️ Inovasi Teknologi Masa Depan</li>
    </ul>
    <h2>🤝 Bergabunglah Bersama Kami</h2>
    <p>🎮 Gabung Bersama CarlandsCompanyID! 🚀
          Apakah kamu punya semangat untuk menciptakan dunia game yang seru, inovatif, dan penuh tantangan?
          Di CarlandsCompanyID, kami bukan hanya membuat game — kami membangun pengalaman, komunitas, dan masa depan industri game Indonesia!
         ✨ Mengapa bergabung dengan kami?
         Lingkungan kreatif dan kolaboratif
         Proyek game yang seru dan penuh potensi
         Kesempatan berkembang bersama tim profesional
         Dukungan penuh untuk ide dan inovasi kamu
  💡 Baik kamu developer, desainer, storyteller, content creator, atau gamers yang ingin berkarya — ini saatnya kamu ambil peran!
  📩 Yuk, kirim portofolio atau kenalan dulu dengan tim kami!
  📍 Temukan info lengkap di [website/link komunitas]
  📱 Atau DM kami langsung di [Instagram/Discord/WhatsApp]
  Bersama CarlandsCompanyID, wujudkan game impianmu!
  #CarlandsCompanyID #GameDeveloperIndonesia #JoinUs #Carlandsantipungli</p>
  </section>

  <div class="form-section text-center my-4">
    <h2 class="mb-2">📝 Pendaftaran Akun Pencoblosan [OPEN]</h2>
    <a href="https://forms.gle/1iyHNtXXghsjmqc9A" class="form-button" target="_blank">Buka Formulir</a>
  </div>

  <div class="social-buttons text-center">
    <h2 class="text-2xl font-semibold mb-4">Temukan CarlandsCompany</h2>
    <a href="https://www.youtube.com/@carlandsid" class="youtube"><i data-lucide="youtube"></i> YouTube</a>
    <a href="https://www.instagram.com/carlandscompanyid/" class="instagram"><i data-lucide="instagram"></i> Instagram</a>
    <a href="https://www.tiktok.com/@carlandscompanyid" class="tiktok"><i data-lucide="music"></i> TikTok</a>
    <a href="https://discord.com/invite/tnzfy7tSVS" class="discord"><i data-lucide="message-circle"></i> Discord</a>
    <a href="https://chat.whatsapp.com/EoyF4WTKUHB1feKjRdowss" class="whatsapp"><i data-lucide="phone"></i> WhatsApp</a>
  </div>

  <section class="text-center">
    <h2 class="text-xl font-semibold my-4">Jam Digital Seluruh Indonesia</h2>
    <div class="clock" id="wib">WIB (Jakarta): </div>
    <div class="clock" id="wita">WITA (Makassar): </div>
    <div class="clock" id="wit">WIT (Jayapura): </div>
  </section>

  <section id="contact" class="text-center">
    <h2 class="text-xl font-semibold mb-2">Kontak Kami</h2>
    <p>Hai, butuh bantuan atau ingin bekerja sama dengan <strong>CarlandsCompanyID</strong>? Kami menunggu kabar darimu!</p>
    <p><strong>Email Utama:</strong></p>
    <a href="mailto:carlandscompanyid@gmail.com" class="text-blue-600 underline">carlandscompanyid@gmail.com</a>
    <p class="mt-4">Jangan ragu untuk mengirimkan pertanyaan, saran, atau sekadar menyapa. Kami akan membalas secepat mungkin!</p>
  </section>

  <div class="status">
    <div class="dot online"></div>
    <span>Sedang Online</span>
  </div>

  <div class="warning mx-4 my-6 text-center text-sm">
    <strong>⚠️ Peringatan:</strong> Ini adalah <strong>situs resmi</strong> milik CarlandsCompanyID. Situs selain <code>carlandscompanyid</code> adalah <strong>tidak resmi atau palsu</strong>.
  </div>

  <footer class="py-6 text-sm">
    &copy; 2025 CarlandsCompanyID. Semua Hak Dilindungi.
    <p id="last-updated" class="mt-2">Terakhir diperbarui: <span id="update-time"></span></p>
  </footer>

  <script>
    lucide.createIcons();

    function dapatkanSapaanFormal() {
      const jam = new Date().getHours();
      return jam < 11 ? "Selamat pagi!" :
             jam < 15 ? "Selamat siang!" :
             jam < 18 ? "Selamat sore!" : "Selamat malam!";
    }
    document.getElementById('sapaan').textContent = dapatkanSapaanFormal();

    const marquee = document.getElementById('marquee');
    marquee.addEventListener('touchstart', () => {
      marquee.querySelector('.marquee-text').classList.toggle('paused');
    });

    function updateIndonesianClocks() {
      const now = new Date();
      const options = {
        hour: '2-digit',
        minute: '2-digit',
        second: '2-digit',
        hour12: false
      };

      document.getElementById("wib").textContent =
        "WIB (Jakarta): " + now.toLocaleTimeString("id-ID", { ...options, timeZone: "Asia/Jakarta" });

      document.getElementById("wita").textContent =
        "WITA (Makassar): " + now.toLocaleTimeString("id-ID", { ...options, timeZone: "Asia/Makassar" });

      document.getElementById("wit").textContent =
        "WIT (Jayapura): " + now.toLocaleTimeString("id-ID", { ...options, timeZone: "Asia/Jayapura" });
    }

    setInterval(updateIndonesianClocks, 1000);
    updateIndonesianClocks();

    const updateTime = new Date();
    document.getElementById("update-time").textContent = updateTime.toLocaleString("id-ID");
  </script>

</body>
</html>
