<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>CarlandsCompanyID | NeoLux Interface</title>
  <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.2.19/dist/tailwind.min.css" rel="stylesheet">
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap" rel="stylesheet">
  <script src="https://unpkg.com/lucide@latest"></script>
  <style>
    body {
      background: linear-gradient(to right, #000000, #1f1f1f);
      font-family: 'Poppins', sans-serif;
      color: #fff;
      overflow-x: hidden;
    }
    .glass {
      backdrop-filter: blur(10px);
      background: rgba(255, 255, 255, 0.08);
      border: 1px solid rgba(255, 255, 255, 0.15);
      border-radius: 1rem;
      padding: 1.5rem;
    }
    .marquee-text {
      display: inline-block;
      white-space: nowrap;
      animation: scroll 30s linear infinite;
      color: #0ff;
    }
    @keyframes scroll {
      0% { transform: translateX(100%); }
      100% { transform: translateX(-100%); }
    }
    .dot { width: 12px; height: 12px; border-radius: 50%; margin-right: 8px; }
    .online { background-color: #4CAF50; }
    .offline { background-color: #f44336; }
  </style>
</head>
<body class="min-h-screen flex flex-col items-center text-center px-4">

  <!-- Header -->
  <header class="mt-10 mb-6">
    <h1 class="text-5xl font-bold text-yellow-400 animate-pulse">CarlandsCompanyID</h1>
    <p id="sapaan" class="text-lg text-gray-300 mt-2"></p>
    <p class="text-sm text-gray-500">Inovasi • Teknologi • Kreativitas</p>
  </header>

  <!-- Marquee -->
  <div class="w-full overflow-hidden py-3 bg-black border-y border-gray-700">
    <div class="marquee-text">👋 Selamat datang di CarlandsCompanyID! Bergabunglah bersama komunitas game masa depan! 🎮🚀</div>
  </div>

  <!-- Fitur Cards -->
  <section class="grid grid-cols-1 md:grid-cols-3 gap-6 max-w-6xl mt-10">
    <div class="glass">
      <h2 class="text-xl font-semibold text-yellow-300">Status Server</h2>
      <div class="flex justify-center items-center mt-2">
        <div class="dot online"></div><span class="text-green-400">ONLINE</span>
      </div>
    </div>
    <div class="glass">
      <h2 class="text-xl font-semibold text-yellow-300">Countdown Event</h2>
      <p id="countdown" class="mt-2 text-white">Memuat...</p>
    </div>
    <div class="glass">
      <h2 class="text-xl font-semibold text-yellow-300">Gabung Komunitas</h2>
      <a href="https://chat.whatsapp.com/EoyF4WTKUHB1feKjRdowss" target="_blank" class="text-blue-400 underline">WhatsApp Group</a>
    </div>
  </section>

  <!-- Visi Misi & Info -->
  <section class="glass mt-10 max-w-4xl">
    <h2 class="text-xl text-yellow-300 font-semibold mb-2">🎯 Misi Kami</h2>
    <p class="text-sm text-gray-300">Mengembangkan game berkualitas tinggi, membangun komunitas sehat, dan mendorong kreativitas lokal melalui teknologi.</p>

    <h2 class="text-xl text-yellow-300 font-semibold mt-6">🚀 Layanan Kami</h2>
    <ul class="list-disc text-left list-inside text-sm text-gray-300">
      <li>🌟 Pengembangan Game & Roleplay Server</li>
      <li>💼 Layanan Digital & Kreatif</li>
      <li>🛠️ Inovasi Teknologi Masa Depan</li>
    </ul>

    <h2 class="text-xl text-yellow-300 font-semibold mt-6">🤝 Ayo Bergabung!</h2>
    <p class="text-sm text-gray-300">📩 Kirim portofolio atau kenalan lewat IG/Discord/WA. Bersama kita bangun dunia game Indonesia! 🎮</p>
  </section>

  <!-- Formulir -->
  <div class="glass mt-10 max-w-md w-full text-center">
    <h2 class="mb-2 text-yellow-300 font-semibold">📝 Pendaftaran Akun Pencoblosan [OPEN]</h2>
    <a href="https://forms.gle/1iyHNtXXghsjmqc9A" class="text-white bg-blue-500 px-4 py-2 rounded hover:bg-blue-700 transition" target="_blank">Buka Formulir</a>
  </div>

  <!-- Jam Digital -->
  <section class="glass mt-10 max-w-xl w-full text-sm text-gray-200">
    <h2 class="text-lg font-semibold text-yellow-300 mb-2">🕒 Jam Digital Indonesia</h2>
    <div id="wib">WIB: -</div>
    <div id="wita">WITA: -</div>
    <div id="wit">WIT: -</div>
  </section>

  <!-- Sosial Media -->
  <div class="glass mt-10 max-w-2xl w-full">
    <h2 class="text-lg text-yellow-300 font-semibold mb-4">🌐 Temukan Kami</h2>
    <div class="flex flex-wrap justify-center gap-4 text-sm">
      <a href="https://www.youtube.com/@carlandsid" class="text-red-400 hover:underline">YouTube</a>
      <a href="https://www.instagram.com/carlandscompanyid/" class="text-pink-400 hover:underline">Instagram</a>
      <a href="https://www.tiktok.com/@carlandscompanyid" class="text-white hover:underline">TikTok</a>
      <a href="https://discord.com/invite/tnzfy7tSVS" class="text-indigo-400 hover:underline">Discord</a>
      <a href="https://chat.whatsapp.com/EoyF4WTKUHB1feKjRdowss" class="text-green-400 hover:underline">WhatsApp</a>
    </div>
  </div>

  <!-- Kontak -->
  <section class="glass mt-10 max-w-md w-full text-sm">
    <h2 class="text-yellow-300 font-semibold">📧 Kontak Kami</h2>
    <p>Email: <a href="mailto:carlandscompanyid@gmail.com" class="underline text-blue-400">carlandscompanyid@gmail.com</a></p>
  </section>

  <!-- Audio Control -->
  <section class="mt-10">
    <audio id="bgMusic" loop autoplay>
      <source src="https://www.bensound.com/bensound-music/bensound-slowmotion.mp3" type="audio/mp3">
    </audio>
    <button onclick="toggleAudio()" class="glass px-4 py-2 rounded-full text-sm font-semibold hover:bg-white hover:text-black transition">🔊 Toggle Audio</button>
  </section>

  <!-- Footer -->
  <footer class="text-gray-500 text-xs my-10">
    &copy; 2025 CarlandsCompanyID • Terakhir diperbarui: <span id="update-time"></span>
  </footer>

  <!-- Script -->
  <script>
    lucide.createIcons();

    document.getElementById('sapaan').textContent =
      new Date().getHours() < 11 ? "Selamat pagi!" :
      new Date().getHours() < 15 ? "Selamat siang!" :
      new Date().getHours() < 18 ? "Selamat sore!" : "Selamat malam!";

    const countdownEl = document.getElementById('countdown');
    const targetDate = new Date().getTime() + 24 * 60 * 60 * 1000;
    function updateCountdown() {
      const now = new Date().getTime();
      const diff = targetDate - now;
      if (diff <= 0) {
        countdownEl.innerText = "Event telah dimulai!";
        return;
      }
      const h = Math.floor((diff % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
      const m = Math.floor((diff % (1000 * 60 * 60)) / (1000 * 60));
      const s = Math.floor((diff % (1000 * 60)) / 1000);
      countdownEl.innerText = `${h}j ${m}m ${s}d`;
      requestAnimationFrame(updateCountdown);
    }
    updateCountdown();

    function updateIndonesianClocks() {
      const now = new Date();
      const opt = { hour: '2-digit', minute: '2-digit', second: '2-digit', hour12: false };
      document.getElementById("wib").textContent = "WIB (Jakarta): " + now.toLocaleTimeString("id-ID", { ...opt, timeZone: "Asia/Jakarta" });
      document.getElementById("wita").textContent = "WITA (Makassar): " + now.toLocaleTimeString("id-ID", { ...opt, timeZone: "Asia/Makassar" });
      document.getElementById("wit").textContent = "WIT (Jayapura): " + now.toLocaleTimeString("id-ID", { ...opt, timeZone: "Asia/Jayapura" });
    }
    setInterval(updateIndonesianClocks, 1000);
    updateIndonesianClocks();

    function toggleAudio() {
      const music = document.getElementById('bgMusic');
      music.paused ? music.play() : music.pause();
    }

    document.getElementById("update-time").textContent = new Date().toLocaleString("id-ID");
  </script>

  <!-- Tawk.to -->
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
