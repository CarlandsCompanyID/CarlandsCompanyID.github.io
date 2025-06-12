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
</html>
