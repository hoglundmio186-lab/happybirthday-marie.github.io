<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Happy Birthday Marie!</title>
  <style>
    body {
      font-family: 'Trebuchet MS', sans-serif;
      background: linear-gradient(to bottom right, #ffe6f0, #fff5fb);
      color: #333;
      text-align: center;
      padding: 50px;
    }

    h1 {
      font-size: 2.5em;
      color: #e34a7f;
    }

    p {
      font-size: 1.2em;
      max-width: 600px;
      margin: 20px auto;
      line-height: 1.6;
    }

    .heart {
      font-size: 3em;
      color: #e34a7f;
      margin-top: 20px;
    }

    button {
      background-color: #e34a7f;
      color: white;
      border: none;
      padding: 12px 24px;
      border-radius: 25px;
      font-size: 1em;
      cursor: pointer;
      margin-top: 30px;
      transition: 0.3s;
    }

    button:hover {
      background-color: #ff79b0;
      transform: scale(1.05);
    }

    #memories {
      display: none;
      margin-top: 40px;
      opacity: 0;
      transition: opacity 1s ease-in-out;
    }

    #memories.show {
      display: block;
      opacity: 1;
    }

    #memories img {
      width: 300px;
      height: auto;
      border-radius: 15px;
      margin: 10px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.2);
      transition: transform 0.3s;
    }

    #memories img:hover {
      transform: scale(1.05);
    }

    #extraMessage {
      margin-top: 20px;
      font-size: 1.2em;
      color: #e34a7f;
      display: none;
    }
  </style>
</head>
<body>
  <h1>💖 Happy Birthday, Marie! 💖</h1>
  <p>Dear Marie,</p>
  <p>Although we haven't known you for that long, it already feels like you've been in our lives forever. It feels like just yesterday when we first played ACNH together, and somehow from that moment, everything just felt right.</p>
  <p>You may be older than us, but you have always made us feel at an equal level, like we truly belong. You bring such warmth, patience, and care into every conversation, making sure everyone is comfortable and included. With you, we can be ourselves completely. With you, we always end up laughing. And with you, there's never a dull moment.</p>
  <p>We love you so much and are just so grateful for each and every moment we've spent together so far. Thank you for being such an amazing friend—for your kindness, your sense of humor, and for just being yourself. Here's to many more cozy calls, endless laughter, and new memories together.</p>
  <p>With all our love,<br><b>Kachow, Lu & Mio</b></p>

  <div class="heart">💗💗💗</div>

  <button onclick="toggleMemories()">Show our memories 💫</button>

  <div id="memories">
    <img src="https://i.imgur.com/oiCZNV7.jpg" alt="Memory 1">
    <img src="https://i.imgur.com/m8LTzZe.jpg" alt="Memory 2">
    <img src="https://i.imgur.com/oiCZNV7.jpg" alt="Memory 3">
  </div>

  <div id="extraMessage">We’ll never forget these moments ❤️</div>

  <script>
    function toggleMemories() {
      const memories = document.getElementById("memories");
      const button = document.querySelector("button");
      const extraMessage = document.getElementById("extraMessage");

      if (!memories.classList.contains("show")) {
        memories.classList.add("show");
        extraMessage.style.display = "block";
        button.textContent = "Hide our memories 💞";
      } else {
        memories.classList.remove("show");
        extraMessage.style.display = "none";
        button.textContent = "Show our memories 💫";
      }
    }
  </script>
</body>
</html>
