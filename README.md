# give-me-a-dolla-
for people that wouldnt mind giving me a dolla
<!-- index.html -->
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Give Me a Dollar</title>
  <style>
    /* page */
    html,body{height:100%;margin:0;font-family:Inter, system-ui, -apple-system, "Segoe UI", Roboto, Arial;}
    body{
      background:#000; /* black background */
      color:#fff;
      display:flex;
      align-items:center;
      justify-content:center;
    }

    /* card */
    .wrap{
      text-align:center;
      padding:36px;
    }
    h1{
      margin:0 0 18px 0;
      font-size:28px;
      color:#9ef08f; /* pale green title */
      letter-spacing:0.6px;
    }
    p.sub{
      margin:0 0 26px 0;
      color:#9aa0a6;
      font-size:14px;
    }

    /* dollar button */
    .dollar-btn{
      --green:#16a34a; /* button green */
      display:inline-flex;
      align-items:center;
      gap:12px;
      background:linear-gradient(180deg,var(--green), #0f7f36);
      color:#00110a;
      border-radius:48px;
      padding:14px 28px;
      text-decoration:none;
      font-weight:700;
      font-size:18px;
      box-shadow: 0 10px 30px rgba(22,163,74,0.18), inset 0 -4px 8px rgba(255,255,255,0.05);
      border: 1px solid rgba(0,0,0,0.15);
      transition: transform .12s ease, box-shadow .12s ease;
    }
    .dollar-btn:hover{ transform: translateY(-3px); box-shadow: 0 18px 40px rgba(22,163,74,0.2); }

    .dollar-icon{
      width:36px;height:36px;border-radius:999px;
      background:rgba(255,255,255,0.15);
      display:inline-flex;align-items:center;justify-content:center;
      color:white;font-weight:800;font-size:20px;
      box-shadow: 0 2px 6px rgba(0,0,0,0.15);
    }

    /* small foot */
    .foot{ margin-top:18px;color:#6b7280;font-size:13px; }
    @media (max-width:420px){
      .dollar-btn{ padding:12px 18px; font-size:16px; gap:10px; }
    }
  </style>
</head>
<body>
  <div class="wrap">
    <h1>Give Me a Dollar</h1>
    <p class="sub">Tap the button below — it opens Cash App and pre-fills $1.00 to my cashtag.</p>

    <!--
      Cash App deep link format (works on web and mobile):
      https://cash.app/$CASHTAG/AMOUNT
      Example below uses $1988murdaman and amount 1.00
    -->
    <a class="dollar-btn" id="cashBtn" href="https://cash.app/$1988murdaman/1.00" target="_blank" rel="noopener noreferrer">
      <span class="dollar-icon">$</span>
      <span>Give Me a Dollar</span>
    </a>

    <div class="foot">Opens Cash App — make sure your device has the Cash App installed or it will open the web profile.</div>
  </div>

  <script>
    // optional: slightly nicer behavior on desktop (confirm before opening)
    document.getElementById('cashBtn').addEventListener('click', function(e){
      // no blocking behavior — let it open. This listener is here if you want to add analytics later.
    });
  </script>
</body>
</html>
