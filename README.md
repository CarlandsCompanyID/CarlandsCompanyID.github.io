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

    <!-- Form Email/Saran -->
    <form onsubmit="submitForm(event)" class="mb-6 text-left">
      <label class="block mb-1 text-gray-700 font-medium">Email (opsional):</label>
      <input type="email" id="email" class="w-full mb-3 px-4 py-2 rounded-lg border border-gray-300 focus:outline-none focus:ring-2 focus:ring-blue-500" placeholder="contoh@email.com" />

      <label class="block mb-1 text-gray-700 font-medium">Saran atau pesan:</label>
      <textarea id="pesan" rows="3" class="w-full px-4 py-2 rounded-lg border border-gray-300 focus:outline-none focus:ring-2 focus:ring-blue-500" placeholder="Ketik saran atau pesan..."></textarea>

      <button type="submit" class="mt-4 w-full bg-blue-600 text-white py-2 rounded-lg hover:bg-blue-700 transition">
        Kirim Pesan
      </button>
    </form>

    <!-- Footer CTA -->
    <p class="text-sm text-gray-500">Kami akan mengirimkan notifikasi ke email Anda ketika website kembali online.</p>
  </div>

  <!-- Script Countdown + Status -->
  <script>
    const countdownEl = document.getElementById("countdown");
    const statusEl = document.getElementById("status");
    const targetTime = new Date().getTime() + 10 * 60 * 60 * 1000; // 10 jam dari sekarang

    function updateCountdown() {
      const now = new Date().getTime();
      const distance = targetTime - now;

      if (distance <= 0) {
        countdownEl.innerText = "Website sudah kembali online!";
        statusEl.innerHTML = "Status: <span class='text-green-600 font-bold'>Online</span>";
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

  <!-- Simulasi Kirim Form -->
  <script>
    function submitForm(e) {
      e.preventDefault();
      const email = document.getElementById('email').value;
      const pesan = document.getElementById('pesan').value;

      if (!pesan.trim()) {
        alert("Tolong isi pesan Anda terlebih dahulu.");
        return;
      }

      alert("Pesan Anda telah dikirim! Terima kasih 🙏\n\n(Notifikasi email akan dikirim saat website online kembali —)");
      e.target.reset();
    }
  </script>

</body>
</html>
