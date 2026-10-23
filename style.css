:root {
  --bg: #fbfbfb;
  --grid: rgba(222, 120, 135, .16);
  --band: #9ca7c7;
  --band-deep: #7f8db3;
  --ink: #1b2027;
  --ink-soft: #3a424c;
  --btn-from: #8d9bb5;
  --btn-to: #12161d;
  --serif-head: "Playfair Display", Georgia, serif;
  --serif-body: "Newsreader", Georgia, serif;
  --sans: "Outfit", system-ui, sans-serif;
  --page: 1100px;
}

*, *::before, *::after { box-sizing: border-box; }
html { scroll-behavior: smooth; scroll-padding-top: 80px; }

body {
  margin: 0;
  color: var(--ink);
  font-family: var(--serif-body);
  font-size: 1.15rem;
  line-height: 1.65;
  background-color: var(--bg);
  background-image:
    linear-gradient(var(--grid) 1px, transparent 1px),
    linear-gradient(90deg, var(--grid) 1px, transparent 1px);
  background-size: 16px 16px;
}

img { max-width: 100%; display: block; }
a { color: inherit; }
:focus-visible { outline: 3px solid var(--ink); outline-offset: 3px; }

h1, h2, h3 { font-family: var(--serif-head); line-height: 1.1; margin: 0 0 1rem; }
h1 { font-size: clamp(2.6rem, 6vw, 4.2rem); font-weight: 700; }
h2 { font-size: clamp(1.8rem, 3.5vw, 2.4rem); font-weight: 700; }
h3 { font-size: 1.3rem; font-weight: 500; text-decoration: underline; text-underline-offset: 4px; }

/* NAV */
.nav {
  position: sticky; top: 0; z-index: 20;
  display: flex; align-items: center; justify-content: space-between;
  padding: .6rem clamp(1rem, 4vw, 3rem);
  background: var(--band);
}
.brand { display: flex; align-items: center; gap: .8rem; text-decoration: none; }
.brand-mark {
  font-family: var(--serif-head); font-size: .95rem; line-height: 1.05; letter-spacing: .04em;
  padding-right: .8rem; border-right: 2px solid var(--ink);
}
.brand-name { font-size: 1.6rem; }

.nav-links { display: flex; gap: clamp(1rem, 3vw, 2.4rem); }
.nav-links a {
  font-family: var(--sans); font-size: .95rem; text-decoration: none; padding: .3rem 0;
  border-bottom: 2px solid transparent; transition: border-color .2s;
}
.nav-links a:hover, .nav-links a.active { border-bottom-color: var(--ink); }
.nav-toggle {
  display: none; font-family: var(--sans); background: none; border: 1px solid var(--ink);
  border-radius: 8px; padding: .35rem .8rem; cursor: pointer; color: var(--ink);
}

/* SHARED LAYOUT */
.section, .hero, .info-wrap, .band .inner {
  max-width: var(--page); margin: 0 auto; padding: 4.5rem clamp(1.2rem, 4vw, 3rem);
}
.band { background: var(--band); }

.btn {
  display: inline-flex; align-items: center; gap: .6rem; cursor: pointer; border: 0;
  font-family: var(--sans); font-size: .95rem; color: #fff; text-decoration: none;
  padding: .9rem 2.2rem; border-radius: 12px;
  background: linear-gradient(90deg, var(--btn-from), var(--btn-to));
  transition: transform .2s, box-shadow .2s;
}
.btn:hover { transform: translateY(-2px); box-shadow: 0 6px 16px rgba(15, 21, 28, .25); }
.btn svg { width: 20px; height: 20px; }

/* HERO */
.hero {
  display: grid; grid-template-columns: 1.1fr .9fr; gap: 2rem; align-items: end;
  min-height: calc(100vh - 70px); padding-bottom: 0;
}
.hero-copy { align-self: center; padding-bottom: 4rem; }
.hero-copy p { max-width: 36ch; color: var(--ink-soft); margin: 0 0 2.2rem; }

.hero-photo { align-self: end; justify-self: center; width: min(100%, 440px); min-height: 380px; }
.hero-photo img { width: 100%; height: auto; filter: grayscale(1) contrast(1.05); }
.hero-photo.no-img, .about-photo.no-img {
  display: grid; place-items: center;
  background: repeating-linear-gradient(45deg, #e3e6ea, #e3e6ea 10px, #eceef1 10px, #eceef1 20px);
}
.hero-photo.no-img::after { content: "Add images/yass.png"; font-family: var(--sans); font-size: .9rem; color: var(--ink-soft); }
.about-photo.no-img::after { content: "Add images/about.jpg"; font-family: var(--sans); font-size: .9rem; color: var(--ink-soft); }
.no-img img { display: none; }

/* MORE INFO */
.info-wrap { display: grid; gap: 2rem; }
.info-panel {
  color: #fff; padding: clamp(1.5rem, 4vw, 3rem); border-radius: 4px;
  background: linear-gradient(135deg, #8d9bb5 0%, #4b5568 45%, #14181f 100%);
}
.info-panel h2, .info-panel h3 { color: #fff; }
.info-panel p { max-width: 52ch; margin: 0 0 1.6rem; font-size: 1.05rem; }
.tools { list-style: disc; columns: 2; max-width: 340px; margin: 0; padding-left: 1.2rem; font-size: 1.05rem; }

.badges { display: flex; flex-wrap: wrap; gap: 1rem; }
.badge {
  display: inline-flex; align-items: center; gap: .6rem; flex: 1 1 200px; justify-content: center;
  font-family: var(--sans); font-size: .85rem; color: #fff;
  padding: .75rem 1.4rem; border-radius: 12px;
  background: linear-gradient(90deg, var(--btn-from), var(--btn-to));
}
.badge svg { width: 18px; height: 18px; fill: #fff; flex: none; }

/* WORK */
.work-band .inner { padding-bottom: 5rem; }
.works { display: grid; grid-template-columns: 1fr 1.25fr 1fr; gap: 1.6rem; align-items: center; margin-top: 2rem; }
.work {
  position: relative; display: block; aspect-ratio: 4 / 5; overflow: hidden;
  text-decoration: none; background: #0d1a1f;
}
.work-main { aspect-ratio: 4 / 5; }
.work img { width: 100%; height: 100%; object-fit: cover; transition: transform .4s; }
.work:hover img { transform: scale(1.04); }
.work-label {
  position: absolute; inset: auto 0 0 0; padding: .8rem 1rem;
  font-family: var(--sans); font-size: .9rem; color: #fff;
  background: linear-gradient(transparent, rgba(0, 0, 0, .7));
  opacity: 0; transition: opacity .25s;
}
.work:hover .work-label, .work:focus-visible .work-label { opacity: 1; }

/* ABOUT */
.about { display: grid; grid-template-columns: 1.3fr 1fr; gap: 3rem; align-items: start; }
.about-text p { max-width: 46ch; margin: 0 0 1.8rem; }
.about-photo { max-width: 520px; aspect-ratio: 16 / 9; overflow: hidden; }
.about-photo img { width: 100%; height: 100%; object-fit: cover; }
.edits h2 { margin: 2.6rem 0 1.2rem; }
.edits ul { list-style: none; margin: 0; padding: 0; display: grid; gap: .8rem; }
.edits li {
  padding: .7rem 1rem; font-size: 1rem; text-align: center;
  background: rgba(156, 167, 199, .22); border: 1px solid #9aa3ab;
}

/* CONTACT */
.contact-band .inner { padding-bottom: 5rem; }
.form { display: grid; max-width: 760px; gap: .4rem; }
.form label { font-family: var(--serif-head); font-weight: 500; font-size: 1.15rem; margin-top: .8rem; }
.form input, .form textarea {
  width: 100%; font: inherit; font-size: 1rem; color: var(--ink);
  padding: .7rem .9rem; background: rgba(255, 255, 255, .55);
  border: 1px solid rgba(27, 32, 39, .45); border-radius: 3px;
}
.form textarea { resize: vertical; }
.form .invalid { border-color: #8f1f1f; background: rgba(255, 255, 255, .8); }
.form-row { display: flex; align-items: center; gap: 1.2rem; margin-top: 1.2rem; flex-wrap: wrap; }
.form-status { margin: 0; font-family: var(--sans); font-size: .9rem; }

/* FOOTER */
.footer {
  display: flex; align-items: center; justify-content: space-between;
  padding: 1.2rem clamp(1rem, 4vw, 3rem); background: var(--bg);
}
.to-top { display: inline-flex; padding: .4rem; }
.to-top svg { width: 40px; height: 24px; }
.socials { display: flex; gap: 1.2rem; list-style: none; margin: 0; padding: 0; }
.socials a {
  display: grid; place-items: center; width: 44px; height: 44px; border-radius: 50%;
  background: var(--ink); transition: transform .2s;
}
.socials a:hover { transform: translateY(-3px); }
.socials svg { width: 22px; height: 22px; fill: #fff; }

/* RESPONSIVE */
@media (max-width: 820px) {
  .nav-toggle { display: block; }
  .nav-links {
    position: absolute; top: 100%; left: 0; right: 0; flex-direction: column; gap: 0;
    background: var(--band-deep); display: none; padding: .5rem 1.2rem 1rem;
  }
  .nav-links.open { display: flex; }
  .nav-links a { padding: .8rem 0; }

  .hero { grid-template-columns: 1fr; min-height: 0; padding-top: 2.5rem; }
  .hero-copy { padding-bottom: 1rem; }
  .hero-photo { min-height: 0; }
  .works { grid-template-columns: 1fr; justify-items: center; }
  .work { width: 100%; max-width: 380px; }
  .about { grid-template-columns: 1fr; gap: 1rem; }
  .edits h2 { margin-top: 1rem; }
}

@media (prefers-reduced-motion: reduce) {
  html { scroll-behavior: auto; }
  * { transition: none !important; }
}