<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no" />
  <title>⚠️ CRITICAL SYSTEM FAILURE ⚠️</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    html, body {
      height: 100%;
    }
    body {
      background-color: black;
      color: red;
      font-family: 'Courier New', Courier, monospace;
      overflow: hidden;
    }
    .center {
      text-align: center;
      padding: 10vh 5vw;
    }
    .warning {
      font-size: 6vw;
      animation: blink 0.6s infinite;
    }
    .details {
      margin-top: 30px;
      font-size: 4vw;
    }
    .loader {
      margin: 50px auto;
      width: 90%;
      background: #330000;
      border: 2px solid red;
    }
    .bar {
      height: 30px;
      width: 0;
      background: darkred;
      animation: load 8s linear forwards;
    }

    @keyframes load {
      to {
        width: 100%;
      }
    }

    @keyframes blink {
      0% { opacity: 1; }
      50% { opacity: 0; }
      100% { opacity: 1; }
    }
  </style>
</head>
<body>
  <div class="center">
    <h1 class="warning">💀 SYSTEM HACKED 💀</h1>
    <div class="details">
      <p>WARNING: Critical malware detected!</p>
      <p>Deleting System Files: C:/Windows/System32...</p>
      <p>IP Address Leaked • Webcam Activated • Bank Login Compromised</p>
    </div>
    <div class="loader">
      <div class="bar"></div>
    </div>
    <p style="color:white; margin-top:30px; font-size:3.5vw;">Please do not close this window...</p>
  </div>

  <audio id="scream" autoplay loop>
    <source src="https://www.myinstants.com/media/sounds/horror-sound.mp3" type="audio/mpeg">
  </audio>

  <script>
    // Auto-trigger popups and sound after delay
    window.onload = () => {
      setTimeout(() => {
        spawnPopup();
      }, 4000); // 4 second delay before prank starts

      setTimeout(() => {
        jumpScare();
      }, 10000); // 10 seconds until jump scare
    }

    function spawnPopup() {
      for (let i = 0; i < 5; i++) {
        let w = window.open('', '', 'width=300,height=200');
        if (w) {
          w.document.write(`
            <body style=\"background:black;color:red;font-family:Courier New;text-align:center;\">
            <h1>💀 SYSTEM FAILURE 💀</h1>
            <p>Data breach in progress...</p>
            <p>Your files are being stolen.</p>
            </body>
          `);
        }
      }
      document.getElementById("scream").play();
    }

    function jumpScare() {
      document.body.innerHTML = `
        <div style="background:black;width:100vw;height:100vh;display:flex;flex-direction:column;justify-content:center;align-items:center;">
          <img src="https://media.tenor.com/SO3wU_FxVnkAAAAC/horror-scary.gif" alt="Ghost Scare" style="width:100vw;height:100vh;object-fit:cover;z-index:999;" />
        </div>
      `;
      new Audio('https://www.myinstants.com/media/sounds/the-horror.mp3').play();
    }
  </script>
</body>
</html>
