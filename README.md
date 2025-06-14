<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>CarlandsCompanyID - Website Resmi</title>
  <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.2.19/dist/tailwind.min.css" rel="stylesheet">
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&display=swap" rel="stylesheet">
  <script src="https://unpkg.com/lucide@latest"></script>
  <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">
  <style>
    :root {
      --primary-color: #003366;
      --secondary-color: #4285F4;
      --accent-color: #FFD700;
      --text-color: #333;
      --background-color: #f4f4f4;
      --glass-bg: rgba(255, 255, 255, 0.1);
      --glass-border: rgba(255, 255, 255, 0.2);
    }

    body {
      margin: 0;
      font-family: 'Poppins', sans-serif;
      background-color: var(--background-color);
      color: var(--text-color);
      line-height: 1.6;
      overflow-x: hidden; /* Mencegah scroll horizontal akibat animasi */
    }

    /* Dark mode untuk bagian NeoLux dan sisanya */
    body.dark-mode {
      background: linear-gradient(to right, #000000, #1f1f1f);
      color: #fff;
    }
    body.dark-mode header, body.dark-mode footer {
      background-color: #1a1a1a;
      color: #eee;
    }
    body.dark-mode section, body.dark-mode .warning {
      background: #2a2a2a;
      color: #fff;
      box-shadow: 0 4px 12px rgba(0,0,0,0.3);
    }
    body.dark-mode .social-buttons a {
      color: #eee;
    }
    body.dark-mode .form-button {
      background-color: #555;
    }
    body.dark-mode .form-button:hover {
      background-color: #777;
    }
    body.dark-mode .clock {
      background: #3a3a3a;
      color: #eee;
    }
    body.dark-mode .dot.online { background-color: #66BB6A; }
    body.dark-mode .dot.offline { background-color: #EF5350; }
    body.dark-mode .glass {
      backdrop-filter: blur(10px);
      background: rgba(255, 255, 255, 0.05);
      border: 1px solid rgba(255, 255, 255, 0.1);
    }
    body.dark-mode .text-gray-700, body.dark-mode .text-gray-500 {
      color: #ccc;
    }
    body.dark-mode a {
      color: #8ab4f8; /* Biru terang untuk tautan di dark mode */
    }


    header, footer {
      background-color: var(--primary-color);
      color: #fff;
      text-align: center;
      padding: 1rem 0;
    }
    section, .warning {
      max-width: 900px;
      margin: 2rem auto;
      background: #fff;
      padding: 2rem;
      border-radius: 10px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.1);
    }

    .social-buttons a {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      gap: 0.5rem;
      margin: 0.5rem;
      padding: 0.75rem 1rem;
      border-radius: 8px;
      font-weight: bold;
      color: #fff;
      transition: transform 0.3s ease, opacity 0.3s ease;
    }
    .social-buttons a:hover {
      transform: translateY(-5px);
      opacity: 0.9;
    }
    .youtube { background: #FF0000; }
    .instagram { background: #C13584; }
    .tiktok { background: #010101; }
    .discord { background: radial-gradient(circle at top left, #5865F2, #404EED); }
    .whatsapp { background: #25D366; }

    .form-button {
      display: inline-block;
      padding: 0.75rem 1.5rem;
      background-color: var(--secondary-color);
      color: white;
      border-radius: 6px;
      transition: background-color .3s ease, transform 0.2s ease;
    }
    .form-button:hover {
      background-color: #3367D6;
      transform: translateY(-2px);
    }

    /* Animasi */
    .fade-in {
      animation: fadeIn 1.5s ease-in-out forwards;
      opacity: 0;
    }
    @keyframes fadeIn {
      to { opacity: 1; }
    }

    .marquee-container {
      width: 100%;
      overflow: hidden;
      background: #121212;
      padding: 20px 0;
      border-top: 1px solid #333;
      border-bottom: 1px solid #333;
    }
    .marquee-text {
      display: inline-block;
      white-space: nowrap;
      font-size: 18px;
      font-weight: 400;
      background: linear-gradient(90deg, #00f7ff, #865dff, #ff5ea5, #00f7ff);
      background-size: 400% auto;
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      animation: scroll 60s linear infinite, gradientShift 12s ease-in-out infinite;
      text-shadow: 0 0 4px rgba(255,255,255,0.05);
      padding-left: 100%; /* Mulai dari luar layar */
    }
    @keyframes scroll {
      from { transform: translateX(0); }
      to { transform: translateX(-100%); }
    }
    @keyframes gradientShift {
      0%   { background-position: 0% 50%; }
      50%  { background-position: 100% 50%; }
      100% { background-position: 0% 50%; }
    }
    .marquee-container:hover .marquee-text,
    .paused {
      animation-play-state: paused !important;
    }

    .clock {
      background: #ffffff;
      padding: 20px;
      margin: 10px auto;
      width: 90%;
      max-width: 300px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
      border-radius: 10px;
      font-size: 1.2em;
      text-align: center;
    }
    @media (min-width: 768px) {
      .clock-grid {
        display: grid;
        grid-template-columns: repeat(3, 1fr);
        gap: 20px;
        max-width: 900px;
        margin: 2rem auto;
      }
      .clock {
        margin: 0;
        width: auto;
      }
    }

    .status {
      display: flex;
      align-items: center;
      font-size: 16px;
      font-family: Arial, sans-serif;
      justify-content: center;
      margin: 20px auto;
    }
    .dot {
      height: 12px;
      width: 12px;
      border-radius: 50%;
      margin-right: 8px;
    }
    .online { background-color: #4CAF50; }
    .offline { background-color: #f44336; }

    /* Gaya Spesifik NeoLux */
    .neolux-section {
      background: linear-gradient(to right, #000000, #1f1f1f);
      color: #fff;
      padding: 4rem 1rem;
      text-align: center;
    }
    .neolux-header {
      font-size: 3.5rem; /* Setara dengan text-6xl */
      font-weight: bold;
      color: var(--accent-color);
      animation: pulse 2s infinite ease-in-out;
    }
    @keyframes pulse {
      0%, 100% { opacity: 1; }
      50% { opacity: 0.7; }
    }
    .neolux-subheader {
      font-size: 1.25rem; /* Setara dengan text-xl */
      color: #ccc;
      margin-top: 0.5rem;
    }
    .neolux-card-grid {
      display: grid;
      grid-template-columns: 1fr;
      gap: 1.5rem;
      max-width: 1200px;
      margin: 3rem auto;
    }
    @media (min-width: 768px) {
      .neolux-card-grid {
        grid-template-columns: repeat(3, 1fr);
      }
    }
    .glass {
      backdrop-filter: blur(10px);
      background: var(--glass-bg);
      border: 1px solid var(--glass-border);
      border-radius: 1rem; /* rounded-2xl */
      padding: 1.5rem; /* p-6 */
      transition: transform 0.3s ease, box-shadow 0.3s ease;
    }
    .glass:hover {
      transform: translateY(-8px);
      box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
    }
    .glass h2 {
      font-size: 1.25rem; /* text-xl */
      font-weight: 600;
      color: var(--accent-color);
    }
    .glass p {
      margin-top: 0.5rem;
      color: #eee;
    }
    .glass a {
      color: #60a5fa; /* blue-400 */
      text-decoration: underline;
    }
    .neolux-audio-button {
      background: var(--glass-bg);
      border: 1px solid var(--glass-border);
      padding: 0.5rem 1rem;
      border-radius: 9999px; /* rounded-full */
      font-size: 0.875rem; /* text-sm */
      font-weight: 600;
      color: white;
      transition: background-color 0.3s, color 0.3s, transform 0.2s;
    }
    .neolux-audio-button:hover {
      background-color: white;
      color: black;
      transform: scale(1.05);
    }

    /* Responsif Umum */
    @media (max-width: 768px) {
      .text-5xl { font-size: 2.5rem; }
      .text-2xl { font-size: 1.5rem; }
      section, .warning {
        margin: 1rem auto;
        padding: 1.5rem;
      }
      .social-buttons a {
        margin: 0.3rem;
        padding: 0.6rem 0.8rem;
        font-size: 0.9rem;
      }
    }

    @media (max-width: 480px) {
      .text-5xl { font-size: 2rem; }
      .text-2xl { font-size: 1.25rem; }
      section, .warning {
        padding: 1rem;
      }
      .social-buttons a {
        flex-direction: column;
        gap: 0.2rem;
        padding: 0.5rem;
        font-size: 0.8rem;
      }
      .social-buttons a svg {
        width: 18px;
        height: 18px;
      }
    }

    /* Tombol Dark Mode */
    .dark-mode-toggle {
        position: fixed;
        bottom: 20px;
        right: 20px;
        background-color: var(--primary-color);
        color: white;
        border: none;
        border-radius: 50%;
        width: 50px;
        height: 50px;
        display: flex;
        align-items: center;
        justify-content: center;
        font-size: 1.5rem;
        cursor: pointer;
        box-shadow: 0 4px 8px rgba(0,0,0,0.2);
        transition: background-color 0.3s, transform 0.3s;
        z-index: 1000;
    }
    .dark-mode-toggle:hover {
        background-color: #004d99;
        transform: scale(1.1);
    }
  </style>
</head>
<body>

  <header data-aos="fade-down">
    <div class="py-4">
      <h1 class="text-3xl md:text-4xl font-bold">CarlandsCompanyID</h1>
      <p class="text-sm md:text-base mt-1">Situs Resmi</p>
    </div>
  </header>

  <section class="fade-in text-center" data-aos="fade-up" data-aos-duration="1000">
    <div class="text-5xl mb-4">👋👋</div>
    <h2 id="sapaan" class="text-2xl font-semibold mb-2"></h2>
    <p class="text-gray-700 mb-4">Selamat datang di situs resmi kami. Semoga hari Anda menyenangkan dan penuh produktivitas.</p>
    <p class="text-sm text-gray-500">Dibawakan oleh <strong>CarlandsCompanyID</strong><br>Inovasi • Teknologi • Kreativitas</p>
  </section>

  <div class="marquee-container" id="marquee" data-aos="fade-left" data-aos-delay="500">
    <div class="marquee-text">
      Selamat Datang di CarlandsCompanyID! Hai, Sobat Carlanders! 👋 Terima kasih sudah bergabung bersama kami...
    </div>
  </div>

  <section data-aos="fade-right" data-aos-duration="1200">
    <h2 class="text-2xl font-semibold mb-4">🎯 Misi Kami</h2>
    <p>Mengembangkan game berkualitas tinggi dengan cerita, gameplay, dan fitur yang orisinal serta menarik bagi berbagai kalangan.
       Mendukung kreativitas dan talenta lokal dalam industri game melalui kolaborasi, pelatihan, dan pengembangan tim internal.
       Membangun komunitas game yang inklusif dan sehat, di mana pemain merasa dihargai, aman, dan memiliki ruang untuk berekspresi.
       Menggunakan teknologi terbaru untuk menciptakan pengalaman bermain yang responsif, realistis, dan inovatif.
       Mewujudkan pertumbuhan berkelanjutan baik dari sisi produk maupun kontribusi terhadap industri kreatif di Indonesia.</p>
    <h2 class="text-2xl font-semibold mt-6 mb-4">🚀 Apa yang Kami Tawarkan</h2>
    <ul class="ml-4 list-disc space-y-2">
      <li>🌟 Pengembangan Game & Roleplay Server</li>
      <li>💼 Layanan Digital & Kreatif</li>
      <li>🛠️ Inovasi Teknologi Masa Depan</li>
    </ul>
  </section>

  <section data-aos="fade-up" data-aos-duration="1200">
    <h2 class="text-2xl font-semibold mb-4">🤝 Bergabunglah Bersama Kami</h2>
    <p class="mb-2">🎮 Gabung Bersama CarlandsCompanyID! 🚀</p>
    <p class="mb-2">Apakah kamu punya semangat untuk menciptakan dunia game yang seru, inovatif, dan penuh tantangan?</p>
    <p class="mb-2">Di CarlandsCompanyID, kami bukan hanya membuat game — kami membangun pengalaman, komunitas, dan masa depan industri game Indonesia!</p>
    <p class="font-bold text-lg mb-2">✨ Mengapa bergabung dengan kami?</p>
    <ul class="ml-4 list-disc space-y-1">
      <li>Lingkungan kreatif dan kolaboratif</li>
      <li>Proyek game yang seru dan penuh potensi</li>
      <li>Kesempatan berkembang bersama tim profesional</li>
      <li>Dukungan penuh untuk ide dan inovasi kamu</li>
    </ul>
    <p class="mt-4 mb-2">💡Baik kamu developer, desainer, storyteller, content creator, atau gamers yang ingin berkarya — ini saatnya kamu ambil peran!</p>
    <p class="mb-2">📩 Yuk, kirim portofolio atau kenalan dulu dengan tim kami!</p>
    <p class="mb-2">📍 Temukan info lengkap di [website/link komunitas]</p>
    <p class="mb-4">📱 Atau DM kami langsung di [Instagram/Discord/WhatsApp]</p>
    <p class="font-bold">Bersama CarlandsCompanyID, wujudkan game impianmu!</p>
    <p class="text-sm mt-2">#CarlandsCompanyID #GameDeveloperIndonesia #JoinUs #Carlandsantipungli</p>
  </section>

  <div class="form-section text-center my-8" data-aos="zoom-in" data-aos-duration="1000">
    <h2 class="text-2xl font-semibold mb-4">📝 Pendaftaran Akun Pencoblosan [OPEN]</h2>
    <a href="https://forms.gle/1iyHNtXXghsjmqc9A" class="form-button text-lg" target="_blank">Buka Formulir</a>
  </div>

  <div class="social-buttons text-center mb-8" data-aos="fade-up" data-aos-duration="1500">
    <h2 class="text-2xl font-semibold mb-4">Temukan CarlandsCompany</h2>
    <div class="flex flex-wrap justify-center gap-2">
      <a href="https://www.youtube.com/@carlandsid" class="youtube"><i data-lucide="youtube"></i> YouTube</a>
      <a href="https://www.instagram.com/carlandscompanyid/" class="instagram"><i data-lucide="instagram"></i> Instagram</a>
      <a href="https://www.tiktok.com/@carlandscompanyid" class="tiktok"><i data-lucide="music"></i> TikTok</a>
      <a href="https://discord.com/invite/tnzfy7tSVS" class="discord"><i data-lucide="message-circle"></i> Discord</a>
      <a href="https://chat.whatsapp.com/EoyF4WTKUHB1feKjRdowss" class="whatsapp"><i data-lucide="phone"></i> WhatsApp</a>
    </div>
  </div>

  <section class="text-center" data-aos="zoom-in" data-aos-duration="1000">
    <h2 class="text-2xl font-semibold my-4">Jam Digital Seluruh Indonesia</h2>
    <div class="clock-grid">
      <div class="clock" id="wib">WIB (Jakarta): </div>
      <div class="clock" id="wita">WITA (Makassar): </div>
      <div class="clock" id="wit">WIT (Jayapura): </div>
    </div>
  </section>

  <section id="contact" class="text-center" data-aos="fade-up" data-aos-duration="1200">
    <h2 class="text-2xl font-semibold mb-4">Kontak Kami</h2>
    <p>Hai, butuh bantuan atau ingin bekerja sama dengan <strong>CarlandsCompanyID</strong>? Kami menunggu kabar darimu!</p>
    <p class="mt-4 font-semibold">Email Utama:</p>
    <a href="mailto:carlandscompanyid@gmail.com" class="text-blue-600 underline text-lg">carlandscompanyid@gmail.com</a>
    <p class="mt-4">Jangan ragu untuk mengirimkan pertanyaan, saran, atau sekadar menyapa. Kami akan membalas secepat mungkin!</p>
  </section>

  <div class="status" data-aos="fade-in" data-aos-duration="1000" data-aos-delay="200">
    <div class="dot online animate-pulse"></div>
    <span>Sedang Online</span>
  </div>

  <div class="warning mx-4 my-6 text-center text-sm" data-aos="flip-up" data-aos-duration="1000">
    <strong>⚠️ Peringatan:</strong> Ini adalah <strong>situs resmi</strong> milik CarlandsCompanyID. Situs selain <code>carlandscompanyid</code> adalah <strong>tidak resmi atau palsu</strong>.
  </div>

  <div class="neolux-section" data-aos="fade-up" data-aos-duration="1500">
    <header class="mb-12">
      <h1 class="neolux-header">NeoLux</h1>
      <p class="neolux-subheader">Elegance Beyond Code</p>
    </header>

    <section class="neolux-card-grid">
      <div class="glass" data-aos="fade-down" data-aos-duration="1000">
        <h2>Status Server</h2>
        <p id="serverStatus" class="mt-2 text-green-400 font-semibold text-xl">ONLINE</p>
      </div>
      <div class="glass" data-aos="fade-down" data-aos-duration="1200" data-aos-delay="200">
        <h2>Countdown Event</h2>
        <p id="countdown" class="mt-2 text-white font-semibold text-xl">Memuat...</p>
      </div>
      <div class="glass" data-aos="fade-down" data-aos-duration="1400" data-aos-delay="400">
        <h2>Gabung Komunitas</h2>
        <a href="https://chat.whatsapp.com/EoyF4WTKUHB1feKjRdowss" target="_blank" class="text-blue-400 underline mt-2 inline-block">Grup WhatsApp</a>
      </div>
    </section>

    <section class="mb-10">
      <audio id="bgMusic" loop autoplay>
        <source src="https://www.bensound.com/bensound-music/bensound-slowmotion.mp3" type="audio/mp3">
        Browser Anda tidak mendukung elemen audio.
      </audio>
      <button onclick="toggleAudio()" class="neolux-audio-button">🔊 Toggle Audio</button>
    </section>
  </div>

  <footer class="py-6 text-sm">
    © 2025 CarlandsCompanyID. Semua Hak Dilindungi.
    <p id="last-updated" class="mt-2">Terakhir diperbarui: <span id="update-time"></span></p>
  </footer>

  <button id="darkModeToggle" class="dark-mode-toggle">💡</button>

  <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
  <script>
    AOS.init({
      once: true, // Animasi hanya terjadi sekali saat discroll
      offset: 100, // Offset dari titik pemicu asli
      duration: 800, // Durasi animasi (ms)
      easing: 'ease-in-out', // Jenis easing animasi AOS
    });

    lucide.createIcons();

    // Sapaan Selamat Pagi/Siang/Sore/Malam
    function dapatkanSapaanFormal() {
      const jam = new Date().getHours();
      return jam < 11 ? "Selamat pagi!" :
             jam < 15 ? "Selamat siang!" :
             jam < 18 ? "Selamat sore!" : "Selamat malam!";
    }
    document.getElementById('sapaan').textContent = dapatkanSapaanFormal();

    // Marquee touch pause/play
    const marquee = document.getElementById('marquee');
    marquee.addEventListener('touchstart', () => {
      marquee.querySelector('.marquee-text').classList.toggle('paused');
    });

    // Perbarui Jam Indonesia
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

    // Waktu terakhir diperbarui
    const updateTime = new Date();
    document.getElementById("update-time").textContent = updateTime.toLocaleString("id-ID");

    // Countdown NeoLux (Diatur untuk 3 hari dari sekarang sebagai contoh)
    const countdownEl = document.getElementById('countdown');
    // Set targetDate menjadi 3 hari dari waktu sekarang
    const targetDate = new Date().getTime() + (3 * 24 * 60 * 60 * 1000); // 3 hari dari sekarang

    function updateCountdown() {
      const now = new Date().getTime();
      const diff = targetDate - now;

      if (diff <= 0) {
        countdownEl.innerText = "Event telah dimulai!";
        return;
      }

      const days = Math.floor(diff / (1000 * 60 * 60 * 24));
      const hours = Math.floor((diff % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
      const minutes = Math.floor((diff % (1000 * 60 * 60)) / (1000 * 60));
      const seconds = Math.floor((diff % (1000 * 60)) / 1000);
      countdownEl.innerText = `${days}h ${hours}j ${minutes}m ${seconds}d`;
      requestAnimationFrame(updateCountdown);
    }
    updateCountdown();

    // Toggle Audio NeoLux
    function toggleAudio() {
      const bgMusic = document.getElementById('bgMusic');
      bgMusic.paused ? bgMusic.play() : bgMusic.pause();
    }

    // Toggle Dark Mode
    const darkModeToggle = document.getElementById('darkModeToggle');
    darkModeToggle.addEventListener('click', () => {
      document.body.classList.toggle('dark-mode');
      const isDarkMode = document.body.classList.contains('dark-mode');
      localStorage.setItem('darkMode', isDarkMode);
      darkModeToggle.textContent = isDarkMode ? '☀️' : '💡'; // Ubah ikon
    });

    // Periksa preferensi dark mode saat halaman dimuat
    window.onload = () => {
      if (localStorage.getItem('darkMode') === 'true') {
        document.body.classList.add('dark-mode');
        darkModeToggle.textContent = '☀️';
      } else {
        darkModeToggle.textContent = '💡';
      }
    };
  </script>
<script type="text/javascript">
var Tawk_API=Tawk_API||{}, Tawk_LoadStart=new Date();
(function(){
var s1=document.createElement("script"),s0=document.getElementsByTagName("script")[0];
s1.async=true;
s1.src='https://embed.tawk.to/684cd03b47f3b9190b9ffeb1/1itm0qqrh';
s1.charset='UTF-8';
s1.setAttribute('crossorigin','*');
s0.parentNode.insertBefore(s1,s0);
})();
</script>
</body>
</html>
