# charity
charity water landing page
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Change Starts With Us — Campus Clean Water</title>
  <!-- Beginner‑friendly, HTML + CSS only. Replace image URLs later. -->
  <style>
    /* =====================
       BRAND TOKENS
       ===================== */
    :root{
      --brand-yellow:#FFD200;      /* CTA background */
      --brand-yellow-d:#E6BD00;    /* CTA hover */
      --bg:#ffffff;                /* page background */
      --ink:#0B1220;               /* main text */
      --ink-dim:#3C4758;           /* muted text */
      --panel:#F6FAFF;             /* light blue stats background */
      --divider:#E6EAF0;           /* subtle borders */
      --radius:14px;               /* rounded corners */
      --max-w:1100px;              /* content width */
      --font-head: system-ui, -apple-system, Segoe UI, Roboto, Helvetica, Arial, sans-serif;
      --font-body: system-ui, -apple-system, Segoe UI, Roboto, Helvetica, Arial, sans-serif;
    }

    /* =====================
       GLOBAL STYLES
       ===================== */
    *{box-sizing:border-box}
    html,body{margin:0;padding:0}
    body{font-family:var(--font-body); color:var(--ink); background:var(--bg); line-height:1.6}
    img{max-width:100%; display:block}
    a{text-decoration:none; color:inherit}
    h1,h2,h3{font-family:var(--font-head); line-height:1.2; margin:0 0 .6rem}
    p{margin:0 0 1rem; color:var(--ink-dim)}
    .container{max-width:var(--max-w); margin:0 auto; padding:0 1rem}
    .section{padding:3rem 0}
    .btn{display:inline-block; background:var(--brand-yellow); color:#0b0b0b; font-weight:700; padding:.9rem 1.2rem; border-radius:10px; box-shadow:0 2px 0 rgba(0,0,0,.1)}
    .btn:hover{background:var(--brand-yellow-d)}
    .grid{display:grid; gap:1.25rem}

    /* =====================
       HEADER (simple)
       ===================== */
    header{position:sticky; top:0; background:#ffffffcc; backdrop-filter:saturate(180%) blur(8px); border-bottom:1px solid var(--divider); z-index:5}
    .nav{display:flex; align-items:center; justify-content:space-between; padding:.75rem 0}
    .logo{font-weight:800}
    .nav .links{display:flex; gap:1rem}

    /* =====================
       TOP HERO BANNER (full width image with floating CTA)
       ===================== */
    .hero-banner{position:relative}
    .hero-banner img{width:100%; height:340px; object-fit:cover}
    .hero-banner .cta-float{position:absolute; right:clamp(1rem, 4vw, 3rem); bottom:clamp(1rem, 4vw, 2rem)}

    /* =====================
       FEATURE SPLIT (image left, copy right)
       ===================== */
    .feature{align-items:center}
    .feature .visual{border-radius:var(--radius); overflow:hidden}
    .feature h2{font-size:clamp(1.8rem, 3.5vw, 2.6rem)}

    /* =====================
       STATS STRIP
       ===================== */
    .stats{background:var(--panel); border-top:1px solid var(--divider); border-bottom:1px solid var(--divider)}
    .stats .items{grid-template-columns:1fr; padding-top:.5rem}
    .stat{display:flex; gap:.9rem; align-items:flex-start; padding:1rem 0; border-top:1px solid var(--divider)}
    .stat:first-child{border-top:0}
    .stat strong{font-size:1.1rem; color:var(--ink)}

    /* Simple icon circles */
    .icon{width:42px; height:42px; border-radius:50%; background:#E7F3FF; display:grid; place-items:center; font-weight:800}

    /* =====================
       STUDENT VOICES
       ===================== */
    .voices .polaroid{background:#fff; border:1px solid var(--divider); border-radius:10px; padding:.75rem; max-width:360px}
    .voices h3{font-size:clamp(1.6rem, 3vw, 2.2rem)}

    /* =====================
       RESPONSIVE
       ===================== */
    @media (min-width: 768px){
      .feature{grid-template-columns:1.2fr 1fr}
      .stats .items{grid-template-columns: repeat(3, 1fr)}
      .voices .wrap{grid-template-columns: 1fr 1.1fr; align-items:center}
    }
  </style>
</head>
<body>
  <!-- ===================== HEADER ===================== -->
  <header>
    <div class="container nav">
      <a class="logo" href="#">Campus Water</a>
      <nav class="links">
        <a href="#impact">Impact</a>
        <a href="#voices">Student Voices</a>
        <a href="#fundraise" class="btn">Start a Campus Fundraiser</a>
      </nav>
    </div>
  </header>

  <main>
    <!-- ===================== HERO BANNER ===================== -->
    <section class="hero-banner">
      <!-- Replace this hero image with your own -->
      <img src="https://images.unsplash.com/photo-1518611012118-696072aa579a?q=80&w=1800&auto=format&fit=crop" alt="Students celebrating at a campus fundraiser" />
      <div class="cta-float">
        <a class="btn" href="#fundraise">Join the Movement</a>
      </div>
    </section>

    <!-- ===================== FEATURE SPLIT ===================== -->
    <section class="section">
      <div class="container grid feature">
        <div class="visual">
          <!-- Replace with your group image -->
          <img src="https://images.unsplash.com/photo-1604881991720-f91add269bed?q=80&w=1200&auto=format&fit=crop" alt="Students holding a sign: Walk for Water" />
        </div>
        <div>
          <h2>Change Starts With Us.</h2>
          <p>771 million people don't have clean water. But change starts with us. Every campus event, every $20 donation, every shared post makes ripples of impact.</p>
          <p>Gather your club, class, or team and turn energy into access to clean water for communities around the world.</p>
          <p><a class="btn" href="#fundraise">Start a Campus Fundraiser</a></p>
        </div>
      </div>
    </section>

    <!-- ===================== STATS STRIP ===================== -->
    <section id="impact" class="section stats">
      <div class="container">
        <div class="grid items">
          <div class="stat">
            <div class="icon" aria-hidden="true">💧</div>
            <div>
              <strong>$40 = clean water for one person.</strong>
              <p>Small gifts add up quickly—your campus can change lives.</p>
            </div>
          </div>
          <div class="stat">
            <div class="icon" aria-hidden="true">100%</div>
            <div>
              <strong>100% of donations go directly to clean water projects</strong>
              <p>Operational costs are covered separately so your gift goes further.</p>
            </div>
          </div>
          <div class="stat">
            <div class="icon" aria-hidden="true">🚰</div>
            <div>
              <strong>150K+ projects funded</strong>
              <p>Be part of the next chapter with your campus community.</p>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- ===================== STUDENT VOICES ===================== -->
    <section id="voices" class="section voices">
      <div class="container grid wrap">
        <div class="polaroid">
          <!-- Replace with your student portrait -->
          <img src="https://images.unsplash.com/photo-1524504388940-b1c1722653e1?q=80&w=900&auto=format&fit=crop" alt="Student holding a donation sign" />
        </div>
        <div>
          <h3>Student Voices</h3>
          <p style="color:var(--ink)"><em>“Raising $500 with my campus club was easier than I thought — and now 12 people have clean water for life.”</em></p>
          <p><strong>Maya</strong>, Ohio State University</p>
        </div>
      </div>
    </section>

    <!-- ===================== FINAL CTA ===================== -->
    <section id="fundraise" class="section" style="padding-top:0">
      <div class="container" style="text-align:center">
        <h2>Ready to take the first step?</h2>
        <p>Launch a fundraiser in minutes. Rally your friends. Change lives.</p>
        <p><a class="btn" href="#">Start a Campus Fundraiser</a></p>
      </div>
    </section>
  </main>

  <footer class="section" style="padding:2rem 0; border-top:1px solid var(--divider)">
    <div class="container" style="color:var(--ink-dim); font-size:.95rem">
      <p><strong>Campus Water</strong> • © 2025 • All rights reserved.</p>
    </div>
  </footer>
</body>
</html>

