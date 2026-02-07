<!DOCTYPE html>
<html lang="tl">
<head>
  <meta charset="UTF-8">
  <title>Will You Be My Valentine?</title>
  <style>
    body {
      margin: 0;
      height: 100vh;
      font-family: 'Segoe UI', sans-serif;
      background: linear-gradient(135deg, #ff6a88, #ff99ac);
      display: flex;
      justify-content: center;
      align-items: center;
      text-align: center;
      color: white;
    }
    .box {
      background: rgba(255,255,255,0.15);
      padding: 40px;
      border-radius: 25px;
      max-width: 420px;
      box-shadow: 0 15px 40px rgba(0,0,0,0.25);
    }
    h1 {
      font-size: 2.4em;
      margin-bottom: 10px;
    }
    p {
      font-size: 1.1em;
      margin-bottom: 25px;
    }
    button {
      padding: 12px 25px;
      font-size: 1em;
      border: none;
      border-radius: 30px;
      cursor: pointer;
      margin: 5px;
    }
    .yes {
      background: white;
      color: #ff4f81;
    }
    .no {
      background: #ff4f81;
      color: white;
      position: absolute;
    }
  </style>
</head>
<body>

  <div class="box">
    <h1>Hi, my love ❤️</h1>
    <p>
      Alam kong may mga araw na nagkukulang ako,  
      pero gusto kong malaman mo na ikaw pa rin ang pipiliin ko palagi.
    </p>
    <h2>Will you be my Valentine? 💘</h2>

    <button class="yes" onclick="yesClicked()">Yes 💕</button>
    <button class="no" onmouseover="moveNo(this)">No 😅</button>
  </div>

  <script>
    function yesClicked() {
      alert("Yay! I love you so much ❤️ Happy Valentine’s Day!");
    }

    function moveNo(btn) {
      const x = Math.random() * (window.innerWidth - 100);
      const y = Math.random() * (window.innerHeight - 50);
      btn.style.left = x + "px";
      btn.style.top = y + "px";
    }
  </script>

</body>
</html>
