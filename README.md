<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Pemeliharaan Website</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <style>
    .fade-in { animation: fadeIn 1.5s ease-in-out both; }
    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(10px); }
      to { opacity: 1; transform: translateY(0); }
    }
  </style>
</head>
<body class="bg-gray-100 flex items-center justify-center min-h-screen px-4">

  <div class="bg-white rounded-2xl shadow-xl p-8 max-w-xl w-full text-center fade-in">
    <!-- Icon & Judul -->
    <div class="mb-4">
      <svg class="mx-auto h-16 w-16 text-yellow-500" fill="none" stroke="currentColor" stroke-width="1.5" viewBox="0 0 24 24">
        <path stroke-linecap="round" stroke-linejoin="round" d="M12 9v2m0 4h.01M21 12a9 9 0 11-18 0 9 9 0 0118 0z" />
      </svg>
    </div>
    <h1 class="text-3xl font-bold text-gray-800 mb-2">Website Sedang Dalam Pemeliharaan</h1>
    <p class="text-gray-600 text-base mb-4">
      Developer kami sedang memperbaiki sistem karena beberapa bug ditemukan. Mohon bersabar, kami akan segera kembali.
    </p>

    <!-- Status -->
    <div id="status" class="mb-4 text-sm font-medium text-yellow-600">Status: <span class="font-bold">Offline</span></div>

    <!-- Countdown -->
    <div class="bg-gray-100 rounded-lg p-4 mb-4">
      <p class="text-gray-700 text-sm mb-1">Perkiraan waktu online kembali:</p>
      <div id="countdown" class="text-xl font-bold text-gray-800">Memuat...</div>
    </div>

    <!-- Progress -->
    <div class="w-full bg-gray-300 rounded-full h-3 mb-6 overflow-hidden">
      <div class="bg-blue-500 h-full animate-pulse w-3/4"></div>
    </div>

    <p class="text-sm text-gray-500">Kami akan mengirimkan notifikasi ke email Anda ketika website kembali online.</p>
  </div>

  <!-- JavaScript Countdown + Simpan Target ke localStorage -->
  <script>
    const countdownEl = document.getElementById("countdown");
    const statusEl = document.getElementById("status");
    const TIMER_KEY = "maintenance_target_time";

    // Inisialisasi target waktu 10 jam ke depan jika belum ada di localStorage
    if (!localStorage.getItem(TIMER_KEY)) {
      const target = new Date().getTime() + 10 * 60 * 60 * 1000;
      localStorage.setItem(TIMER_KEY, target);
    }

    const targetTime = parseInt(localStorage.getItem(TIMER_KEY), 10);

    function updateCountdown() {
      const now = new Date().getTime();
      const distance = targetTime - now;

      if (distance <= 0) {
        countdownEl.innerText = "Website sudah kembali online!";
        statusEl.innerHTML = "Status: <span class='text-green-600 font-bold'>Online</span>";
        localStorage.removeItem(TIMER_KEY);
        return;
      }

      const hours = Math.floor(distance / (1000 * 60 * 60));
      const minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
      const seconds = Math.floor((distance % (1000 * 60)) / 1000);

      countdownEl.innerText = `${hours}j ${minutes}m ${seconds}d`;
    }

    setInterval(updateCountdown, 1000);
    updateCountdown();
  </script>

</body>
</html>
