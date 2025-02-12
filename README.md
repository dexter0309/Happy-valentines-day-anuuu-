<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Ur Lovely Batoot</title>
  <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
  <style>
    body {
      font-family: 'Roboto', sans-serif;
      margin: 0;
      padding: 0;
      background-color: #3b0a45;
      color: white;
      text-align: center;
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      flex-direction: column;
    }
    .container {
      width: 100%;
      max-width: 500px;
      margin: 0 auto;
      padding: 20px;
      background-color: rgba(0, 0, 0, 0.7);
      border-radius: 10px;
    }
    h1 {
      font-size: 2.5em;
      margin-bottom: 30px;
      text-shadow: 2px 2px 5px rgba(255, 255, 255, 0.3);
    }
    input {
      padding: 10px;
      font-size: 1.2em;
      margin: 10px 0;
      width: 80%;
      border-radius: 5px;
      border: none;
      outline: none;
    }
    button {
      padding: 15px 25px;
      font-size: 1.2em;
      background-color: #e63946;
      color: white;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      margin-top: 20px;
    }
    button:hover {
      background-color: #f1faee;
    }
    .message {
      display: none;
      font-size: 1.5em;
      margin-top: 30px;
      line-height: 1.8;
    }
    audio {
      display: none;
    }
    .background {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: url('https://source.unsplash.com/1600x900/?love,roses') no-repeat center center fixed;
      background-size: cover;
      z-index: -1;
      opacity: 0.6;
    }
  </style>
</head>
<body>
  <div class="background"></div>
  <div class="container">
    <h1>Welcome, Ya Batatsss 💖</h1>
    <input type="text" id="username" placeholder="Username">
    <input type="password" id="password" placeholder="Password">
    <button onclick="login()">Log In</button>
    <div class="message" id="message">
      <p>I'm really sorry for every bad attitude I showed you. I never meant to do it. Maybe I’m just stressed over something, but just so you know, you're my happiness. I can’t imagine my life without you, Baby. You’re my person, my peace, my happiness, and the one who makes everything feel right, even when life is a mess. 😭❤️</p>
      <p>Distance sucks, I won’t lie. There are days I wish I could just teleport to you, hold you, and never let go. 🥺💔 But even with all the miles between us, my heart has never felt closer to someone. You’re the first thing on my mind when I wake up ☀️ and the last thought before I sleep. 🌙 And honestly? I wanna keep it that way forever.</p>
      <p>I don’t just want you to be my Valentine this year. I want you to be my Valentine every single year, for the rest of our lives. 💍🥰 I wanna be the one who makes you laugh when you’re sad 😘, who hypes you up when you doubt yourself 💪, and who stays by your side no matter what. I see a whole future with you, and I swear, I’ll do whatever it takes to make that happen. 💖✨</p>
      <p>So, Ya Batatsss, will you be my Valentine? Not just for today, not just for this year—but forever? 💌🥰💖</p>
      <p>Always yours, <br> Aduuuu ❤️</p>
      <button onclick="window.location.href='reply.html'">Next</button> <!-- Next Button -->
    </div>
  </div>
  <audio id="bgMusic" loop>
    <source src="https://www.soundhelix.com/examples/mp3/SoundHelix-Song-1.mp3" type="audio/mpeg">
  </audio>
  <script>
    // Play background music
    document.getElementById("bgMusic").play();

    // Login function: Automatically logs in after any input
    function login() {
      const username = document.getElementById("username").value;
      const password = document.getElementById("password").value;
      
      // Check if fields are not empty
      if (username !== "" && password !== "") {
        document.querySelector("h1").style.display = "none";
        document.querySelector("input").style.display = "none";
        document.querySelector("button").style.display = "none";
        document.getElementById("message").style.display = "block";
      } else {
        alert("Please enter both username and password!");
      }
    }
  </script>
</body>
</html>
