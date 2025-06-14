<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>CarlandscompanyID - Pemeliharaan Website</title>
  <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.2.19/dist/tailwind.min.css" rel="stylesheet" />
  <style>
    :root {
      color-scheme: light dark;
    }
    .countdown span {
      min-width: 60px;
      display: inline-block;
    }
  </style>
</head>
<body class="bg-gray-100 dark:bg-gray-900 flex items-center justify-center min-h-screen p-6 transition-colors">
  <div class="bg-white dark:bg-gray-800 rounded-2xl shadow-xl p-8 max-w-xl text-center text-gray-900 dark:text-white">
    <h1 class="text-3xl font-bold text-red-600 dark:text-red-400 mb-4">🔧 Website Sementara Dinonaktifkan</h1>
    <p class="text-lg mb-4">
      Website sementara kami nonaktifkan karena sedang dalam proses <span class="font-semibold text-blue-600 dark:text-blue-400">perombakan total</span>.
      Harap bersabar dan tunggu hingga proses selesai.
    </p>
    <p class="mb-6 text-gray-600 dark:text-gray-300">
      Semua progress pengerjaan akan dikirim melalui <span class="font-semibold text-green-600 dark:text-green-400">Pengumuman Komunitas CarlandscompanyID</span>.
    </p>

    <div class="countdown text-2xl font-mono space-x-2 mb-4">
      <span id="days">00</span>:
      <span id="hours">00</span>:
      <span id="minutes">00</span>:
      <span id="seconds">00</span>:
      <span id="milliseconds">000</span>
    </div>

    <div class="w-full bg-gray-300 dark:bg-gray-700 h-4 rounded-full overflow-hidden mb-6">
      <div id="progressBar" class="h-full bg-green-500 dark:bg-green-400 transition-all duration-200" style="width: 0%;"></div>
    </div>

    <a href="https://chat.whatsapp.com/EoyF4WTKUHB1feKjRdowss" target="_blank"
      class="inline-block bg-green-600 hover:bg-green-700 text-white font-semibold py-2 px-6 rounded-full transition">
      Bergabung ke Komunitas
    </a>
  </div>

  <!-- Audio Notifikasi -->
  <audio id="dingSound" src="https://actions.google.com/sounds/v1/alarms/alarm_clock.ogg" preload="auto"></audio>

  <script>
    const countdownDuration = 1 * 24 * 60 * 60 * 1000 + // 1 hari
                              20 * 60 * 60 * 1000 +     // 20 jam
                              20 * 60 * 1000 +          // 20 menit
                              20 * 1000 +               // 20 detik
                              200;                      // 200 milidetik

    const countdownKey = "carlandsCountdownEndTime";
    let endTime = localStorage.getItem(countdownKey);
    const dingSound = document.getElementById("dingSound");

    if (!endTime) {
      endTime = Date.now() + countdownDuration;
      localStorage.setItem(countdownKey, endTime);
    } else {
      endTime = parseInt(endTime, 10);
    }

    const totalDuration = endTime - (Date.now());

    let countdownDone = false;

    function updateCountdown() {
      const now = Date.now();
      let distance = endTime - now;

      if (distance <= 0 && !countdownDone) {
        document.getElementById("days").textContent = "00";
        document.getElementById("hours").textContent = "00";
        document.getElementById("minutes").textContent = "00";
        document.getElementById("seconds").textContent = "00";
        document.getElementById("milliseconds").textContent = "000";
        document.getElementById("progressBar").style.width = "100%";
        dingSound.play();
        countdownDone = true;
        return;
      }

      const days = Math.floor(distance / (1000 * 60 * 60 * 24));
      const hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
      const minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
      const seconds = Math.floor((distance % (1000 * 60)) / 1000);
      const milliseconds = distance % 1000;

      const percent = 100 - (distance / totalDuration * 100);
      document.getElementById("progressBar").style.width = `${percent.toFixed(2)}%`;

      document.getElementById("days").textContent = String(days).padStart(2, "0");
      document.getElementById("hours").textContent = String(hours).padStart(2, "0");
      document.getElementById("minutes").textContent = String(minutes).padStart(2, "0");
      document.getElementById("seconds").textContent = String(seconds).padStart(2, "0");
      document.getElementById("milliseconds").textContent = String(milliseconds).padStart(3, "0");
    }

    setInterval(updateCountdown, 50);
  </script>
</body>
</html>
