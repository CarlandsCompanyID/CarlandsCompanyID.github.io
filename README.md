<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Status Website</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      height: 100vh;
      display: flex;
      align-items: center;
      justify-content: center;
      background-color: #f0f2f5;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }

    .card {
      text-align: center;
      background-color: #fff;
      padding: 40px 60px;
      border-radius: 20px;
      box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
    }

    .card h1 {
      font-size: 2.8rem;
      color: #c0392b;
      margin-bottom: 20px;
    }

    .status {
      display: inline-block;
      padding: 10px 20px;
      border-radius: 50px;
      font-weight: bold;
      font-size: 1rem;
      color: #fff;
    }

    .online {
      background-color: #27ae60;
    }

    .offline {
      background-color: #e74c3c;
    }
  </style>
</head>
<body>
  <div class="card">
    <h1>[ WEBSITE SEDANG DI PERBAIKI ]</h1>

    <!-- Ganti class 'offline' menjadi 'online' jika status aktif -->
    <div class="status offline">STATUS: OFFLINE</div>
  </div>
</body>
</html>
