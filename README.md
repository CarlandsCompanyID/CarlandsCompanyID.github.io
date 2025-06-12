<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>CarlandsCompanyID - Website Resmi</title>
  <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.2.19/dist/tailwind.min.css" rel="stylesheet">
  <script src="https://unpkg.com/lucide@latest"></script>
  <style>
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
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
  </style>
</head>
<body>
  <header class="py-8">
    <h1 class="text-3xl font-bold">CarlandsCompanyID Website Resmi</h1>
  </header>

  <section class="fade-in text-center">
    <div class="text-5xl mb-4">👋</div>
    <h2 id="sapaan" class="text-2xl font-semibold mb-2"></h2>
    <p class="text-gray-700 mb-4">Selamat datang @user di situs resmi kami. Semoga hari Anda menyenangkan dan penuh produktivitas.</p>
    <p class="text-sm text-gray-500">Dibawakan oleh <strong>CarlandsCompanyID</strong><br>Inovasi • Teknologi • Kreativitas</p>
  </section>

  <section>
    <h2>🎯 Misi Kami</h2>
    <p>Membangun ekosistem digital yang kreatif dan inovatif, serta memberikan solusi teknologi berkualitas tinggi untuk semua kalangan.</p>
    <h2>🚀 Apa yang Kami Tawarkan</h2>
    <ul class="ml-4 list-disc">
      <li>🌟 Pengembangan Game & Roleplay Server</li>
      <li>💼 Layanan Digital & Kreatif</li>
      <li>🛠️ Inovasi Teknologi Masa Depan</li>
    </ul>
    <h2>🤝 Bergabunglah Bersama Kami</h2>
    <p>Kami terbuka untuk kolaborasi, mitra kerja, dan talenta baru yang ingin tumbuh bersama membangun masa depan digital Indonesia.</p>
  </section>

  <div class="form-section text-center">
    <h2 class="mb-2">📝 Pendaftaran Akun Pencoblosan [OPEN] </h2>
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
  <html lang="id">
<head>
  <meta charset="UTF-8">
  <title>Jam Seluruh Indonesia</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
      background-color: #f0f0f0;
      padding: 40px;
    }
    h1 {
      margin-bottom: 40px;
    }
    .clock {
      background: #ffffff;
      padding: 20px;
      margin: 10px auto;
      width: 300px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
      border-radius: 10px;
      font-size: 1.8em;
    }
  </style>
</head>
<body>
  <h1>Jam Digital Seluruh Indonesia</h1>

  <div class="clock" id="wib">WIB (Jakarta): </div>
  <div class="clock" id="wita">WITA (Makassar): </div>
  <div class="clock" id="wit">WIT (Jayapura): </div>

  <script>
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
  </script>
</body>
</html>
  <div class="warning mx-4">
    <strong>⚠️ Peringatan:</strong> Ini adalah <strong>situs resmi</strong> milik CarlandsCompanyID. Situs selain <code>carlandscompanyid</code> adalah <strong>tidak resmi atau palsu</strong>.
  </div>

  <footer class="py-6">
    &copy; 2025 CarlandsCompanyID. Semua Hak Dilindungi.
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
  </script>
</body>
</html>
<p id="last-updated">Terakhir diperbarui: <span id="update-time"></span></p>

<script>
  const updateTime = new Date();
  document.getElementById("update-time").textContent = updateTime.toLocaleString("id-ID");
</script>
