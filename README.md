
<html lang="fr">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Prestige Conciergerie 20</title>
  <meta name="description" content="Conciergerie & Nettoyage haut de gamme — Ajaccio • Porticcio • Coti-Chiavari" />
  <style>
    :root{
      --white:#fff;
      --overlay: rgba(0,0,0,.55);
      --overlay-strong: rgba(0,0,0,.70);
      --card: rgba(0,0,0,.38);
      --line: rgba(255,255,255,.18);
      --shadow: 0 18px 60px rgba(0,0,0,.45);
      --radius: 18px;
      --max: 1120px;
    }

    *{ box-sizing:border-box; }
    html,body{ height:100%; }
    body{
      margin:0;
      font-family: system-ui, -apple-system, Segoe UI, Roboto, Arial, sans-serif;
      color: var(--white); /* toutes les écritures en blanc */
      background:
        linear-gradient(180deg, rgba(0,0,0,.55), rgba(0,0,0,.55)),
        url("villa.jpg") center/cover no-repeat fixed;
    }
    a{ color:var(--white); text-decoration:none; }
    a:hover{ text-decoration:underline; }

    /* Top bar (style photo 1 : "Conciergerie" / "Nettoyage") */
    .topbar{
      padding: 14px 18px;
      border-bottom: 1px solid var(--line);
      background: rgba(0,0,0,.22);
      backdrop-filter: blur(6px);
      position: sticky;
      top: 0;
      z-index: 50;
    }
    .topbar-inner{
      max-width: var(--max);
      margin: 0 auto;
      display:flex;
      align-items:center;
      justify-content:space-between;
      gap: 12px;
    }
    .topbar .tag{
      letter-spacing: .14em;
      text-transform: uppercase;
      font-size: 12px;
      opacity: .95;
      padding-bottom: 3px;
      border-bottom: 1px solid rgba(255,255,255,.35);
      white-space: nowrap;
    }
    nav{
      display:flex;
      gap: 18px;
      align-items:center;
      font-size: 14px;
      opacity:.95;
    }
    nav a{ opacity:.95; }
    nav a:hover{ opacity:1; }

    /* Hero */
    .hero{
      max-width: var(--max);
      margin: 0 auto;
      padding: 64px 18px 28px;
      display:grid;
      grid-template-columns: 1.1fr .9fr;
      gap: 22px;
      align-items: center;
    }
    .brand{
      display:flex;
      gap: 16px;
      align-items:center;
    }
    .logo{
      width: 92px;
      height: 92px;
      border-radius: 999px;
      background: rgba(0,0,0,.25);
      border: 1px solid var(--line);
      display:grid;
      place-items:center;
      box-shadow: var(--shadow);
    }
    .logo img{
      width: 74px;
      height: 74px;
      object-fit: contain;
      display:block;
      filter: drop-shadow(0 10px 24px rgba(0,0,0,.35));
    }
    .title h1{
      margin:0;
      font-size: clamp(32px, 4.2vw, 54px);
      line-height: 1.05;
      letter-spacing: .08em;
      text-transform: uppercase;
    }
    .title p{
      margin: 10px 0 0;
      font-size: 16px;
      opacity: .92;
      letter-spacing: .06em;
    }

    .hero-card{
      border: 1px solid var(--line);
      border-radius: var(--radius);
      background: var(--card);
      box-shadow: var(--shadow);
      padding: 18px 18px 16px;
      backdrop-filter: blur(8px);
    }
    .hero-card h2{
      margin: 0 0 10px;
      font-size: 16px;
      letter-spacing: .12em;
      text-transform: uppercase;
      opacity: .95;
    }
    .hero-card ul{
      margin:0;
      padding:0 0 0 18px;
      display:grid;
      gap: 8px;
      opacity:.95;
      line-height: 1.5;
    }

    .cta{
      display:flex;
      gap: 10px;
      flex-wrap: wrap;
      margin-top: 18px;
    }
    .btn{
      display:inline-flex;
      align-items:center;
      justify-content:center;
      gap:10px;
      padding: 12px 16px;
      border-radius: 999px;
      border: 1px solid rgba(255,255,255,.28);
      background: rgba(0,0,0,.35);
      color: var(--white);
      font-weight: 600;
      letter-spacing: .02em;
      transition: transform .15s ease, background .15s ease, border-color .15s ease;
    }
    .btn:hover{
      transform: translateY(-1px);
      background: rgba(0,0,0,.48);
      border-color: rgba(255,255,255,.45);
      text-decoration:none;
    }
    .btn.secondary{
      background: rgba(255,255,255,.10);
    }

    /* Section title bandeau (style "NOS SERVICES") */
    .band{
      margin: 26px 0 0;
      background: var(--overlay-strong);
      border-top: 1px solid rgba(255,255,255,.12);
      border-bottom: 1px solid rgba(255,255,255,.12);
    }
    .band-inner{
      max-width: var(--max);
      margin: 0 auto;
      padding: 14px 18px;
      display:flex;
      align-items:center;
      justify-content:center;
      gap: 16px;
    }
    .band-inner .line{
      height:1px;
      width: min(160px, 18vw);
      background: rgba(255,255,255,.35);
      opacity:.8;
    }
    .band-inner h3{
      margin:0;
      font-size: 18px;
      letter-spacing: .18em;
      text-transform: uppercase;
    }

    /* Services */
    .section{
      max-width: var(--max);
      margin: 0 auto;
      padding: 24px 18px 10px;
    }
    .grid{
      display:grid;
      grid-template-columns: repeat(12, 1fr);
      gap: 14px;
    }
    .service{
      grid-column: span 6;
      border-radius: var(--radius);
      border: 1px solid var(--line);
      background: rgba(0,0,0,.30);
      backdrop-filter: blur(8px);
      box-shadow: 0 16px 40px rgba(0,0,0,.35);
      padding: 16px 16px 14px;
      display:flex;
      gap: 12px;
      align-items:flex-start;
      min-height: 98px;
    }
    .icon{
      width: 44px;
      height: 44px;
      border-radius: 12px;
      border: 1px solid rgba(255,255,255,.18);
      background: rgba(255,255,255,.08);
      display:grid;
      place-items:center;
      flex: 0 0 auto;
    }
    .service h4{
      margin: 0 0 4px;
      font-size: 15px;
      letter-spacing: .04em;
      text-transform: uppercase;
    }
    .service p{
      margin:0;
      opacity:.92;
      line-height: 1.45;
      font-size: 14px;
    }
    svg{ stroke: #fff; }

    /* Contact */
    .contact-wrap{
      margin-top: 18px;
      display:grid;
      grid-template-columns: 1fr 1fr;
      gap: 14px;
    }
    .panel{
      border-radius: var(--radius);
      border: 1px solid var(--line);
      background: rgba(0,0,0,.36);
      backdrop-filter: blur(8px);
      box-shadow: var(--shadow);
      padding: 18px;
    }
    .panel h3{
      margin:0 0 10px;
      letter-spacing: .14em;
      text-transform: uppercase;
      font-size: 16px;
    }
    .panel .muted{ opacity:.92; line-height:1.6; }

    footer{
      margin-top: 26px;
      padding: 22px 18px 28px;
      background: rgba(0,0,0,.55);
      border-top: 1px solid rgba(255,255,255,.12);
    }
    .footer-inner{
      max-width: var(--max);
      margin: 0 auto;
      display:flex;
      flex-wrap: wrap;
      gap: 10px 18px;
      justify-content: space-between;
      align-items:center;
      opacity:.92;
    }

    /* Responsive */
    @media (max-width: 920px){
      .hero{ grid-template-columns: 1fr; padding-top: 46px; }
      .service{ grid-column: span 12; }
      .contact-wrap{ grid-template-columns: 1fr; }
      nav{ display:none; }
    }
  </style>
</head>

<body>
  <header class="topbar">
    <div class="topbar-inner">
      <div class="tag">Conciergerie</div>

      <nav aria-label="Navigation">
        <a href="#services">Services</a>
        <a href="#zones">Zones</a>
        <a href="#contact">Contact</a>
      </nav>

      <div class="tag">Nettoyage</div>
    </div>
  </header>

  <main>
    <section class="hero" id="accueil">
      <div>
        <div class="brand">
          <div class="logo" aria-label="Logo Prestige Conciergerie 20">
            <img src="logo.png" alt="Logo Prestige Conciergerie 20">
          </div>
          <div class="title">
            <h1>Prestige Conciergerie 20</h1>
            <p>Ajaccio • Porticcio • Coti-Chiavari</p>
          </div>
        </div>

        <div class="cta">
          <a class="btn" href="tel:+33682916874" aria-label="Appeler">📞 06 82 91 68 74</a>
          <a class="btn secondary" href="mailto:prestige.residence20@gmail.com" aria-label="Envoyer un email">✉️ prestige.residence20@gmail.com</a>
        </div>
      </div>

      <aside class="hero-card" id="zones">
        <h2>Devis gratuit</h2>
        <ul>
          <li>Gestion complète des annonces (Airbnb, Booking, etc.)</li>
          <li>Nettoyage professionnel & préparation haut de gamme</li>
          <li>Linge : fourniture, blanchisserie, repassage</li>
          <li>Entretien intérieur/extérieur & gardiennage</li>
          <li>Courses, transports & livraisons</li>
        </ul>
      </aside>
    </section>

    <div class="band" id="services">
      <div class="band-inner">
        <span class="line" aria-hidden="true"></span>
        <h3>Nos services</h3>
        <span class="line" aria-hidden="true"></span>
      </div>
    </div>

    <section class="section">
      <div class="grid">
        <article class="service">
          <div class="icon" aria-hidden="true">
            <!-- Clipboard -->
            <svg width="22" height="22" viewBox="0 0 24 24" fill="none" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
              <path d="M9 5h6" />
              <path d="M9 3h6a2 2 0 0 1 2 2v2H7V5a2 2 0 0 1 2-2z" />
              <path d="M7 7h10v14H7z" />
              <path d="M9 11h6" />
              <path d="M9 15h6" />
            </svg>
          </div>
          <div>
            <h4>Gestion des annonces</h4>
            <p>Création, optimisation et suivi (Airbnb, Booking, etc.). Communication voyageurs et coordination des arrivées/départs.</p>
          </div>
        </article>

        <article class="service">
          <div class="icon" aria-hidden="true">
            <!-- Spray -->
            <svg width="22" height="22" viewBox="0 0 24 24" fill="none" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
              <path d="M10 4h4" />
              <path d="M12 4v4" />
              <path d="M9 8h6" />
              <path d="M8 9h8l-1 12H9L8 9z" />
              <path d="M5 12h0" />
              <path d="M5 15h0" />
              <path d="M5 18h0" />
            </svg>
          </div>
          <div>
            <h4>Nettoyage haut de gamme</h4>
            <p>Nettoyage professionnel, contrôle qualité, consommables, mise en place soignée pour une expérience premium.</p>
          </div>
        </article>

        <article class="service">
          <div class="icon" aria-hidden="true">
            <!-- Hanger -->
            <svg width="22" height="22" viewBox="0 0 24 24" fill="none" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
              <path d="M12 6a2 2 0 1 0-2 2" />
              <path d="M10 8c0 2-6 4-8 6h20c-2-2-8-4-8-6" />
              <path d="M4 14l8 7 8-7" />
            </svg>
          </div>
          <div>
            <h4>Linge & blanchisserie</h4>
            <p>Draps, serviettes, remplacement, entretien et repassage. Gestion complète entre chaque séjour.</p>
          </div>
        </article>

        <article class="service">
          <div class="icon" aria-hidden="true">
            <!-- Home -->
            <svg width="22" height="22" viewBox="0 0 24 24" fill="none" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
              <path d="M3 10l9-7 9 7" />
              <path d="M5 10v10h14V10" />
              <path d="M9 20v-6h6v6" />
            </svg>
          </div>
          <div>
            <h4>Entretien & gardiennage</h4>
            <p>Suivi intérieur/extérieur, passages réguliers, petits contrôles et coordination d’interventions.</p>
          </div>
        </article>

        <article class="service">
          <div class="icon" aria-hidden="true">
            <!-- Car -->
            <svg width="22" height="22" viewBox="0 0 24 24" fill="none" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
              <path d="M3 16l1-5a3 3 0 0 1 3-2h10a3 3 0 0 1 3 2l1 5" />
              <path d="M5 16h14" />
              <path d="M7 16v3" />
              <path d="M17 16v3" />
              <circle cx="7" cy="19" r="1" />
              <circle cx="17" cy="19" r="1" />
            </svg>
          </div>
          <div>
            <h4>Courses & livraisons</h4>
            <p>Courses d’arrivée, livraisons, transports et services sur demande pour simplifier la logistique.</p>
          </div>
        </article>

        <article class="service">
          <div class="icon" aria-hidden="true">
            <!-- Key -->
            <svg width="22" height="22" viewBox="0 0 24 24" fill="none" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
              <circle cx="8" cy="15" r="3" />
              <path d="M11 15h10" />
              <path d="M18 15v3" />
              <path d="M21 15v2" />
            </svg>
          </div>
          <div>
            <h4>Check-in / Check-out</h4>
            <p>Accueil, remise des clés, assistance voyageurs, état des lieux et coordination des rotations.</p>
          </div>
        </article>
      </div>

      <div class="contact-wrap" id="contact">
        <div class="panel">
          <h3>Zones couvertes</h3>
          <p class="muted">
            Ajaccio • Porticcio • Coti-Chiavari<br/>
            (et alentours selon demande)
          </p>
        </div>

        <div class="panel">
          <h3>Contact</h3>
          <p class="muted">
            Téléphone : <a href="tel:+33682916874">06 82 91 68 74</a><br/>
            Email : <a href="mailto:prestige.residence20@gmail.com">prestige.residence20@gmail.com</a><br/>
            <span style="opacity:.9;">Devis gratuit — réponse rapide</span>
          </p>
          <div class="cta" style="margin-top:12px;">
            <a class="btn" href="mailto:prestige.residence20@gmail.com?subject=Demande%20de%20devis%20-%20Prestige%20Conciergerie%2020&body=Bonjour%2C%0A%0AJe%20souhaite%20un%20devis%20pour%20la%20conciergerie%20de%20mon%20logement%20%C3%A0%20%3A%0A-%20Ville%20%3A%0A-%20Type%20de%20bien%20%3A%0A-%20Nombre%20de%20couchages%20%3A%0A-%20Fr%C3%A9quence%20des%20s%C3%A9jours%20%3A%0A%0AMerci%20%21">Demander un devis</a>
          </div>
        </div>
      </div>
    </section>

    <footer>
      <div class="footer-inner">
        <div>© <span id="year"></span> Prestige Conciergerie 20 — Conciergerie & Nettoyage</div>
        <div>Ajaccio • Porticcio • Coti-Chiavari</div>
      </div>
    </footer>
  </main>

  <script>
    document.getElementById("year").textContent = new Date().getFullYear();
  </script>
</body>
</html>
