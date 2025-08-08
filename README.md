<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Jeeban Bohara | Portfolio</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <style>
    body {
      margin: 0;
      padding: 40px 20px;
      background: #0f1117;
      color: white;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }

    h1, h2, h3 {
      margin: 0;
      padding: 0;
    }

    .intro {
      text-align: center;
      margin-bottom: 60px;
    }

    .intro h1 {
      font-size: 3rem;
      color: #00ffe7;
      text-shadow: 0 0 8px #00ffe7;
    }

    .intro h2 {
      font-size: 1.6rem;
      color: #00f7ff;
      margin-top: 10px;
    }

    .animated-text {
      margin-top: 15px;
      font-size: 1.3rem;
      color: #3399ff;
      height: 30px;
      overflow: hidden;
      white-space: nowrap;
      border-right: 2px solid #3399ff;
      width: fit-content;
      margin-left: auto;
      margin-right: auto;
      animation: typing 3s steps(40, end) infinite, blink 0.75s step-end infinite;
    }

    @keyframes typing {
      0%, 100% { width: 0 }
      20%, 80% { width: 100% }
    }

    @keyframes blink {
      from, to { border-color: transparent }
      50% { border-color: #3399ff }
    }

    .section {
      margin-bottom: 50px;
    }

    .section-title {
      font-size: 1.4rem;
      margin-bottom: 10px;
    }

    .divider {
      height: 2px;
      background: linear-gradient(to right, #444, #888, #444);
      margin: 15px 0 25px;
      border-radius: 5px;
    }

    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(120px, 1fr));
      gap: 20px;
    }

    .item {
      background-color: #1c1e26;
      border-radius: 10px;
      padding: 15px 10px;
      text-align: center;
      transition: transform 0.2s ease, background 0.3s ease;
    }

    .item:hover {
      transform: scale(1.05);
      background-color: #2a2d3a;
    }

    .item img {
      width: 40px;
      height: 40px;
      margin-bottom: 8px;
    }

    .item span {
      font-size: 0.9rem;
      display: block;
    }
  </style>
</head>
<body>

  <div class="intro">
    <h1>👋 Hi, I'm Jeeban Bohara</h1>
    <h2>💻 Computer Engineering Student — FWU SOE</h2>
    <div class="animated-text" id="type-text">Crafting clean & efficient code is my passion.</div>
  </div>

  <!-- Languages & Frameworks -->
  <div class="section">
    <div class="section-title">🛠️ Languages & Frameworks</div>
    <div class="divider"></div>
    <div class="grid">
      <div class="item"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg"><span>JavaScript</span></div>
      <div class="item"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/typescript/typescript-original.svg"><span>TypeScript</span></div>
      <div class="item"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg"><span>Python</span></div>
      <div class="item"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/c/c-original.svg"><span>C</span></div>
      <div class="item"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/cplusplus/cplusplus-original.svg"><span>C++</span></div>
      <div class="item"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/react/react-original.svg"><span>React</span></div>
      <div class="item"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vuejs/vuejs-original.svg"><span>Vue</span></div>
      <div class="item"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nodejs/nodejs-original.svg"><span>Node.js</span></div>
      <div class="item"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/express/express-original.svg"><span>Express</span></div>
      <div class="item"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/laravel/laravel-plain.svg"><span>Laravel</span></div>
    </div>
  </div>

  <!-- Databases & Cloud -->
  <div class="section">
    <div class="section-title">☁️ Databases & Cloud</div>
    <div class="divider"></div>
    <div class="grid">
      <div class="item"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/mongodb/mongodb-original.svg"><span>MongoDB</span></div>
      <div class="item"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/mysql/mysql-original.svg"><span>MySQL</span></div>
      <div class="item"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/redis/redis-original.svg"><span>Redis</span></div>
      <div class="item"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/amazonwebservices/amazonwebservices-original.svg"><span>AWS</span></div>
      <div class="item"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/docker/docker-original.svg"><span>Docker</span></div>
      <div class="item"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nginx/nginx-original.svg"><span>Nginx</span></div>
      <div class="item"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vercel/vercel-original.svg"><span>Vercel</span></div>
      <div class="item"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/firebase/firebase-plain.svg"><span>Firebase</span></div>
      <div class="item"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/heroku/heroku-original.svg"><span>Heroku</span></div>
    </div>
  </div>

  <script>
    const texts = [
      "Crafting clean & efficient code is my passion.",
      "Designing user-centric experiences excites me.",
      "I enjoy storytelling through creative editing.",
      "Cricket fuels my competitive spirit & teamwork."
    ];

    let count = 0;
    const textElement = document.getElementById("type-text");

    setInterval(() => {
      textElement.textContent = texts[count % texts.length];
      count++;
    }, 4000);
  </script>

</body>
</html>
