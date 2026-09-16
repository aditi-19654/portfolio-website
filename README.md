
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Aniket Express Cargo Logistics | Roorkee · Dehradun · Delhi</title>
<meta name="description" content="Aniket Express Cargo Logistics — reliable freight & cargo transport across the Roorkee, Dehradun and Delhi corridor.">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Oswald:wght@400;500;600;700&family=Inter:wght@400;500;600;700;800&family=JetBrains+Mono:wght@400;600&display=swap" rel="stylesheet">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
<style>
  :root{
    --asphalt:#12181F;
    --panel:#1B2432;
    --panel-2:#212C3D;
    --amber:#FF8A1E;
    --amber-dark:#E56F00;
    --green:#3CB878;
    --paper:#F5F3EE;
    --gray:#8A93A0;
    --line: rgba(245,243,238,0.09);
  }
  *{margin:0;padding:0;box-sizing:border-box;}
  html{scroll-behavior:smooth;}
  body{
    background:var(--asphalt);
    color:var(--paper);
    font-family:'Inter',sans-serif;
    overflow-x:hidden;
  }
  h1,h2,h3,.display{
    font-family:'Oswald',sans-serif;
    text-transform:uppercase;
    letter-spacing:0.02em;
    font-weight:600;
  }
  .mono{font-family:'JetBrains Mono',monospace;}
  a{color:inherit;text-decoration:none;}
  .wrap{max-width:1180px;margin:0 auto;padding:0 24px;}
  ::selection{background:var(--amber);color:var(--asphalt);}

  /* -------- reveal on scroll -------- */
  .reveal{opacity:0;transform:translateY(28px);transition:opacity .8s cubic-bezier(.2,.7,.2,1),transform .8s cubic-bezier(.2,.7,.2,1);}
  .reveal.in{opacity:1;transform:translateY(0);}

  /* -------- nav -------- */
  header{
    position:fixed;top:0;left:0;right:0;z-index:100;
    background:rgba(18,24,31,0.85);
    backdrop-filter:blur(10px);
    border-bottom:1px solid var(--line);
  }
  nav{display:flex;align-items:center;justify-content:space-between;padding:16px 24px;max-width:1180px;margin:0 auto;}
  .logo{display:flex;align-items:center;gap:10px;font-family:'Oswald',sans-serif;font-size:19px;letter-spacing:0.03em;}
  .logo .mark{
    width:38px;height:38px;border-radius:6px;
    background:linear-gradient(135deg,var(--amber),var(--amber-dark));
    display:flex;align-items:center;justify-content:center;
    color:var(--asphalt);font-size:17px;flex-shrink:0;
  }
  .logo small{display:block;font-family:'Inter',sans-serif;text-transform:none;letter-spacing:0;font-size:10.5px;color:var(--gray);font-weight:500;}
  .nav-links{display:flex;gap:32px;font-size:14px;font-weight:500;color:var(--gray);}
  .nav-links a:hover{color:var(--paper);}
  .nav-call{
    display:flex;align-items:center;gap:8px;
    background:var(--amber);color:var(--asphalt);
    padding:10px 18px;border-radius:5px;font-weight:700;font-size:14px;
    transition:background .2s, transform .2s;
  }
  .nav-call:hover{background:var(--amber-dark);transform:translateY(-1px);}
  .nav-links-mobile{display:none;}
  @media(max-width:820px){.nav-links{display:none;}}

  /* -------- hero -------- */
  .hero{
    position:relative;
    min-height:100vh;
    display:flex;align-items:center;
    padding-top:100px;padding-bottom:80px;
    overflow:hidden;
  }
  .hero-lanes{
    position:absolute;inset:0;z-index:0;
    background:
      repeating-linear-gradient(115deg, transparent 0 78px, var(--line) 78px 80px);
    mask-image:linear-gradient(to bottom, transparent, black 20%, black 75%, transparent);
  }
  .hero-lane-dash{
    position:absolute;inset:0;z-index:0;opacity:.5;
  }
  .hero-lane-dash::before{
    content:'';
    position:absolute;
    top:0;left:-10%;right:-10%;bottom:0;
    background:repeating-linear-gradient(115deg,
      transparent 0 60px,
      rgba(255,138,30,0.14) 60px 66px,
      transparent 66px 220px);
    animation:laneMove 5.5s linear infinite;
  }
  @keyframes laneMove{
    from{transform:translateX(0);}
    to{transform:translateX(220px);}
  }
  .hero-inner{position:relative;z-index:2;width:100%;}
  .eyebrow{
    display:inline-flex;align-items:center;gap:8px;
    font-family:'JetBrains Mono',monospace;font-size:12.5px;
    color:var(--amber);letter-spacing:0.08em;text-transform:uppercase;
    border:1px solid rgba(255,138,30,0.35);
    padding:6px 14px;border-radius:999px;margin-bottom:26px;
  }
  .eyebrow .dot{width:6px;height:6px;border-radius:50%;background:var(--green);animation:pulse 1.8s infinite;}
  @keyframes pulse{0%,100%{opacity:1;}50%{opacity:.3;}}
  .hero h1{
    font-size:clamp(40px,7vw,84px);
    line-height:0.98;
    max-width:920px;
  }
  .hero h1 .accent{color:var(--amber);}
  .hero p.sub{
    margin-top:26px;max-width:560px;
    font-size:18px;line-height:1.6;color:var(--gray);
  }
  .hero-cta{display:flex;gap:16px;margin-top:40px;flex-wrap:wrap;}
  .btn-primary{
    display:inline-flex;align-items:center;gap:10px;
    background:var(--amber);color:var(--asphalt);
    padding:16px 28px;border-radius:6px;font-weight:700;font-size:15.5px;
    box-shadow:0 0 0 0 rgba(255,138,30,0.5);
    transition:transform .2s, box-shadow .3s, background .2s;
  }
  .btn-primary:hover{transform:translateY(-2px);background:var(--amber-dark);}
  .btn-primary i{font-size:14px;}
  .btn-secondary{
    display:inline-flex;align-items:center;gap:10px;
    border:1px solid rgba(245,243,238,0.25);
    padding:16px 28px;border-radius:6px;font-weight:600;font-size:15.5px;
    color:var(--paper);transition:border-color .2s, background .2s;
  }
  .btn-secondary:hover{border-color:var(--paper);background:rgba(245,243,238,0.05);}
  .hero-meta{
    margin-top:64px;display:flex;gap:40px;flex-wrap:wrap;
    padding-top:32px;border-top:1px solid var(--line);
    max-width:760px;
  }
  .hero-meta .item .num{font-family:'Oswald',sans-serif;font-size:28px;color:var(--amber);}
  .hero-meta .item .label{font-size:12.5px;color:var(--gray);margin-top:2px;text-transform:uppercase;letter-spacing:0.06em;}

  /* -------- section shell -------- */
  section{padding:110px 0;position:relative;}
  .section-head{max-width:640px;margin-bottom:56px;}
  .kicker{
    font-family:'JetBrains Mono',monospace;font-size:12.5px;color:var(--amber);
    letter-spacing:0.1em;text-transform:uppercase;margin-bottom:14px;display:block;
  }
  .section-head h2{font-size:clamp(30px,4vw,46px);line-height:1.05;}
  .section-head p{color:var(--gray);margin-top:16px;font-size:16px;line-height:1.6;}

  /* -------- why us -------- */
  .why{background:var(--panel);}
  .why-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:1px;background:var(--line);border:1px solid var(--line);border-radius:14px;overflow:hidden;}
  .why-card{background:var(--panel);padding:34px 30px;transition:background .25s;}
  .why-card:hover{background:var(--panel-2);}
  .why-card i{font-size:22px;color:var(--amber);margin-bottom:18px;display:block;}
  .why-card h3{font-family:'Inter',sans-serif;text-transform:none;letter-spacing:0;font-size:18px;font-weight:700;margin-bottom:10px;}
  .why-card p{color:var(--gray);font-size:14.5px;line-height:1.6;}
  @media(max-width:820px){.why-grid{grid-template-columns:1fr;}}

  /* -------- route map (signature) -------- */
  .route-section{background:var(--asphalt);}
  .route-map{
    position:relative;
    background:var(--panel);
    border:1px solid var(--line);
    border-radius:16px;
    padding:56px 40px 40px;
    overflow:hidden;
  }
  .route-svg-wrap{position:relative;width:100%;max-width:900px;margin:0 auto;}
  .route-path{
    stroke:rgba(245,243,238,0.18);
    stroke-width:2;
    fill:none;
  }
  .route-path-active{
    stroke:var(--amber);
    stroke-width:2.5;
    fill:none;
    stroke-dasharray:1000;
    stroke-dashoffset:1000;
    transition:stroke-dashoffset 2.2s cubic-bezier(.3,.7,.2,1);
  }
  .route-path-active.in{stroke-dashoffset:0;}
  .route-truck{
    font-size:16px;color:var(--paper);
    filter:drop-shadow(0 0 6px rgba(255,138,30,0.7));
  }
  .route-stop{
    display:flex;flex-direction:column;align-items:center;gap:10px;
  }
  .route-stop .pin{
    width:16px;height:16px;border-radius:50%;
    background:var(--asphalt);border:3px solid var(--amber);
  }
  .route-stop .city{font-family:'Oswald',sans-serif;font-size:16px;letter-spacing:0.02em;}
  .route-stop .tag{font-family:'JetBrains Mono',monospace;font-size:11px;color:var(--gray);margin-top:2px;}
  .route-labels{
    display:flex;justify-content:space-between;margin-top:20px;
  }
  .coverage-list{
    margin-top:44px;padding-top:36px;border-top:1px solid var(--line);
  }
  .coverage-list .kicker{margin-bottom:16px;}
  .chip-row{display:flex;flex-wrap:wrap;gap:10px;}
  .chip{
    font-family:'JetBrains Mono',monospace;font-size:13px;
    border:1px solid var(--line);color:var(--gray);
    padding:8px 16px;border-radius:999px;
  }
  .chip.core{border-color:rgba(255,138,30,0.4);color:var(--amber);}

  /* -------- services -------- */
  .services-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:20px;}
  .service-card{
    background:var(--panel);border:1px solid var(--line);border-radius:14px;
    padding:30px 28px;transition:transform .25s, border-color .25s;
  }
  .service-card:hover{transform:translateY(-4px);border-color:rgba(255,138,30,0.35);}
  .service-card .num{font-family:'JetBrains Mono',monospace;color:var(--amber);font-size:12.5px;}
  .service-card h3{font-family:'Inter',sans-serif;text-transform:none;letter-spacing:0;font-size:19px;font-weight:700;margin:14px 0 10px;}
  .service-card p{color:var(--gray);font-size:14.5px;line-height:1.6;}
  @media(max-width:900px){.services-grid{grid-template-columns:1fr 1fr;}}
  @media(max-width:600px){.services-grid{grid-template-columns:1fr;}}

  /* -------- process -------- */
  .process{background:var(--panel);}
  .process-row{display:flex;gap:0;counter-reset:step;}
  .step{flex:1;position:relative;padding:0 24px;}
  .step:not(:last-child)::after{
    content:'';position:absolute;top:22px;right:-10px;width:20px;height:1px;
    background:var(--line);
  }
  .step .step-num{
    font-family:'Oswald',sans-serif;font-size:14px;color:var(--amber);
    width:44px;height:44px;border:1px solid rgba(255,138,30,0.35);border-radius:50%;
    display:flex;align-items:center;justify-content:center;margin-bottom:20px;
  }
  .step h3{font-family:'Inter',sans-serif;text-transform:none;letter-spacing:0;font-size:16.5px;font-weight:700;margin-bottom:8px;}
  .step p{color:var(--gray);font-size:14px;line-height:1.6;}
  @media(max-width:820px){.process-row{flex-direction:column;gap:36px;}.step:not(:last-child)::after{display:none;}}

  /* -------- testimonials -------- */
  .quotes{display:grid;grid-template-columns:repeat(3,1fr);gap:20px;}
  .quote-card{background:var(--panel);border:1px solid var(--line);border-radius:14px;padding:28px;}
  .quote-card i.fa-quote-left{color:rgba(255,138,30,0.4);font-size:18px;margin-bottom:14px;display:block;}
  .quote-card p.text{font-size:14.5px;line-height:1.65;color:var(--paper);margin-bottom:18px;}
  .quote-card .who{font-size:13px;color:var(--gray);font-family:'JetBrains Mono',monospace;}
  @media(max-width:900px){.quotes{grid-template-columns:1fr;}}

  /* -------- contact -------- */
  .contact{background:linear-gradient(180deg,var(--panel) 0%, var(--asphalt) 100%);}
  .contact-grid{display:grid;grid-template-columns:1.1fr 0.9fr;gap:60px;}
  @media(max-width:900px){.contact-grid{grid-template-columns:1fr;}}
  .call-block{
    background:var(--panel);border:1px solid var(--line);border-radius:16px;
    padding:44px 36px;text-align:center;position:relative;overflow:hidden;
  }
  .call-block::before{
    content:'';position:absolute;inset:0;
    background:radial-gradient(circle at 50% 0%, rgba(255,138,30,0.12), transparent 60%);
  }
  .call-icon{
    width:72px;height:72px;border-radius:50%;
    background:rgba(255,138,30,0.12);border:1px solid rgba(255,138,30,0.35);
    display:flex;align-items:center;justify-content:center;margin:0 auto 22px;
    position:relative;z-index:1;
  }
  .call-icon i{font-size:26px;color:var(--amber);}
  .call-icon .ring{
    position:absolute;inset:-8px;border-radius:50%;border:1px solid rgba(255,138,30,0.35);
    animation:ring 2s ease-out infinite;
  }
  @keyframes ring{0%{transform:scale(1);opacity:.8;}100%{transform:scale(1.5);opacity:0;}}
  .call-number{
    font-family:'Oswald',sans-serif;font-size:clamp(26px,4vw,36px);
    color:var(--paper);position:relative;z-index:1;display:inline-block;margin:6px 0 4px;
    letter-spacing:0.02em;
  }
  .call-note{color:var(--gray);font-size:13.5px;position:relative;z-index:1;margin-bottom:26px;}
  .contact-details{display:flex;flex-direction:column;gap:22px;}
  .detail-row{display:flex;gap:16px;align-items:flex-start;}
  .detail-row i{width:38px;height:38px;border-radius:8px;background:var(--panel);border:1px solid var(--line);display:flex;align-items:center;justify-content:center;color:var(--amber);flex-shrink:0;}
  .detail-row .t{font-size:12.5px;text-transform:uppercase;letter-spacing:0.06em;color:var(--gray);margin-bottom:4px;}
  .detail-row .v{font-size:15.5px;font-weight:600;}
  .detail-row .v small{display:block;font-weight:400;color:var(--gray);font-size:13px;margin-top:2px;}

  /* -------- footer -------- */
  footer{
    border-top:1px solid var(--line);padding:36px 0;
    display:flex;justify-content:space-between;align-items:center;flex-wrap:wrap;gap:16px;
  }
  footer .f-logo{display:flex;align-items:center;gap:10px;font-family:'Oswald',sans-serif;font-size:15px;}
  footer .f-note{color:var(--gray);font-size:13px;}
  footer .f-links{display:flex;gap:22px;font-size:13.5px;color:var(--gray);}
  footer .f-links a:hover{color:var(--paper);}

  /* focus visibility */
  a:focus-visible, button:focus-visible{outline:2px solid var(--amber);outline-offset:2px;}

  @media (prefers-reduced-motion: reduce){
    *{animation-duration:0.001ms !important; animation-iteration-count:1 !important; transition-duration:0.001ms !important;}
  }
</style>
</head>
<body>

<header>
  <nav>
    <div class="logo">
      <div class="mark"><i class="fa-solid fa-truck-fast"></i></div>
      <div>
        ANIKET EXPRESS
        <small>CARGO LOGISTICS</small>
      </div>
    </div>
    <div class="nav-links">
      <a href="#why">Why Us</a>
      <a href="#coverage">Coverage</a>
      <a href="#services">Services</a>
      <a href="#contact">Contact</a>
    </div>
    <a class="nav-call" href="tel:+919876543210"><i class="fa-solid fa-phone"></i> Call Now</a>
  </nav>
</header>

<section class="hero">
  <div class="hero-lanes"></div>
  <div class="hero-lane-dash"></div>
  <div class="wrap hero-inner">
    <div class="eyebrow"><span class="dot"></span> DISPATCH OPEN &middot; ROORKEE &ndash; DEHRADUN &ndash; DELHI CORRIDOR</div>
    <h1>Your Cargo Moves <span class="accent">On Schedule.</span><br>Every Route. Every Time.</h1>
    <p class="sub">Aniket Express Cargo Logistics runs dedicated freight lines across Roorkee, Dehradun and Delhi &mdash; built for businesses that can't afford a late delivery.</p>
    <div class="hero-cta">
      <a class="btn-primary" href="tel:+919876543210"><i class="fa-solid fa-phone"></i> Call for Booking</a>
      <a class="btn-secondary" href="#coverage"><i class="fa-solid fa-route"></i> View Coverage Map</a>
    </div>
    <div class="hero-meta">
      <div class="item"><div class="num">3</div><div class="label">Core Routes Covered</div></div>
      <div class="item"><div class="num">24/7</div><div class="label">Dispatch Support</div></div>
      <div class="item"><div class="num">100%</div><div class="label">Insured Cargo Handling</div></div>
    </div>
  </div>
</section>

<section class="why" id="why">
  <div class="wrap">
    <div class="section-head reveal">
      <span class="kicker">Why Ship With Us</span>
      <h2>Reasons businesses choose Aniket Express</h2>
      <p>Freight partners are chosen on one thing &mdash; whether they show up when promised. Here's how we make sure of it.</p>
    </div>
    <div class="why-grid reveal">
      <div class="why-card">
        <i class="fa-solid fa-clock"></i>
        <h3>On-Time, Every Time</h3>
        <p>Fixed departure windows on the Roorkee&ndash;Dehradun&ndash;Delhi line mean your shipment isn't waiting on someone else's schedule.</p>
      </div>
      <div class="why-card">
        <i class="fa-solid fa-shield-halved"></i>
        <h3>Safe & Insured Handling</h3>
        <p>Every consignment is loaded, secured and insured to standard &mdash; so what leaves your dock is what arrives at the other end.</p>
      </div>
      <div class="why-card">
        <i class="fa-solid fa-route"></i>
        <h3>Corridor Specialists</h3>
        <p>We don't spread thin across the map. Roorkee, Dehradun and Delhi is our core lane &mdash; we know every stop on it.</p>
      </div>
      <div class="why-card">
        <i class="fa-solid fa-indian-rupee-sign"></i>
        <h3>Transparent Pricing</h3>
        <p>One quote, no surprise charges at delivery. You know the cost before the truck leaves.</p>
      </div>
      <div class="why-card">
        <i class="fa-solid fa-headset"></i>
        <h3>Direct Dispatch Line</h3>
        <p>No call centres or ticket queues &mdash; speak straight to dispatch and get a real answer on your shipment.</p>
      </div>
      <div class="why-card">
        <i class="fa-solid fa-truck"></i>
        <h3>Fleet Ready for Any Load</h3>
        <p>From single-carton express parcels to full truck loads &mdash; the right vehicle is matched to your consignment.</p>
      </div>
    </div>
  </div>
</section>

<section class="route-section" id="coverage">
  <div class="wrap">
    <div class="section-head reveal">
      <span class="kicker">Service Coverage</span>
      <h2>Running the Roorkee &ndash; Dehradun &ndash; Delhi corridor</h2>
      <p>Our vehicles run this line daily, with pickup and drop across the towns along the way.</p>
    </div>

    <div class="route-map reveal">
      <div class="route-svg-wrap">
        <svg viewBox="0 0 900 160" width="100%" height="auto" style="overflow:visible;">
          <path class="route-path" d="M 60 100 C 250 20, 400 160, 480 90 S 750 20, 840 90" />
          <path id="routeActive" class="route-path-active" d="M 60 100 C 250 20, 400 160, 480 90 S 750 20, 840 90" />
          <circle cx="60" cy="100" r="7" fill="#12181F" stroke="#FF8A1E" stroke-width="3"/>
          <circle cx="480" cy="90" r="7" fill="#12181F" stroke="#FF8A1E" stroke-width="3"/>
          <circle cx="840" cy="90" r="7" fill="#12181F" stroke="#FF8A1E" stroke-width="3"/>
          <text id="routeTruck" x="60" y="100" class="route-truck" font-family="'Font Awesome 6 Free'" font-weight="900">&#xf0d1;</text>
        </svg>
      </div>
      <div class="route-labels">
        <div class="route-stop"><span class="city">Roorkee</span><span class="tag">ORIGIN HUB</span></div>
        <div class="route-stop"><span class="city">Dehradun</span><span class="tag">MID-ROUTE STOP</span></div>
        <div class="route-stop"><span class="city">Delhi</span><span class="tag">TERMINAL HUB</span></div>
      </div>

      <div class="coverage-list">
        <span class="kicker">Also Serving Nearby Areas</span>
        <div class="chip-row">
          <span class="chip core">Roorkee</span>
          <span class="chip core">Dehradun</span>
          <span class="chip core">Delhi</span>
          <span class="chip">Haridwar</span>
          <span class="chip">Rishikesh</span>
          <span class="chip">Saharanpur</span>
          <span class="chip">Muzaffarnagar</span>
          <span class="chip">Meerut</span>
          <span class="chip">Ghaziabad</span>
          <span class="chip">Noida</span>
        </div>
      </div>
    </div>
  </div>
</section>

<section id="services">
  <div class="wrap">
    <div class="section-head reveal">
      <span class="kicker">What We Move</span>
      <h2>Services built around your cargo</h2>
      <p>Whichever way your consignment needs to travel, there's a service line for it.</p>
    </div>
    <div class="services-grid reveal">
      <div class="service-card">
        <span class="num">01</span>
        <h3>Full Truck Load (FTL)</h3>
        <p>Dedicated vehicle, direct route, no shared stops &mdash; for bulk consignments that need a straight run.</p>
      </div>
      <div class="service-card">
        <span class="num">02</span>
        <h3>Part Truck Load (PTL)</h3>
        <p>Pay for the space you use. Ideal for smaller loads moving along the same corridor.</p>
      </div>
      <div class="service-card">
        <span class="num">03</span>
        <h3>Express Parcel Delivery</h3>
        <p>Time-critical documents and small packages, prioritised on the next available run.</p>
      </div>
      <div class="service-card">
        <span class="num">04</span>
        <h3>Industrial & Bulk Cargo</h3>
        <p>Machinery, raw material and heavy consignments handled with the right loading equipment.</p>
      </div>
      <div class="service-card">
        <span class="num">05</span>
        <h3>Office & Household Shifting</h3>
        <p>Packed, moved and unloaded with care &mdash; for relocations across the service corridor.</p>
      </div>
      <div class="service-card">
        <span class="num">06</span>
        <h3>Warehousing & Storage</h3>
        <p>Short-term holding for consignments in transit between pickup and final delivery.</p>
      </div>
    </div>
  </div>
</section>

<section class="process">
  <div class="wrap">
    <div class="section-head reveal">
      <span class="kicker">How It Works</span>
      <h2>From your call to delivery</h2>
    </div>
    <div class="process-row reveal">
      <div class="step">
        <div class="step-num">1</div>
        <h3>You call dispatch</h3>
        <p>Share pickup point, drop point and load details &mdash; get a straight quote on the call.</p>
      </div>
      <div class="step">
        <div class="step-num">2</div>
        <h3>Vehicle assigned</h3>
        <p>A vehicle matched to your load size is scheduled on the next available run.</p>
      </div>
      <div class="step">
        <div class="step-num">3</div>
        <h3>Pickup & transit</h3>
        <p>Cargo is loaded, secured and moved along the Roorkee&ndash;Dehradun&ndash;Delhi line.</p>
      </div>
      <div class="step">
        <div class="step-num">4</div>
        <h3>Delivered & confirmed</h3>
        <p>Drop-off at destination with confirmation back to you.</p>
      </div>
    </div>
  </div>
</section>

<section id="reviews">
  <div class="wrap">
    <div class="section-head reveal">
      <span class="kicker">What Clients Say</span>
      <h2>Businesses that ship with us</h2>
    </div>
    <div class="quotes reveal">
      <div class="quote-card">
        <i class="fa-solid fa-quote-left"></i>
        <p class="text">Our shipments between Roorkee and Delhi now leave and arrive exactly when we're told. That reliability changed how we plan dispatch on our end.</p>
        <div class="who">Wholesale Trader &middot; Roorkee</div>
      </div>
      <div class="quote-card">
        <i class="fa-solid fa-quote-left"></i>
        <p class="text">Pricing was clear from the first call, no last-minute additions at delivery. Straightforward to work with.</p>
        <div class="who">Retail Distributor &middot; Dehradun</div>
      </div>
      <div class="quote-card">
        <i class="fa-solid fa-quote-left"></i>
        <p class="text">We needed a partner who actually knew the Delhi&ndash;Dehradun stretch, not just a generic transporter. This is that partner.</p>
        <div class="who">Manufacturing Unit &middot; Delhi NCR</div>
      </div>
    </div>
  </div>
</section>

<section class="contact" id="contact">
  <div class="wrap">
    <div class="section-head reveal">
      <span class="kicker">Get In Touch</span>
      <h2>Book your shipment today</h2>
      <p>Fastest way to get a quote and a vehicle scheduled is a direct call to dispatch.</p>
    </div>
    <div class="contact-grid reveal">
      <div class="call-block">
        <div class="call-icon"><div class="ring"></div><i class="fa-solid fa-phone"></i></div>
        <div class="call-note">Tap to call dispatch directly</div>
        <a class="call-number" href="tel:+919876543210">+91 98765 43210</a>
        <div class="call-note">Available 24/7 for bookings & queries</div>
        <a class="btn-primary" href="tel:+919876543210" style="margin-top:10px;"><i class="fa-solid fa-phone"></i> Call Now</a>
      </div>
      <div class="contact-details">
        <div class="detail-row">
          <i class="fa-solid fa-location-dot"></i>
          <div>
            <div class="t">Base of Operations</div>
            <div class="v">Roorkee, Uttarakhand<small>Serving the Roorkee &ndash; Dehradun &ndash; Delhi corridor</small></div>
          </div>
        </div>
        <div class="detail-row">
          <i class="fa-solid fa-envelope"></i>
          <div>
            <div class="t">Email</div>
            <div class="v">bookings@aniketexpresscargo.com</div>
          </div>
        </div>
        <div class="detail-row">
          <i class="fa-solid fa-clock"></i>
          <div>
            <div class="t">Dispatch Hours</div>
            <div class="v">24/7 <small>Booking calls answered around the clock</small></div>
          </div>
        </div>
        <div class="detail-row">
          <i class="fa-brands fa-whatsapp"></i>
          <div>
            <div class="t">WhatsApp Booking</div>
            <div class="v"><a href="https://wa.me/919876543210" target="_blank" rel="noopener">+91 98765 43210</a></div>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

<footer>
  <div class="wrap" style="width:100%;display:flex;justify-content:space-between;align-items:center;flex-wrap:wrap;gap:16px;">
    <div class="f-logo"><i class="fa-solid fa-truck-fast" style="color:var(--amber);"></i> ANIKET EXPRESS CARGO LOGISTICS</div>
    <div class="f-links">
      <a href="#why">Why Us</a>
      <a href="#coverage">Coverage</a>
      <a href="#services">Services</a>
      <a href="#contact">Contact</a>
    </div>
    <div class="f-note">&copy; 2026 Aniket Express Cargo Logistics. All rights reserved.</div>
  </div>
</footer>

<script>
  // scroll reveal
  const revealEls = document.querySelectorAll('.reveal');
  const io = new IntersectionObserver((entries)=>{
    entries.forEach(e=>{
      if(e.isIntersecting){ e.target.classList.add('in'); }
    });
  }, {threshold:0.15});
  revealEls.forEach(el=>io.observe(el));

  // route path draw + truck motion
  const routePath = document.getElementById('routeActive');
  const routeTruck = document.getElementById('routeTruck');
  const pathLen = routePath.getTotalLength();
  routePath.style.strokeDasharray = pathLen;
  routePath.style.strokeDashoffset = pathLen;

  let animated = false;
  const routeObserver = new IntersectionObserver((entries)=>{
    entries.forEach(e=>{
      if(e.isIntersecting && !animated){
        animated = true;
        routePath.classList.add('in');
        routePath.style.strokeDashoffset = 0;
        animateTruck();
      }
    });
  }, {threshold:0.3});
  routeObserver.observe(document.querySelector('.route-map'));

  function animateTruck(){
    const duration = 2200;
    const start = performance.now();
    function frame(now){
      let t = Math.min((now-start)/duration, 1);
      const point = routePath.getPointAtLength(t*pathLen);
      routeTruck.setAttribute('x', point.x - 8);
      routeTruck.setAttribute('y', point.y + 5);
      if(t < 1){ requestAnimationFrame(frame); }
      else { loopTruck(); }
    }
    requestAnimationFrame(frame);
  }
  function loopTruck(){
    const duration = 6000;
    function frame(t0){
      const start = performance.now();
      function step(now){
        let t = ((now-start)/duration) % 1;
        const point = routePath.getPointAtLength(t*pathLen);
        routeTruck.setAttribute('x', point.x - 8);
        routeTruck.setAttribute('y', point.y + 5);
        requestAnimationFrame(step);
      }
      requestAnimationFrame(step);
    }
    frame();
  }
</script>

</body>
</html>
