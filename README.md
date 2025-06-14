<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>NeoLux - Elegance Beyond Code</title>
  <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.2.19/dist/tailwind.min.css" rel="stylesheet">
  <style>
    body {
      background: linear-gradient(to right, #000000, #1f1f1f);
      font-family: 'Poppins', sans-serif;
      color: #fff;
      overflow-x: hidden;
    }
    .glass {
      backdrop-filter: blur(10px);
      background: rgba(255, 255, 255, 0.1);
      border: 1px solid rgba(255, 255, 255, 0.2);
    }
  </style>
</head>
<body class="min-h-screen flex flex-col items-center justify-center text-center px-4">
  
  <!-- Header -->
  <header class="mb-12">
    <h1 class="text-4xl md:text-6xl font-bold text-yellow-400 animate-pulse">NeoLux</h1>
    <p class="text-gray-300 text-lg md:text-xl mt-2">Elegance Beyond Code</p>
  </header>

  <!-- Fitur Cards -->
  <section class="grid grid-cols-1 md:grid-cols-3 gap-6 max-w-6xl mb-12">
    <div class="glass rounded-2xl p-6">
      <h2 class="text-xl font-semibold text-yellow-300">Status Server</h2>
      <p id="serverStatus" class="mt-2 text-green-400">ONLINE</p>
    </div>
    <div class="glass rounded-2xl p-6">
      <h2 class="text-xl font-semibold text-yellow-300">Countdown Event</h2>
      <p id="countdown" class="mt-2 text-white">Loading...</p>
    </div>
    <div class="glass rounded-2xl p-6">
      <h2 class="text-xl font-semibold text-yellow-300">Gabung Komunitas</h2>
      <a href="https://chat.whatsapp.com/EoyF4WTKUHB1feKjRdowss" target="_blank" class="text-blue-400 underline">WhatsApp Group</a>
    </div>
  </section>

  <!-- Audio -->
  <section class="mb-10">
    <audio id="bgMusic" loop autoplay>
      <source src="https://www.bensound.com/bensound-music/bensound-slowmotion.mp3" type="audio/mp3">
    </audio>
    <button onclick="toggleAudio()" class="glass px-4 py-2 rounded-full text-sm font-semibold text-white hover:bg-white hover:text-black transition">🔊 Toggle Audio</button>
  </section>

  <!-- Footer -->
  <footer class="text-gray-400 text-sm">
    © 2025 NeoLux. Crafted with ✨
  </footer>

  <script>
    // Countdown
    const countdownEl = document.getElementById('countdown');
    const targetDate = new Date().getTime() + (1 * 24 * 60 * 60 * 1000); // 1 hari

    function updateCountdown() {
      const now = new Date().getTime();
      const diff = targetDate - now;

      if (diff <= 0) {
        countdownEl.innerText = "Event telah dimulai!";
        return;
      }

      const hours = Math.floor((diff % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
      const minutes = Math.floor((diff % (1000 * 60 * 60)) / (1000 * 60));
      const seconds = Math.floor((diff % (1000 * 60)) / 1000);
      countdownEl.innerText = `${hours}j ${minutes}m ${seconds}d`;
      requestAnimationFrame(updateCountdown);
    }
    updateCountdown();

    // Toggle Audio
    function toggleAudio() {
      const bgMusic = document.getElementById('bgMusic');
      bgMusic.paused ? bgMusic.play() : bgMusic.pause();
    }
  </script>
</body>
</html>
