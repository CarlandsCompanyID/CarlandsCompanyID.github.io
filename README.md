<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>CarlandsCompanyID - Website Resmi</title>
  <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.2.19/dist/tailwind.min.css" rel="stylesheet">
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap" rel="stylesheet">
  <script src="https://unpkg.com/lucide@latest"></script>
  <style>
    body {
      margin: 0;
      font-family: 'Poppins', sans-serif;
      background-color: #f4f4f4;
      color: #333;
      line-height: 1.6;
    }
    header, footer {
      background-color: #003366;
      color: #fff;
      text-align: center;
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
      display: inline-block;
      margin: 0.5rem;
      padding: 0.75rem 1rem;
      border-radius: 8px;
      font-weight: bold;
      color: #fff;
    }
    .youtube { background: #FF0000; }
    .instagram { background: #C13584; }
    .tiktok { background: #010101; }
    .discord { background: radial-gradient(circle at top left, #5865F2, #404EED); }
    .whatsapp { background: #25D366; }
    .social-buttons a:hover {
      opacity: 0.8;
    }
    .form-button {
      display: inline-block;
      padding: 0.75rem 1.5rem;
      background-color: #4285F4;
      color: white;
      border-radius: 6px;
      transition: background-color .3s;
    }
    .form-button:hover {
      background-color: #3367D6;
    }
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
      padding-left: 100%;
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
    }
    @media (max-width: 600px) {
      .text-5xl { font-size: 2.5rem; }
      .text-2xl { font-size: 1.25rem; }
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
  </style>
</head>
<body>

  <section class="fade-in text-center">
    <div class="text-5xl mb-4">👋👋</div>
    <h2 id="sapaan" class="text-2xl font-semibold mb-2"></h2>
    <p class="text-gray-700 mb-4">Selamat datang di situs resmi kami. Semoga hari Anda menyenangkan dan penuh produktivitas.</p>
    <p class="text-sm text-gray-500">Dibawakan oleh <strong>CarlandsCompanyID</strong><br>Inovasi • Teknologi • Kreativitas</p>
  </section>

  <div class="marquee-container" id="marquee">
    <div class="marquee-text">
      Selamat Datang di CarlandsCompanyID! Hai, Sobat Carlanders! 👋 Terima kasih sudah bergabung bersama kami...
    </div>
  </div>

  <section>
    <h2>🎯 Misi Kami</h2>
    <p>Membangun ekosistem digital yang kreatif dan inovatif...</p>
    <h2>🚀 Apa yang Kami Tawarkan</h2>
    <ul class="ml-4 list-disc">
      <li>🌟 Pengembangan Game & Roleplay Server</li>
      <li>💼 Layanan Digital & Kreatif</li>
      <li>🛠️ Inovasi Teknologi Masa Depan</li>
    </ul>
    <h2>🤝 Bergabunglah Bersama Kami</h2>
    <p>Kami terbuka untuk kolaborasi, mitra kerja...</p>
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
