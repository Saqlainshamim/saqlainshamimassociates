<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Saqlain Shamim &amp; Associates | Advocate, Supreme Court of India</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Fraunces:opsz,wght@9..144,300;9..144,500;9..144,600;9..144,700&family=IBM+Plex+Sans:wght@400;500;600&family=IBM+Plex+Mono:wght@400;500&display=swap" rel="stylesheet">
<style>
  :root{
    --ink:#14110F;
    --ink-panel:#1D1915;
    --oxblood:#7A1522;
    --oxblood-bright:#9C1C2C;
    --brass:#B4924F;
    --brass-dim:#8A713C;
    --parchment:#EDE7DA;
    --parchment-dim:#D9D1BE;
    --slate:#C9C2B4;
    --line:rgba(180,146,79,0.25);
  }
  *{margin:0;padding:0;box-sizing:border-box;}
  html{scroll-behavior:smooth;}
  body{
    background:var(--ink);
    color:var(--slate);
    font-family:'IBM Plex Sans',sans-serif;
    line-height:1.6;
    -webkit-font-smoothing:antialiased;
  }
  .serif{font-family:'Fraunces',serif;}
  .mono{font-family:'IBM Plex Mono',monospace;}
  a{color:inherit;text-decoration:none;}
  .wrap{max-width:1100px;margin:0 auto;padding:0 32px;}

  /* Skip link */
  .skip-link{position:absolute;left:-999px;top:0;background:var(--brass);color:var(--ink);padding:10px 16px;z-index:200;}
  .skip-link:focus{left:12px;top:12px;}

  /* Header */
  header{
    position:sticky;top:0;z-index:100;
    background:rgba(20,17,15,0.92);
    backdrop-filter:blur(8px);
    border-bottom:1px solid var(--line);
  }
  .nav-inner{
    display:flex;align-items:center;justify-content:space-between;
    padding:18px 32px;max-width:1100px;margin:0 auto;
  }
  .brand{font-size:1.05rem;letter-spacing:0.02em;}
  .brand .serif{font-weight:600;color:var(--parchment);}
  .brand small{display:block;font-size:0.65rem;color:var(--brass);letter-spacing:0.18em;text-transform:uppercase;margin-top:2px;}
  nav ul{list-style:none;display:flex;gap:32px;}
  nav a{font-size:0.85rem;letter-spacing:0.04em;color:var(--slate);position:relative;padding:4px 0;}
  nav a:hover, nav a:focus-visible{color:var(--brass);}
  nav a::after{content:"";position:absolute;left:0;bottom:0;width:0;height:1px;background:var(--brass);transition:width 0.25s ease;}
  nav a:hover::after, nav a:focus-visible::after{width:100%;}
  .nav-toggle{display:none;background:none;border:1px solid var(--line);color:var(--parchment);padding:8px 12px;font-size:0.8rem;}

  /* Hero */
  .hero{
    position:relative;padding:120px 32px 100px;overflow:hidden;
    border-bottom:1px solid var(--line);
  }
  .hero::before{
    content:"";position:absolute;inset:0;
    background:
      radial-gradient(ellipse 900px 500px at 78% -10%, rgba(122,21,34,0.35), transparent 60%),
      radial-gradient(ellipse 700px 400px at 5% 100%, rgba(180,146,79,0.12), transparent 60%);
    pointer-events:none;
  }
  .hero-inner{max-width:1100px;margin:0 auto;position:relative;}
  .eyebrow{
    font-family:'IBM Plex Mono',monospace;font-size:0.75rem;letter-spacing:0.22em;
    text-transform:uppercase;color:var(--brass);margin-bottom:24px;display:flex;align-items:center;gap:14px;
  }
  .eyebrow::before{content:"";width:32px;height:1px;background:var(--brass-dim);display:inline-block;}
  h1{
    font-size:clamp(2.4rem,5.5vw,4.4rem);font-weight:600;color:var(--parchment);
    line-height:1.08;max-width:16ch;letter-spacing:-0.01em;
    opacity:0;transform:translateY(16px);animation:rise 0.9s ease forwards 0.15s;
  }
  h1 em{font-style:italic;color:var(--oxblood-bright);}
  .hero-sub{
    margin-top:28px;max-width:52ch;font-size:1.05rem;color:var(--slate);
    opacity:0;transform:translateY(16px);animation:rise 0.9s ease forwards 0.4s;
  }
  .hero-cta{
    margin-top:40px;display:flex;gap:16px;flex-wrap:wrap;
    opacity:0;transform:translateY(16px);animation:rise 0.9s ease forwards 0.6s;
  }
  @keyframes rise{to{opacity:1;transform:translateY(0);}}
  @media (prefers-reduced-motion: reduce){
    h1,.hero-sub,.hero-cta{animation:none;opacity:1;transform:none;}
  }
  .btn{
    display:inline-flex;align-items:center;gap:10px;
    padding:14px 26px;font-size:0.9rem;letter-spacing:0.03em;
    border:1px solid var(--brass-dim);transition:all 0.25s ease;
  }
  .btn-primary{background:var(--oxblood);color:var(--parchment);border-color:var(--oxblood);}
  .btn-primary:hover,.btn-primary:focus-visible{background:var(--oxblood-bright);border-color:var(--oxblood-bright);}
  .btn-ghost{color:var(--parchment);}
  .btn-ghost:hover,.btn-ghost:focus-visible{border-color:var(--brass);color:var(--brass);}

  /* Section headings */
  .section{padding:90px 32px;border-bottom:1px solid var(--line);}
  .section-head{margin-bottom:52px;}
  .section-tag{
    font-family:'IBM Plex Mono',monospace;font-size:0.72rem;letter-spacing:0.2em;
    text-transform:uppercase;color:var(--brass);margin-bottom:14px;
  }
  .section-title{font-size:clamp(1.7rem,3vw,2.4rem);color:var(--parchment);font-weight:600;max-width:20ch;}

  /* About */
  .about-grid{display:grid;grid-template-columns:1fr 1.4fr;gap:60px;align-items:start;}
  .about-grid p{font-size:1.02rem;color:var(--slate);margin-bottom:18px;max-width:56ch;}
  .about-name{font-size:1.5rem;color:var(--parchment);font-weight:600;margin-bottom:6px;}
  .about-role{font-size:0.85rem;color:var(--brass);letter-spacing:0.04em;}
  .about-seal{
    width:96px;height:96px;border-radius:50%;border:1px solid var(--brass-dim);
    display:flex;align-items:center;justify-content:center;margin-top:28px;
    position:relative;
  }
  .about-seal::before{content:"";position:absolute;inset:8px;border:1px solid var(--line);border-radius:50%;}
  .about-seal svg{width:40px;height:40px;stroke:var(--brass);}

  /* Cause list / practice areas */
  .causelist{width:100%;border-collapse:collapse;}
  .causelist thead th{
    text-align:left;font-family:'IBM Plex Mono',monospace;font-size:0.72rem;
    letter-spacing:0.14em;text-transform:uppercase;color:var(--brass);
    padding:0 20px 16px;border-bottom:1px solid var(--brass-dim);
  }
  .causelist tbody tr{
    border-bottom:1px solid var(--line);
    opacity:0;transform:translateX(-10px);
    animation:slidein 0.6s ease forwards;
  }
  @media (prefers-reduced-motion: reduce){ .causelist tbody tr{animation:none;opacity:1;transform:none;} }
  .causelist tbody tr:nth-child(1){animation-delay:0.05s;}
  .causelist tbody tr:nth-child(2){animation-delay:0.15s;}
  .causelist tbody tr:nth-child(3){animation-delay:0.25s;}
  .causelist tbody tr:nth-child(4){animation-delay:0.35s;}
  .causelist tbody tr:nth-child(5){animation-delay:0.45s;}
  @keyframes slidein{to{opacity:1;transform:translateX(0);}}
  .causelist td{padding:22px 20px;vertical-align:top;}
  .causelist tbody tr:hover{background:rgba(180,146,79,0.05);}
  .cl-no{font-family:'IBM Plex Mono',monospace;color:var(--brass-dim);font-size:0.85rem;width:60px;}
  .cl-title{color:var(--parchment);font-weight:600;font-size:1.02rem;width:220px;}
  .cl-desc{color:var(--slate);font-size:0.92rem;max-width:52ch;}

  /* Membership */
  .member-list{display:grid;grid-template-columns:repeat(2,1fr);gap:1px;background:var(--line);border:1px solid var(--line);}
  .member-item{
    background:var(--ink);padding:28px 30px;display:flex;gap:18px;align-items:flex-start;
  }
  .member-mark{
    font-family:'IBM Plex Mono',monospace;color:var(--brass);font-size:0.75rem;
    border:1px solid var(--brass-dim);border-radius:50%;width:28px;height:28px;
    display:flex;align-items:center;justify-content:center;flex-shrink:0;margin-top:2px;
  }
  .member-item h3{color:var(--parchment);font-size:1rem;font-weight:600;margin-bottom:4px;}
  .member-item p{font-size:0.85rem;color:var(--slate);}

  /* Contact */
  .contact{background:var(--ink-panel);}
  .contact-grid{display:grid;grid-template-columns:1.2fr 1fr;gap:60px;align-items:center;}
  .contact-title{font-size:clamp(1.8rem,3.4vw,2.6rem);color:var(--parchment);font-weight:600;line-height:1.15;margin-bottom:20px;max-width:16ch;}
  .contact-lede{color:var(--slate);max-width:48ch;margin-bottom:8px;}
  .contact-card{border:1px solid var(--brass-dim);padding:36px;}
  .contact-row{display:flex;flex-direction:column;gap:4px;padding:18px 0;border-bottom:1px solid var(--line);}
  .contact-row:last-child{border-bottom:none;}
  .contact-label{font-family:'IBM Plex Mono',monospace;font-size:0.7rem;letter-spacing:0.16em;text-transform:uppercase;color:var(--brass);}
  .contact-value{font-size:1.1rem;color:var(--parchment);}
  .contact-value a:hover{color:var(--brass);}

  footer{padding:44px 32px;text-align:center;}
  footer .serif{color:var(--parchment);font-size:1.05rem;font-weight:600;}
  footer .tagline{font-size:0.8rem;color:var(--brass-dim);letter-spacing:0.06em;margin-top:8px;font-style:italic;}
  footer .copy{font-size:0.75rem;color:#6b6558;margin-top:20px;}

  @media (max-width:820px){
    nav ul{display:none;}
    .nav-toggle{display:block;}
    .about-grid,.contact-grid{grid-template-columns:1fr;}
    .member-list{grid-template-columns:1fr;}
    .causelist thead{display:none;}
    .causelist td{display:block;padding:4px 20px;}
    .causelist tr{padding:20px 0;}
    .cl-title{width:auto;}
  }
</style>
</head>
<body>
<a href="#main" class="skip-link">Skip to content</a>

<header>
  <div class="nav-inner">
    <div class="brand">
      <span class="serif">Saqlain Shamim &amp; Associates</span>
      <small>Advocates &middot; Supreme Court of India</small>
    </div>
    <nav aria-label="Primary">
      <ul>
        <li><a href="#practice">Practice</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#membership">Membership</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </div>
</header>

<main id="main">
  <section class="hero">
    <div class="hero-inner">
      <p class="eyebrow">Criminal Litigation &middot; Supreme Court Practice</p>
      <h1 class="serif">Defending Rights.<br>Securing <em>Liberty</em>.<br>Delivering Justice.</h1>
      <p class="hero-sub">Adv. Saqlain Shamim represents clients in criminal matters before the Supreme Court of India, with focused practice in NDPS, ED, and Excise Act litigation, bail applications, and transfer petitions.</p>
      <div class="hero-cta">
        <a class="btn btn-primary" href="tel:+917610272750">Call +91 76102 72750</a>
        <a class="btn btn-ghost" href="mailto:advsaqlainshamim@gmail.com">Email the Chambers</a>
      </div>
    </div>
  </section>

  <section class="section" id="about">
    <div class="wrap">
      <div class="about-grid">
        <div>
          <p class="about-name serif">Adv. Saqlain Shamim</p>
          <p class="about-role">Advocate &middot; Supreme Court of India</p>
          <div class="about-seal" aria-hidden="true">
            <svg viewBox="0 0 24 24" fill="none" stroke-width="1.2">
              <path d="M12 2v20M4 8h16M6 8l-3 6a4 4 0 0 0 8 0l-3-6M18 8l-3 6a4 4 0 0 0 8 0l-3-6" stroke-linecap="round" stroke-linejoin="round"/>
            </svg>
          </div>
        </div>
        <div>
          <p class="section-tag">About the Chambers</p>
          <p>Saqlain Shamim &amp; Associates is a New Delhi based criminal litigation practice appearing before the Supreme Court of India. The chambers acts for clients in narcotics, money-laundering, and excise proceedings, alongside bail matters and transfer petitions.</p>
          <p>The practice is built around direct, rigorous representation at the apex court &mdash; where liberty is often decided on the strength of the first hearing.</p>
        </div>
      </div>
    </div>
  </section>

  <section class="section" id="practice">
    <div class="wrap">
      <div class="section-head">
        <p class="section-tag">Register of Practice</p>
        <h2 class="section-title serif">Core areas heard before the Court</h2>
      </div>
      <table class="causelist">
        <thead>
          <tr><th>S. No.</th><th>Matter</th><th>Scope</th></tr>
        </thead>
        <tbody>
          <tr>
            <td class="cl-no mono">01</td>
            <td class="cl-title">NDPS Matters</td>
            <td class="cl-desc">Defense in cases under the Narcotic Drugs and Psychotropic Substances Act, from bail through appeal.</td>
          </tr>
          <tr>
            <td class="cl-no mono">02</td>
            <td class="cl-title">ED Matters</td>
            <td class="cl-desc">Representation in Enforcement Directorate proceedings, including PMLA summons and prosecution.</td>
          </tr>
          <tr>
            <td class="cl-no mono">03</td>
            <td class="cl-title">Excise Act Cases</td>
            <td class="cl-desc">Litigation arising under state and central Excise Act provisions.</td>
          </tr>
          <tr>
            <td class="cl-no mono">04</td>
            <td class="cl-title">Bail Matters</td>
            <td class="cl-desc">Regular, anticipatory, and interim bail applications across forums.</td>
          </tr>
          <tr>
            <td class="cl-no mono">05</td>
            <td class="cl-title">Transfer Petitions</td>
            <td class="cl-desc">Transfer petitions filed and argued before the Supreme Court of India.</td>
          </tr>
        </tbody>
      </table>
    </div>
  </section>

  <section class="section" id="membership">
    <div class="wrap">
      <div class="section-head">
        <p class="section-tag">Enrollment &amp; Membership</p>
        <h2 class="section-title serif">Recognised by the Bar</h2>
      </div>
      <div class="member-list">
        <div class="member-item">
          <span class="member-mark mono">01</span>
          <div><h3>Supreme Court Bar Association</h3><p>SCBA, New Delhi</p></div>
        </div>
        <div class="member-item">
          <span class="member-mark mono">02</span>
          <div><h3>Delhi High Court Bar Association</h3><p>DHCBA, New Delhi</p></div>
        </div>
        <div class="member-item">
          <span class="member-mark mono">03</span>
          <div><h3>International Council of Jurists</h3><p>London</p></div>
        </div>
        <div class="member-item">
          <span class="member-mark mono">04</span>
          <div><h3>Legal Aid Council</h3><p>Government of India</p></div>
        </div>
      </div>
    </div>
  </section>

  <section class="section contact" id="contact" style="border-bottom:none;">
    <div class="wrap">
      <div class="contact-grid">
        <div>
          <p class="section-tag">Consult the Chambers</p>
          <h2 class="contact-title serif">Every hearing begins with a conversation.</h2>
          <p class="contact-lede">Reach out directly by phone or email to discuss your matter with Adv. Saqlain Shamim.</p>
        </div>
        <div class="contact-card">
          <div class="contact-row">
            <span class="contact-label">Phone</span>
            <span class="contact-value"><a href="tel:+917610272750">+91 76102 72750</a></span>
          </div>
          <div class="contact-row">
            <span class="contact-label">Email</span>
            <span class="contact-value"><a href="mailto:advsaqlainshamim@gmail.com">advsaqlainshamim@gmail.com</a></span>
          </div>
          <div class="contact-row">
            <span class="contact-label">Office</span>
            <span class="contact-value">New Delhi, India</span>
          </div>
        </div>
      </div>
    </div>
  </section>
</main>

<footer>
  <p class="serif">Saqlain Shamim &amp; Associates</p>
  <p class="tagline">Defending Rights. Securing Liberty. Delivering Justice.</p>
  <p class="copy">&copy; <span id="year"></span> Saqlain Shamim &amp; Associates, Advocates. All rights reserved.</p>
</footer>

<script>
  document.getElementById('year').textContent = new Date().getFullYear();
</script>
</body>
</html>

