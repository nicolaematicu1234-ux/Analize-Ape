<!DOCTYPE html>
<html lang="ro">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Analize de Apă – Pachete & Contact</title>
  <meta name="description" content="Analize profesionale de apă potabilă și uzată. Pachete clare, rezultate rapide și consiliere. Cere ofertă sau programează recoltarea."/>
  <style>
    :root{
      --hanna-blue:#005baa;
      --hanna-bg:#e6f0fa;
      --text:#111;
      --muted:#556;
      --ok:#1a7f37;
      --accent:#0ea5e9;
      --card-radius:14px;
    }
    *{box-sizing:border-box}
    body{font-family:Arial, Helvetica, sans-serif;margin:0;color:var(--text);line-height:1.55;background:#fff}
    a{color:var(--hanna-blue);text-decoration:none}
    .container{max-width:1100px;margin:0 auto;padding:0 16px}

    /* Header */
    header{position:sticky;top:0;background:#fff;border-bottom:1px solid #eef;z-index:10}
    .topbar{display:flex;align-items:center;justify-content:space-between;padding:10px 0}
    .brand{display:flex;align-items:center;gap:12px}
    .logo{width:42px;height:42px;border-radius:10px;background:linear-gradient(135deg, var(--hanna-blue), #2d8bee)}
    .brand h1{font-size:18px;margin:0;color:var(--hanna-blue)}
    nav a{margin:0 10px;font-weight:600}
    .cta-btn{background:var(--hanna-blue);color:#fff;padding:10px 16px;border-radius:999px;display:inline-block}
    .cta-btn:hover{opacity:.92}

    /* Hero */
    .hero{background:linear-gradient(180deg,#f7fbff, #fff)}
    .hero .wrap{display:grid;grid-template-columns:1.2fr .8fr;gap:28px;align-items:center;padding:36px 0}
    .hero h2{font-size:36px;margin:8px 0 12px;color:#0b2b52}
    .hero p{color:#334}
    .hero .card{background:var(--hanna-bg);border-left:6px solid var(--hanna-blue);padding:18px;border-radius:var(--card-radius)}
    .hero ul{margin:0;padding-left:18px}
    .hero .img{min-height:260px;border-radius:16px;background:url('https://images.unsplash.com/photo-1470246973918-29a93221c455?q=80&w=1200&auto=format&fit=crop') center/cover no-repeat}

    /* Badges */
    .badges{display:flex;gap:10px;flex-wrap:wrap;margin-top:10px}
    .badge{background:#f2f7ff;border:1px solid #d9e7ff;border-radius:999px;padding:6px 10px;font-size:13px;color:#234}

    /* Packages */
    .section{padding:40px 0}
    .section h3{font-size:28px;margin:0 0 10px;color:#0b2b52}
    .section p.lead{margin-top:0;color:#334}
    .grid{display:grid;grid-template-columns:repeat(3,1fr);gap:18px}
    .card{background:#fff;border:1px solid #e6edf8;border-radius:var(--card-radius);padding:18px}
    .card .title{font-size:18px;color:var(--hanna-blue);margin:0 0 6px}
    .price{font-size:22px;font-weight:800;margin:6px 0}
    .pill{display:inline-block;background:var(--hanna-bg);border-left:5px solid var(--hanna-blue);border-radius:12px;padding:6px 10px;margin:6px 0;color:#123}
    .card ul{padding-left:18px;margin:8px 0}
    .card footer{display:flex;gap:10px;align-items:center;margin-top:10px}
    .outline{border:1px solid var(--hanna-blue);color:var(--hanna-blue);background:transparent}

    /* How it works */
    .steps{display:grid;grid-template-columns:repeat(4,1fr);gap:14px;margin-top:12px}
    .step{background:var(--hanna-bg);border-left:6px solid var(--hanna-blue);border-radius:var(--card-radius);padding:14px}
    .step h4{margin:0 0 6px;color:#0b2b52}
    .step p{margin:0;color:#223}

    /* Trust */
    .trust{display:grid;grid-template-columns:repeat(3,1fr);gap:14px}
    .trust .card{background:var(--hanna-bg)}

    /* FAQ */
    details{border:1px solid #e6edf8;border-radius:12px;padding:12px;margin:8px 0}
    summary{font-weight:700;color:#0b2b52;cursor:pointer}

    /* Contact */
    .contact-wrap{display:grid;grid-template-columns:1fr 1fr;gap:20px}
    form{background:#fff;border:1px solid #e6edf8;border-radius:16px;padding:16px}
    label{font-weight:600;display:block;margin:10px 0 6px}
    input,select,textarea{width:100%;padding:12px;border:1px solid #d9e7ff;border-radius:10px}
    textarea{min-height:120px}
    .submit{margin-top:12px}
    .whatsapp{display:inline-flex;align-items:center;gap:8px;border:1px solid #35b54a;color:#0c7c1c;background:#e9f9ee;padding:10px 14px;border-radius:999px}

    /* Footer */
    footer.site{margin-top:30px;border-top:1px solid #eef;padding:18px 0;color:#445;font-size:14px}

    @media (max-width:980px){
      .hero .wrap{grid-template-columns:1fr}
      .grid{grid-template-columns:1fr}
      .steps{grid-template-columns:1fr 1fr}
      .trust{grid-template-columns:1fr}
      .contact-wrap{grid-template-columns:1fr}
    }
  </style>
  <script>
    // Smooth scroll
    document.addEventListener('DOMContentLoaded', () => {
      document.querySelectorAll('a[href^="#"]').forEach(a => {
        a.addEventListener('click', e => { e.preventDefault(); document.querySelector(a.getAttribute('href')).scrollIntoView({behavior:'smooth'}); });
      });
    });
  </script>
</head>
<body>
  <header>
    <div class="container topbar">
      <div class="brand">
        <div class="logo" aria-hidden="true"></div>
        <h1>Analize de Apă</h1>
      </div>
      <nav>
        <a href="#pachete">Pachete</a>
        <a href="#cum-functioneaza">Cum funcționează</a>
        <a href="#faq">Întrebări</a>
        <a href="#contact" class="cta-btn">Contact</a>
      </nav>
    </div>
  </header>

  <section class="hero">
    <div class="container wrap">
      <div>
        <h2>Analize profesionale de apă – rapid, corect, la preț corect</h2>
        <p>Determinăm parametri esențiali pentru apă potabilă și uzată (pH, conductivitate, TDS, turbiditate, nitrați, amoniu, fier, fosfor, clor, duritate etc.). Alege pachetul potrivit și primești interpretare și recomandări.</p>
        <div class="card">
          <strong>Ce primești:</strong>
          <ul>
            <li>Raport clar cu valori măsurate și limite recomandate</li>
            <li>Consiliere gratuită pentru corectarea problemelor</li>
            <li>Opțional: recoltare la locația ta</li>
          </ul>
          <div class="badges">
            <span class="badge">Rezultate rapide</span>
            <span class="badge">Metode fotometrice & potențiometrice</span>
            <span class="badge">Trasabilitate & calibrare</span>
          </div>
        </div>
      </div>
      <div class="img" role="img" aria-label="Pahar cu apă"></div>
    </div>
  </section>

  <section id="pachete" class="section">
    <div class="container">
      <h3>Pachete de analiză</h3>
      <p class="lead">Dacă ai nevoie de altă combinație de parametri, spune-ne și creăm un pachet personalizat pentru aplicația ta (fântână, puț, piscină, stație de epurare, industrie alimentară etc.).</p>

      <div class="grid">
        <!-- BASIC -->
        <div class="card">
          <div class="pill">Recomandat pentru verificare rapidă</div>
          <h4 class="title">Basic – 12 indicatori</h4>
          <div class="price">de la 199 RON</div>
          <ul>
            <li>pH, Conductivitate, TDS, Turbiditate</li>
            <li>Nitrați, Nitriți, Amoniu</li>
            <li>Clor liber & total / Fier</li>
            <li>Duritate totală, Alcalinitate</li>
          </ul>
          <footer>
            <a href="#contact" class="cta-btn">Cere ofertă</a>
            <a href="#faq" class="outline cta-btn">Detalii</a>
          </footer>
        </div>
        <!-- STANDARD -->
        <div class="card">
          <div class="pill">Cel mai popular</div>
          <h4 class="title">Standard – 29 indicatori</h4>
          <div class="price">de la 399 RON</div>
          <ul>
            <li>Toți din Basic + Fosfați/Fosfor (P, P2O5)</li>
            <li>Cloruri, Sulfați, Sodiu/Potasiu (sumar)</li>
            <li>Metale: Fier, Mangan, Zinc, Cupru</li>
            <li>Oxigen dizolvat / oxidabilitate, Culoare</li>
          </ul>
          <footer>
            <a href="#contact" class="cta-btn">Programează</a>
            <a href="#faq" class="outline cta-btn">Detalii</a>
          </footer>
        </div>
        <!-- PREMIUM -->
        <div class="card">
          <div class="pill">Screening extins</div>
          <h4 class="title">Premium – 50 indicatori</h4>
          <div class="price">de la 699 RON</div>
          <ul>
            <li>Toți din Standard + pachet extins metale</li>
            <li>Parametri suplimentari pentru apă uzată</li>
            <li>Raport detaliat & recomandări personalizate</li>
            <li>Opțional: recoltare la sediul tău</li>
          </ul>
          <footer>
            <a href="#contact" class="cta-btn">Solicită ofertă</a>
            <a href="#faq" class="outline cta-btn">Listă completă</a>
          </footer>
        </div>
      </div>
    </div>
  </section>

  <section id="cum-functioneaza" class="section">
    <div class="container">
      <h3>Cum funcționează</h3>
      <div class="steps">
        <div class="step">
          <h4>1. Alegi pachetul</h4>
          <p>Ne spui aplicația: fântână, puț, piscină, apă uzată, industrie.</p>
        </div>
        <div class="step">
          <h4>2. Recoltare</h4>
          <p>Trimiți proba la laborator sau programăm recoltare la locație.</p>
        </div>
        <div class="step">
          <h4>3. Analiză</h4>
          <p>Determinări cu metode fotometrice, potențiometrice, gravimetrice.</p>
        </div>
        <div class="step">
          <h4>4. Raport & consultanță</h4>
          <p>Primești raport clar + recomandări pentru tratare/corecții.</p>
        </div>
      </div>
    </div>
  </section>

  <section class="section">
    <div class="container">
      <h3>De ce să ne alegi</h3>
      <div class="trust">
        <div class="card">
          <strong>Trasabilitate & Calibrare</strong>
          <p>Echipamente calibrate, proceduri standardizate și controle de calitate.</p>
        </div>
        <div class="card">
          <strong>Rapid & Transparent</strong>
          <p>Termene clare, prețuri vizibile, fără costuri ascunse.</p>
        </div>
        <div class="card">
          <strong>Consiliere utilă</strong>
          <p>Interpretăm rezultatele și îți spunem ce să faci mai departe.</p>
        </div>
      </div>
    </div>
  </section>

  <section id="faq" class="section">
    <div class="container">
      <h3>Întrebări frecvente</h3>
      <details>
        <summary>Cât durează până primesc rezultatele?</summary>
        <p>În mod obișnuit 1–3 zile lucrătoare după primirea probei (în funcție de pachet).</p>
      </details>
      <details>
        <summary>Faceți recoltare la domiciliu/firmă?</summary>
        <p>Da, în anumite orașe/zone. Spune-ne adresa și verificăm disponibilitatea.</p>
      </details>
      <details>
        <summary>Pot alege alți indicatori?</summary>
        <p>Desigur. Creăm pachete personalizate pe aplicația ta și buget.</p>
      </details>
      <details>
        <summary>Emiteți raport pentru autorități?</summary>
        <p>Oferim rapoarte clare cu metode și unități. Pentru rapoarte acreditate RENAR putem redirecționa către parteneri.</p>
      </details>
    </div>
  </section>

  <section id="contact" class="section">
    <div class="container">
      <h3>Cere ofertă sau programează recoltarea</h3>
      <div class="contact-wrap">
        <form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
          <label for="nume">Nume</label>
          <input id="nume" name="nume" required placeholder="Numele tău" />

          <label for="email">Email</label>
          <input id="email" type="email" name="email" required placeholder="email@exemplu.ro" />

          <label for="tel">Telefon</label>
          <input id="tel" type="tel" name="telefon" placeholder="07xx xxx xxx" />

          <label for="loc">Localitate / Județ</label>
          <input id="loc" name="localitate" placeholder="Ex: Cluj-Napoca, Cluj" />

          <label for="pachet">Pachet dorit</label>
          <select id="pachet" name="pachet">
            <option>Basic – 12 indicatori</option>
            <option>Standard – 29 indicatori</option>
            <option>Premium – 50 indicatori</option>
            <option>Personalizat</option>
          </select>

          <label for="msg">Mesaj</label>
          <textarea id="msg" name="mesaj" placeholder="Spune-ne pe scurt aplicația și ce te interesează"></textarea>

          <button class="cta-btn submit" type="submit">Trimite cererea</button>
          <p style="font-size:12px;color:#556;margin:8px 0 0">Prin trimitere ești de acord cu prelucrarea datelor pentru a-ți răspunde solicitării.</p>
        </form>
        <div>
          <div class="card" style="background:var(--hanna-bg)">
            <strong>Contact direct</strong>
            <p style="margin:.5rem 0 0">Telefon: <a href="tel:+40700000000">+40 700 000 000</a></p>
            <p style="margin:.25rem 0 0">Email: <a href="mailto:contact@analize-apa.ro">contact@analize-apa.ro</a></p>
            <p style="margin:.25rem 0 0">WhatsApp: <a class="whatsapp" href="https://wa.me/40700000000" target="_blank" rel="noopener">Scrie pe WhatsApp</a></p>
          </div>
          <div class="card">
            <strong>Program</strong>
            <p>Luni–Vineri: 9:00–17:00</p>
            <p>Recoltări la cerere.</p>
          </div>
          <div class="card">
            <strong>Adresa laborator</strong>
            <p>Str. Exemplu 12, Cluj-Napoca</p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <footer class="site">
    <div class="container" style="display:flex;align-items:center;justify-content:space-between;gap:10px;flex-wrap:wrap">
      <div>© <span id="y"></span> Analize de Apă • Toate drepturile rezervate</div>
      <div style="font-size:13px">
        <a href="#">Politica de confidențialitate</a> · 
        <a href="#">Termeni</a>
      </div>
    </div>
  </footer>
  <script>document.getElementById('y').textContent=new Date().getFullYear()</script>

  <!-- Optional: SEO JSON-LD -->
  <script type="application/ld+json">
  {
    "@context": "https://schema.org",
    "@type": "LocalBusiness",
    "name": "Analize de Apă",
    "url": "https://exemplu.ro",
    "telephone": "+40 700 000 000",
    "address": {
      "@type": "PostalAddress",
      "streetAddress": "Str. Exemplu 12",
      "addressLocality": "Cluj-Napoca",
      "addressCountry": "RO"
    },
    "areaServed": "Romania",
    "sameAs": []
  }
  </script>
</body>
</html>
