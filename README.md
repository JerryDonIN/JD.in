# JD.in
My insta ACCAUNT follow me
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>JD.in | Jerrydon</title>
  <meta name="description" content="JD.in - Official website of Jerrydon">

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: Arial, Helvetica, sans-serif;
    }

    body {
      min-height: 100vh;
      background:
        radial-gradient(circle at 20% 20%, #3b0764 0%, transparent 35%),
        radial-gradient(circle at 80% 80%, #0f3b63 0%, transparent 35%),
        #050505;
      color: white;
      display: flex;
      align-items: center;
      justify-content: center;
      overflow: hidden;
    }

    .orb {
      position: fixed;
      width: 250px;
      height: 250px;
      border-radius: 50%;
      filter: blur(80px);
      opacity: 0.35;
      pointer-events: none;
    }

    .orb.one {
      background: #8b5cf6;
      top: -80px;
      left: -80px;
    }

    .orb.two {
      background: #06b6d4;
      bottom: -100px;
      right: -80px;
    }

    .container {
      width: min(92%, 430px);
      text-align: center;
      padding: 35px 25px;
      border: 1px solid rgba(255,255,255,0.12);
      border-radius: 30px;
      background: rgba(255,255,255,0.07);
      backdrop-filter: blur(20px);
      -webkit-backdrop-filter: blur(20px);
      box-shadow: 0 25px 80px rgba(0,0,0,0.45);
      animation: appear 0.8s ease;
    }

    @keyframes appear {
      from {
        opacity: 0;
        transform: translateY(25px) scale(0.96);
      }

      to {
        opacity: 1;
        transform: translateY(0) scale(1);
      }
    }

    .logo {
      width: 100px;
      height: 100px;
      margin: 0 auto 18px;
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 38px;
      font-weight: 900;
      letter-spacing: -3px;
      background: linear-gradient(135deg, #ffffff, #9ca3af);
      color: #080808;
      border: 4px solid rgba(255,255,255,0.15);
      box-shadow:
        0 0 35px rgba(255,255,255,0.15),
        inset 0 0 20px rgba(0,0,0,0.15);
    }

    h1 {
      font-size: 34px;
      margin-bottom: 7px;
      letter-spacing: -1px;
    }

    .username {
      color: #bdbdbd;
      font-size: 16px;
      margin-bottom: 18px;
    }

    .verified {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      width: 18px;
      height: 18px;
      margin-left: 5px;
      border-radius: 50%;
      background: #3897f0;
      color: white;
      font-size: 11px;
      font-weight: bold;
      vertical-align: middle;
    }

    .bio {
      color: #d1d1d1;
      line-height: 1.6;
      font-size: 15px;
      margin: 0 auto 28px;
      max-width: 330px;
    }

    .links {
      display: flex;
      flex-direction: column;
      gap: 13px;
    }

    .btn {
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 10px;
      width: 100%;
      padding: 16px 20px;
      border-radius: 15px;
      text-decoration: none;
      color: white;
      font-size: 16px;
      font-weight: 700;
      border: 1px solid rgba(255,255,255,0.12);
      background: rgba(255,255,255,0.09);
      transition: 0.25s ease;
      cursor: pointer;
    }

    .btn:hover {
      transform: translateY(-3px);
      background: rgba(255,255,255,0.16);
      box-shadow: 0 10px 30px rgba(0,0,0,0.25);
    }

    .btn:active {
      transform: scale(0.97);
    }

    .instagram {
      background: linear-gradient(
        135deg,
        #833ab4,
        #fd1d1d,
        #fcb045
      );
      border: none;
      box-shadow: 0 10px 30px rgba(225,48,108,0.25);
    }

    .instagram:hover {
      box-shadow: 0 15px 40px rgba(225,48,108,0.4);
      filter: brightness(1.08);
    }

    .icon {
      font-size: 21px;
    }

    footer {
      margin-top: 27px;
      color: #777;
      font-size: 12px;
    }

    footer span {
      color: #aaa;
    }

    @media (max-width: 480px) {
      .container {
        padding: 30px 20px;
        border-radius: 25px;
      }

      .logo {
        width: 88px;
        height: 88px;
        font-size: 33px;
      }

      h1 {
        font-size: 30px;
      }
    }
  </style>
</head>

<body>

  <div class="orb one"></div>
  <div class="orb two"></div>

  <main class="container">

    <div class="logo">JD</div>

    <h1>
      Jerrydon
      <span class="verified">✓</span>
    </h1>

    <div class="username">@jerrydon.official</div>

    <p class="bio">
      Welcome to JD.in — the official home of Jerrydon.
      Follow me on Instagram and stay connected.
    </p>

    <div class="links">

      <!-- YOUR INSTAGRAM LINK -->
      <a
        class="btn instagram"
        href="https://www.instagram.com/jerrydon.official?stkn=NnNjZ2duZmlwbnRk"
        target="_blank"
        rel="noopener noreferrer"
      >
        <span class="icon">◎</span>
        Follow on Instagram
      </a>

      <a class="btn" href="#about" onclick="showAbout(event)">
        <span class="icon">✦</span>
        About Jerrydon
      </a>

      <button class="btn" onclick="shareWebsite()">
        <span class="icon">↗</span>
        Share JD.in
      </button>

    </div>

    <footer>
      © <span id="year"></span> JD.in · All rights reserved.
    </footer>

  </main>

  <script>
    document.getElementById("year").textContent =
      new Date().getFullYear();

    function showAbout(event) {
      event.preventDefault();

      alert(
        "Welcome to JD.in!\\n\\n" +
        "Official profile: @jerrydon.official\\n\\n" +
        "Follow Jerrydon on Instagram to stay connected."
      );
    }

    async function shareWebsite() {

      const shareData = {
        title: "JD.in | Jerrydon",
        text: "Check out the official JD.in website!",
        url: window.location.href
      };

      try {
        if (navigator.share) {
          await navigator.share(shareData);
        } else {
          await navigator.clipboard.writeText(window.location.href);
          alert("Website link copied!");
        }
      } catch (error) {
        console.log("Share cancelled.");
      }
    }
  </script>

</body>
</html>
