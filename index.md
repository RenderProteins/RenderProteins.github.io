---
layout: default
author_profile: false
---

<style>
/* Reset page padding that minimal-mistakes adds */
.page__content { padding: 0 !important; background: transparent !important; }
#main { background: #07080c; padding: 0 !important; float: none !important; width: 100% !important; }
.page { background: #07080c; }
.initial-content { background: #07080c; }

/* Atmospheric background */
.atm { position: fixed; inset: 0; z-index: 0; pointer-events: none; }
.atm::before {
  content: '';
  position: absolute; inset: 0;
  background:
    radial-gradient(ellipse 70% 50% at 12% 5%, rgba(99,102,241,.07) 0%, transparent 60%),
    radial-gradient(ellipse 50% 40% at 88% 12%, rgba(139,92,246,.05) 0%, transparent 50%),
    radial-gradient(ellipse 60% 50% at 65% 92%, rgba(99,102,241,.03) 0%, transparent 50%);
}

/* Hero */
.rn-hero {
  position: relative; z-index: 1;
  min-height: 92vh;
  display: flex; flex-direction: column; justify-content: center;
  padding: 8rem 3rem 4rem;
  max-width: 1280px; margin: 0 auto;
}
.rn-eyebrow {
  font-family: 'IBM Plex Mono', monospace;
  font-size: .76rem; letter-spacing: .18em; text-transform: uppercase;
  color: #a5b4fc; margin-bottom: 2rem;
  display: flex; align-items: center; gap: .8rem;
  animation: rn-fu .7s .15s both;
}
.rn-eyebrow::before {
  content: ''; width: 2.5rem; height: 1px;
  background: linear-gradient(90deg, #6366f1, transparent);
}
.rn-hero h1 {
  font-family: 'Fraunces', serif !important;
  font-size: clamp(2.8rem, 6vw, 5rem) !important;
  line-height: 1.08 !important;
  font-weight: 300 !important;
  max-width: 820px;
  letter-spacing: -.02em !important;
  color: #eef0f6 !important;
  border: none !important;
  animation: rn-fu .7s .3s both;
}
.rn-hero h1 em {
  font-style: italic; font-weight: 400;
  background: linear-gradient(135deg, #a5b4fc, #8b5cf6);
  -webkit-background-clip: text; -webkit-text-fill-color: transparent;
  background-clip: text;
}
.rn-sub {
  font-family: 'Manrope', sans-serif;
  font-size: 1.12rem; color: #9399b2;
  max-width: 600px; margin-top: 2rem;
  font-weight: 300; line-height: 1.85;
  animation: rn-fu .7s .5s both;
}
.rn-actions {
  margin-top: 3rem; display: flex; gap: 1.2rem; flex-wrap: wrap;
  animation: rn-fu .7s .65s both;
}
.rn-btn-p {
  display: inline-flex; align-items: center; gap: .5rem;
  padding: .85rem 2rem; border-radius: 6px;
  font-family: 'Manrope', sans-serif;
  font-size: .86rem; font-weight: 600;
  text-decoration: none; letter-spacing: .02em;
  background: #6366f1; color: #fff !important;
  box-shadow: 0 2px 20px rgba(99,102,241,.2);
  transition: all .3s; border: none;
}
.rn-btn-p:hover { background: #5558e8 !important; transform: translateY(-2px); box-shadow: 0 8px 35px rgba(99,102,241,.35); }
.rn-btn-g {
  display: inline-flex; align-items: center;
  padding: .85rem 2rem; border-radius: 6px;
  font-family: 'Manrope', sans-serif;
  font-size: .86rem; font-weight: 600;
  text-decoration: none; letter-spacing: .02em;
  background: transparent; color: #9399b2 !important;
  border: 1px solid rgba(147,153,178,.08);
  transition: all .3s;
}
.rn-btn-g:hover { border-color: rgba(99,102,241,.25) !important; color: #a5b4fc !important; }

/* Mission banner */
.rn-mission {
  position: relative; z-index: 1;
  max-width: 1280px; margin: 0 auto; padding: 0 3rem 6rem;
}
.rn-mission-inner {
  background: linear-gradient(135deg, rgba(99,102,241,.08), rgba(139,92,246,.04));
  border: 1px solid rgba(99,102,241,.14);
  border-radius: 12px; padding: 3rem 3.5rem; text-align: center;
}
.rn-mission-inner p {
  font-family: 'Fraunces', serif !important;
  font-size: clamp(1.2rem, 2.5vw, 1.55rem) !important;
  line-height: 1.5 !important; font-weight: 300 !important;
  color: #9399b2 !important;
  max-width: 750px; margin: 0 auto;
}
.rn-mission-inner strong { color: #a5b4fc !important; font-weight: 600 !important; }
.rn-mission-inner em { color: #34d399 !important; font-style: normal !important; font-weight: 600 !important; }

@keyframes rn-fu { from { opacity: 0; transform: translateY(28px); } to { opacity: 1; transform: translateY(0); } }

@media (max-width: 768px) {
  .rn-hero { padding: 7rem 1.5rem 3rem; }
  .rn-mission { padding: 0 1.5rem 4rem; }
  .rn-mission-inner { padding: 2rem 1.5rem; }
}
</style>

<div class="atm"></div>

<div class="rn-hero">
  <div class="rn-eyebrow">From Static to Dynamic</div>
  <h1>Biology occurs in motion.<br>It's time we <em>render</em> it.</h1>
  <p class="rn-sub">Render is building the methods, tools, and infrastructure to make protein motion visible, measurable, and usable — transforming how we discover drugs, design biology, and understand disease.</p>
  <div class="rn-actions">
    <a href="/about/" class="rn-btn-p">Explore the Initiative →</a>
    <a href="/research/" class="rn-btn-g">Why This Matters</a>
  </div>
</div>

<div class="rn-mission">
  <div class="rn-mission-inner">
    <p></p>
  </div>
</div>
