# give-me-a-dolla-
for people that wouldnt mind giving me a dolla
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Give Me a Dollar — Grant's DALL·E Tip Jar</title>
  <link rel="stylesheet" href="/styles.css" />
</head>
<body>
  <main class="container">
    <header>
      <h1>Give Me a Dollar</h1>
      <p class="subtitle">Support Grant — get a quick DALL·E image in return 🎨</p>
    </header>

    <section class="donate">
      <a id="cashapp-link" class="cashapp btn" href="https://cash.app/$1988murdaman" target="_blank" rel="noopener">
        Give $1 on Cash App — <span class="cashtag">$1988murdaman</span>
      </a>
      <p class="small">Tip: After sending a dollar, come back and enter an image prompt below — the site will create an image for you.</p>
    </section>

    <section class="generator">
      <h2>Ask for an image (DALL·E)</h2>

      <label for="prompt">Image prompt</label>
      <textarea id="prompt" rows="4" placeholder="A neon retro city at night, ultra wide, cinematic"></textarea>

      <div class="controls">
        <input id="email" type="text" placeholder="(optional) your email to receive the image link" />
        <button id="generate" class="btn primary">Generate Image</button>
        <button id="copyPrompt" class="btn">Copy Prompt</button>
      </div>

      <div id="status" class="status">Idle</div>

      <div id="result" class="result hidden">
        <h3>Result</h3>
        <div id="imageContainer"></div>
        <a id="downloadLink" class="btn" download="dalle.png">Download Image</a>
      </div>
    </section>

    <footer>
      <small>Deployed from GitHub &mdash; Backend must be deployed (see README).</small>
    </footer>
  </main>

  <script src="/script.js"></script>
</body>
</html>
