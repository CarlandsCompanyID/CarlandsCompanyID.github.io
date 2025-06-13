<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Website Sedang Down</title>
  <style>
    * {
      box-sizing: border-box;
    }

    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background-color: #f2f4f8;
      margin: 0;
      padding: 0;
      display: flex;
      justify-content: center;
      align-items: center;
      min-height: 100vh;
    }

    .container {
      background: #ffffff;
      padding: 30px 20px;
      border-radius: 15px;
      box-shadow: 0 5px 20px rgba(0,0,0,0.1);
      text-align: center;
      max-width: 500px;
      width: 90%;
    }

    .emoji {
      font-size: 50px;
      margin-bottom: 10px;
    }

    h1 {
      font-size: 24px;
      color: #e74c3c;
      margin-bottom: 15px;
    }

    p {
      font-size: 16px;
      color: #333;
      margin-bottom: 10px;
    }

    .social {
      font-size: 14px;
      color: #666;
      margin-top: 20px;
    }

    @media (min-width: 768px) {
      .container {
        padding: 40px;
      }

      h1 {
        font-size: 28px;
      }

      p {
        font-size: 18px;
      }

      .emoji {
        font-size: 60px;
      }
    }
  </style>
</head>
<body>
  <div class="container">
    <div class="emoji">🔧</div>
    <h1>WEBSITE SEDANG DI PERBARUI!</h1>
    <p>Tim kami sedang melakukan <strong>pemeliharaan dan perbaikan sistem</strong> untuk meningkatkan kualitas layanan.</p>
    <p>⏳ Harap bersabar, website akan kembali <strong>segera</strong>.</p>
    <div class="social">
      📢 Untuk info terbaru, silakan pantau media sosial resmi kami.
    </div>
  </div>
</body>
</html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <title>Countdown 5 Jam</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
      font-size: 2em;
      margin-top: 100px;
    }
  </style>
</head>
<body>
  <div id="countdown">Memulai hitung mundur...</div>

  <script>
    // Hitung waktu target (5 jam dari sekarang)
    const targetTime = new Date().getTime() + 5 * 60 * 60 * 1000;

    const countdownElement = document.getElementById("countdown");

    const updateCountdown = () => {
      const now = new Date().getTime();
      const distance = targetTime - now;

      if (distance < 0) {
        countdownElement.innerHTML = "Waktu Habis!";
        clearInterval(interval);
        return;
      }

      const hours = Math.floor(distance / (1000 * 60 * 60));
      const minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
      const seconds = Math.floor((distance % (1000 * 60)) / 1000);

      countdownElement.innerHTML = ${hours.toString().padStart(2, '0')}: +
                                   ${minutes.toString().padStart(2, '0')}: +
                                   ${seconds.toString().padStart(2, '0')};
    };

    // Perbarui setiap detik
    const interval = setInterval(updateCountdown, 1000);
    updateCountdown();
  </script>
</body>
</html>
</body>
</html>
