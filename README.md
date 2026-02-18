<!doctype html>
<html lang="hu">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Farmi állatállomány</title>
  <style>
    :root{
      --bg1:#f59e0b;
      --bg2:#ef4444;
      --card:#cfe8c9;
      --border:#f59e0b;
      --text:#0f172a;
      --muted:#334155;
      --wrap:1100px;
      --r:14px;
      --shadow:0 10px 30px rgba(0,0,0,.12);
    }
    *{box-sizing:border-box}
    body{
      margin:0;
      font-family:system-ui,-apple-system,Segoe UI,Roboto,Arial,sans-serif;
      color:var(--text);
      background:linear-gradient(180deg,var(--bg1),var(--bg2));
      min-height:100vh;
    }
    .container{max-width:var(--wrap); margin:0 auto; padding:22px 16px 28px}
    header{color:#fff}
    .top{
      display:flex;
      align-items:flex-end;
      justify-content:space-between;
      gap:18px;
      flex-wrap:wrap;
    }
    h1{margin:0; font-size:28px; font-weight:800; letter-spacing:.2px}
    nav{display:flex; gap:14px; flex-wrap:wrap}
    nav a{
      color:#fff;
      text-decoration:none;
      font-weight:600;
      opacity:.92;
      padding:6px 10px;
      border-radius:999px;
      background:rgba(255,255,255,.12);
      backdrop-filter:blur(6px);
    }
    nav a:hover{opacity:1; background:rgba(255,255,255,.18)}
    .lead{margin:8px 0 0; opacity:.9; font-size:13px; max-width:520px}

    .section-title{
      margin:18px 0 10px;
      color:#fff;
      font-weight:800;
      font-size:16px;
      opacity:.95;
    }

    .grid{
      display:grid;
      grid-template-columns:1fr;
      gap:14px;
    }
    @media (min-width: 700px){
      .grid{grid-template-columns:repeat(2,minmax(0,1fr))}
    }
    @media (min-width: 980px){
      .grid{grid-template-columns:repeat(4,minmax(0,1fr))}
    }

    .card{
      background:var(--card);
      border:4px solid var(--border);
      border-radius:var(--r);
      box-shadow:var(--shadow);
      overflow:hidden;
      display:flex;
      flex-direction:column;
      min-height:160px;
    }
    .card-head{
      display:flex;
      justify-content:space-between;
      align-items:flex-start;
      gap:10px;
      padding:12px 12px 6px;
    }
    .id{
      font-weight:900;
      font-size:20px;
      line-height:1;
    }
    .name{
      font-weight:900;
      font-size:18px;
      line-height:1.1;
      text-align:right;
    }
    .meta{
      padding:0 12px 12px;
      display:grid;
      grid-template-columns:1fr auto;
      gap:6px 10px;
      font-size:13px;
      color:var(--muted);
    }
    .meta b{color:var(--text); font-weight:800}
    .divider{
      height:6px;
      background:linear-gradient(90deg, rgba(245,158,11,.0), rgba(245,158,11,.85), rgba(245,158,11,.0));
      margin:0 8px;
      border-radius:999px;
    }

    .footer{
      margin-top:18px;
      padding:14px 16px;
      border-radius:var(--r);
      background:rgba(255,255,255,.12);
      color:#fff;
      backdrop-filter:blur(6px);
    }
    .footer h2{margin:0 0 6px; font-size:16px}
    .footer p{margin:0; font-size:13px; opacity:.92}
  </style>
</head>
<body>
  <div class="container">
    <header>
      <div class="top">
        <div>
          <h1>Farmi állatállomány</h1>
          <div class="lead">Ez az oldal a farm állatállományát mutatja be statikus, reszponzív kártyák formájában.</div>
        </div>
        <nav>
          <a href="#">Állatok</a>
          <a href="#">Leírás</a>
          <a href="#">Kapcsolat</a>
        </nav>
      </div>
      <div class="section-title">Állatok</div>
    </header>

    <main class="grid">
      <article class="card">
        <div class="card-head">
          <div class="id">#1</div>
          <div class="name">Bori</div>
        </div>
        <div class="divider"></div>
        <div class="meta">
          <span>Faj</span><b>Szarvasmarha</b>
          <span>Státusz</span><b>Aktív</b>
          <span>Születési dátum</span><b>2022-04-10</b>
        </div>
      </article>

      <article class="card">
        <div class="card-head">
          <div class="id">#2</div>
          <div class="name">Malacka</div>
        </div>
        <div class="divider"></div>
        <div class="meta">
          <span>Faj</span><b>Sertés</b>
          <span>Státusz</span><b>Aktív</b>
          <span>Születési dátum</span><b>2023-01-05</b>
        </div>
      </article>

      <article class="card">
        <div class="card-head">
          <div class="id">#3</div>
          <div class="name">Fanni</div>
        </div>
        <div class="divider"></div>
        <div class="meta">
          <span>Faj</span><b>Juh</b>
          <span>Státusz</span><b>Inaktív</b>
          <span>Születési dátum</span><b>2021-09-21</b>
        </div>
      </article>

      <article class="card">
        <div class="card-head">
          <div class="id">#4</div>
          <div class="name">Csibész</div>
        </div>
        <div class="divider"></div>
        <div class="meta">
          <span>Faj</span><b>Kecske</b>
          <span>Státusz</span><b>Aktív</b>
          <span>Születési dátum</span><b>2020-11-14</b>
        </div>
      </article>

      <article class="card">
        <div class="card-head">
          <div class="id">#5</div>
          <div class="name">Pöttyös</div>
        </div>
        <div class="divider"></div>
        <div class="meta">
          <span>Faj</span><b>Ló</b>
          <span>Státusz</span><b>Aktív</b>
          <span>Születési dátum</span><b>2019-06-02</b>
        </div>
      </article>

      <article class="card">
        <div class="card-head">
          <div class="id">#6</div>
          <div class="name">Zokni</div>
        </div>
        <div class="divider"></div>
        <div class="meta">
          <span>Faj</span><b>Macska</b>
          <span>Státusz</span><b>Inaktív</b>
          <span>Születési dátum</span><b>2021-02-28</b>
        </div>
      </article>

      <article class="card">
        <div class="card-head">
          <div class="id">#7</div>
          <div class="name">Komondor</div>
        </div>
        <div class="divider"></div>
        <div class="meta">
          <span>Faj</span><b>Kutya</b>
          <span>Státusz</span><b>Aktív</b>
          <span>Születési dátum</span><b>2018-12-09</b>
        </div>
      </article>

      <article class="card">
        <div class="card-head">
          <div class="id">#8</div>
          <div class="name">Kacsa</div>
        </div>
        <div class="divider"></div>
        <div class="meta">
          <span>Faj</span><b>Kacsa</b>
          <span>Státusz</span><b>Aktív</b>
          <span>Születési dátum</span><b>2024-03-17</b>
        </div>
      </article>
    </main>

    <section class="footer">
      <h2>Kapcsolat</h2>
      <p>Ez egy belső, statikus demo oldal; kapcsolati adatok nem kerültek megadásra.</p>
    </section>
  </div>
</body>
</html>