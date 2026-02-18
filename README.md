<!DOCTYPE html>
<html>
<head>
  <title>Happy Birthday Legend 🎉</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    body {
      margin: 0;
      padding: 0;
      text-align: center;
      font-family: 'Arial', sans-serif;
      overflow: hidden;
      background: linear-gradient(-45deg, #ff4e50, #f9d423, #24c6dc, #5433ff);
      background-size: 400% 400%;
      animation: gradientBG 8s ease infinite;
      color: white;
    }

    @keyframes gradientBG {
      0% { background-position: 0% 50%; }
      50% { background-position: 100% 50%; }
      100% { background-position: 0% 50%; }
    }

    h1 {
      font-size: 60px;
      margin-top: 120px;
      animation: fadeIn 2s ease-in-out;
    }

    p {
      font-size: 24px;
      animation: fadeIn 3s ease-in-out;
    }

    button {
      padding: 15px 30px;
      font-size: 18px;
      border: none;
      border-radius: 30px;
      cursor: pointer;
      margin-top: 30px;
      background: white;
      color: #ff4e50;
      font-weight: bold;
      transition: 0.3s;
    }

    button:hover {
      transform: scale(1.1);
    }

    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }

    .confetti {
      position: fixed;
      width: 10px;
      height: 10px;
      background-color: white;
      top: -10px;
      animation: fall 5s linear infinite;
    }

    @keyframes fall {
      to {
        transform: translateY(100vh);
      }
    }
  </style>
</head>

<body>

  <h1>🎉 Happy Birthday Bro 🎉</h1>
  <p>You are not older… just more legendary 😎🔥</p>

  <button onclick="surprise()">Click for Surprise 🎁</button>

  <script>
    function surprise() {
      alert("You're not just my best friend. You're family. Stay crazy, stay awesome. Love you bro 💙");
    }

    // Confetti generator
    for (let i = 0; i < 100; i++) {
      let confetti = document.createElement("div");
      confetti.classList.add("confetti");
      confetti.style.left = Math.random() * 100 + "vw";
      confetti.style.animationDuration = (Math.random() * 3 + 2) + "s";
      confetti.style.backgroundColor = 
        "hsl(" + Math.random() * 360 + ", 100%, 50%)";
      document.body.appendChild(confetti);
    }
  </script>

</body>
</html>
