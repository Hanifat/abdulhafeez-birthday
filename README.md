<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Happy Birthday Abdulhafeez 🎉</title>

  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Poppins', sans-serif;
    }

    body {
      min-height: 100vh;
      background: linear-gradient(135deg, #0f2027, #203a43, #2c5364);
      color: #ffffff;
      overflow-x: hidden;
    }

    .container {
      padding: 80px 20px;
      text-align: center;
    }

    h1 {
      font-size: 3rem;
      margin-bottom: 10px;
      animation: fadeDown 1.5s ease;
    }

    h2 {
      font-weight: 300;
      margin-bottom: 40px;
      animation: fadeUp 2s ease;
    }

    .card {
      max-width: 520px;
      margin: auto;
      background: rgba(255, 255, 255, 0.15);
      backdrop-filter: blur(10px);
      border-radius: 20px;
      padding: 35px 30px;
      animation: zoomIn 2s ease;
    }

    .card p {
      font-size: 1.1rem;
      line-height: 1.9;
    }

    .signature {
      margin-top: 20px;
      font-weight: 600;
      font-size: 1.2rem;
      color: #ffd700;
    }

    footer {
      margin-top: 60px;
      font-size: 0.9rem;
      opacity: 0.8;
    }

    @keyframes fadeDown {
      from { opacity: 0; transform: translateY(-40px); }
      to { opacity: 1; transform: translateY(0); }
    }

    @keyframes fadeUp {
      from { opacity: 0; transform: translateY(40px); }
      to { opacity: 1; transform: translateY(0); }
    }

    @keyframes zoomIn {
      from { opacity: 0; transform: scale(0.85); }
      to { opacity: 1; transform: scale(1); }
    }

    /* Confetti */
    .confetti {
      position: fixed;
      width: 10px;
      height: 10px;
      top: -10px;
      animation: fall linear infinite;
    }

    @keyframes fall {
      to {
        transform: translateY(110vh) rotate(360deg);
      }
    }
  </style>
</head>
<body>

  <div class="container">
    <h1>🎉 Happy Birthday 🎉</h1>
    <h2>Alade Abdulhafeez</h2>

    <div class="card">
      <p>
        On this special day, I pray that Allah blesses you with long life, good health,
        and abundant barakah. May He guide your steps, strengthen your imān, and reward
        your kindness and sincerity. May your life continue to inspire and motivate
        everyone around you, and may Allah grant you success in this world and the Hereafter.
        Āmīn.
      </p>

      <div class="signature">
        — With heartfelt prayers, <br>
        Haneefah 🤍
      </div>
    </div>

    <footer>
      Made with ❤️ by Haneefah
    </footer>
  </div>

  <script>
    for (let i = 0; i < 60; i++) {
      const confetti = document.createElement("div");
      confetti.classList.add("confetti");
      confetti.style.left = Math.random() * 100 + "vw";
      confetti.style.animationDuration = Math.random() * 3 + 2 + "s";
      confetti.style.backgroundColor =
        ["#ffd700", "#ffffff", "#4dd0e1", "#ff8a65"][Math.floor(Math.random() * 4)];
      document.body.appendChild(confetti);
    }
  </script>

</body>
</html>
