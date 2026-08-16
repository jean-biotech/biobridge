---
layout: splash
title: " "
classes: wide
---

<style>
/* ================================================================
   Homepage — editorial layout built on the global tokens in
   assets/css/main.scss (--paper, --ink, --pine, --terracotta,
   --ochre, --spark, --sage, --font-display/body/mono).
   ================================================================ */

.hp { max-width: 1360px; margin: 0 auto; padding: 0 1.25rem; }
.hp-band { padding: 3.5rem 0; }
.hp-band + .hp-band { border-top: 1px solid var(--border-soft); }
.hp-band--tint { background: var(--paper-warm); }
.hp-band--dark {
  background: var(--pine-dark);
  color: rgba(247,241,230,0.92);
}
.hp-band--dark .eyebrow { color: var(--spark); }
.hp-band--dark h2 { color: var(--paper); }

/* ---------------- Hero ---------------- */
.hero {
  display: grid;
  grid-template-columns: 1fr;
  gap: 2.5rem;
  align-items: center;
  padding-top: 2.5rem;
  padding-bottom: 1rem;
}
.hero-copy { max-width: 640px; }
.hero-copy h1 {
  font-size: clamp(2.1rem, 5.4vw, 3.4rem);
  font-weight: 600;
  line-height: 1.08;
  letter-spacing: -0.015em;
  margin: 0.9rem 0 1.25rem;
  color: var(--ink);
}
.hero-copy h1 em {
  font-style: italic;
  color: var(--terracotta);
}
.hero-copy h1 .accent-pine { color: var(--pine); font-style: italic; }
.hero-copy .hero-sub {
  font-size: 1.15rem;
  color: var(--ink-soft);
  line-height: 1.65;
  margin: 0 0 1.75rem;
  max-width: 520px;
}
.hero-actions { display: flex; flex-wrap: wrap; align-items: center; gap: 1.5rem; margin-bottom: 1.5rem; }
.btn-start {
  display: inline-flex;
  align-items: center;
  gap: 0.5rem;
  background: var(--terracotta);
  color: var(--paper) !important;
  font-family: var(--font-body);
  font-weight: 600;
  font-size: 1rem;
  padding: 0.9rem 1.75rem;
  border-radius: 100px;
  text-decoration: none !important;
  box-shadow: var(--shadow-sm);
  transition: transform 0.2s ease, box-shadow 0.2s ease, background 0.2s ease;
}
.btn-start:hover { background: var(--pine); transform: translateY(-2px); box-shadow: var(--shadow-md); color: var(--paper) !important; }
.hero-quiet-links { display: flex; flex-direction: column; gap: 0.4rem; }
.hero-quiet-links a {
  font-family: var(--font-body);
  font-size: 0.92rem;
  font-weight: 500;
  color: var(--ink-soft) !important;
  text-decoration: none !important;
  border-bottom: 1px solid var(--border);
  width: fit-content;
  padding-bottom: 1px;
  transition: color 0.2s ease, border-color 0.2s ease;
}
.hero-quiet-links a:hover { color: var(--pine) !important; border-color: var(--pine); }
.hero-honest-line {
  font-family: var(--font-mono);
  font-size: 0.82rem;
  color: var(--ink-soft);
  border-left: 2px solid var(--sage);
  padding-left: 0.75rem;
  max-width: 420px;
}
.hero-visual { display: flex; justify-content: center; transform: rotate(-1.2deg); }
.hero-visual svg { width: 100%; max-width: 480px; height: auto; }

@media (min-width: 900px) {
  .hero { grid-template-columns: 1.1fr 0.9fr; padding-top: 4.5rem; padding-bottom: 2.5rem; }
  .hero-visual { transform: rotate(-2deg) translateY(-10px); }
}

/* ---------------- Journey ---------------- */
.journey-head { max-width: 560px; margin-bottom: 2.75rem; }
.journey-wrap { display: grid; grid-template-columns: 1fr; gap: 0; position: relative; }
.journey-spine { display: none; }
.journey-stop {
  display: grid;
  grid-template-columns: auto 1fr;
  gap: 1.25rem;
  padding: 1.75rem 0;
  border-bottom: 1px dashed var(--border);
}
.journey-stop:last-child { border-bottom: none; }
.journey-num {
  font-family: var(--font-mono);
  font-size: 0.95rem;
  color: var(--paper);
  background: var(--pine);
  width: 2.5rem;
  height: 2.5rem;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-shrink: 0;
}
.journey-stop:nth-child(2) .journey-num { background: var(--terracotta); }
.journey-stop:nth-child(3) .journey-num { background: var(--ochre); color: var(--ink); }
.journey-body h3 { margin: 0 0 0.5rem; font-size: 1.3rem; }
.journey-body p { color: var(--ink-soft); margin: 0 0 0.75rem; max-width: 560px; }
.journey-body a { font-family: var(--font-body); font-weight: 600; text-decoration: none !important; }

@media (min-width: 900px) {
  .journey-wrap { grid-template-columns: 70px 1fr; gap: 1.5rem; }
  .journey-spine { display: block; grid-row: 1 / -1; }
  .journey-spine svg { width: 100%; height: 100%; }
  .journey-stop:nth-child(2) { margin-left: 4%; }
  .journey-stop:nth-child(3) { margin-left: 1%; }
}

/* ---------------- Founder story ---------------- */
.story-grid {
  display: grid;
  grid-template-columns: 1fr;
  gap: 2.25rem;
}
.story-photo-col { display: flex; justify-content: center; }
.story-photo-frame {
  position: relative;
  transform: rotate(-2deg);
}
.story-photo {
  width: 220px;
  height: 220px;
  border-radius: var(--radius-lg);
  object-fit: cover;
  box-shadow: var(--shadow-lg);
  border: 6px solid var(--paper);
  display: block;
}
.story-caption {
  font-family: var(--font-mono);
  font-size: 0.75rem;
  color: var(--ink-soft);
  text-align: center;
  margin-top: 0.85rem;
  transform: rotate(1.5deg);
}
.story-caption strong { color: var(--pine-dark); display: block; font-family: var(--font-body); font-size: 0.95rem; margin-bottom: 0.15rem; }
.story-content p.lede { font-size: 1.08rem; line-height: 1.8; color: var(--ink); }
.story-content p { color: var(--ink-soft); line-height: 1.8; margin-bottom: 1rem; }
.story-connect { display: flex; align-items: center; gap: 1rem; flex-wrap: wrap; margin-top: 1.5rem; }
.story-connect-label { font-family: var(--font-mono); font-size: 0.72rem; text-transform: uppercase; letter-spacing: 0.08em; color: var(--ink-soft); }
.story-connect a {
  display: inline-flex; align-items: center; gap: 0.4rem;
  font-family: var(--font-body); font-weight: 600; font-size: 0.9rem;
  text-decoration: none !important;
  padding: 0.45rem 0.9rem;
  border-radius: 100px;
  border: 1px solid var(--border);
  color: var(--ink) !important;
  background: var(--paper);
  transition: all 0.2s ease;
}
.story-connect a:hover { border-color: var(--terracotta); color: var(--terracotta) !important; }

@media (min-width: 900px) {
  .story-grid { grid-template-columns: 260px 1fr; gap: 3.5rem; align-items: start; }
}

/* ---------------- Career Explorer ---------------- */
.explorer-head { max-width: 640px; margin-bottom: 2rem; }
.explorer-filters {
  background: var(--paper-warm);
  border: 1px solid var(--border);
  border-radius: var(--radius-md);
  padding: 1.5rem;
  margin-bottom: 2rem;
}
.filter-group { margin-bottom: 1.1rem; }
.filter-group:last-child { margin-bottom: 0; }
.filter-group-label {
  display: block;
  font-family: var(--font-mono);
  font-size: 0.72rem;
  text-transform: uppercase;
  letter-spacing: 0.08em;
  color: var(--ink-soft);
  margin-bottom: 0.6rem;
}
.explorer-chips { display: flex; flex-wrap: wrap; gap: 0.5rem; }
.chip {
  font-family: var(--font-body);
  font-size: 0.85rem;
  font-weight: 500;
  padding: 0.45rem 0.95rem;
  border-radius: 100px;
  border: 1.5px solid var(--border);
  background: var(--paper);
  color: var(--ink-soft);
  cursor: pointer;
  transition: all 0.15s ease;
}
.chip:hover { border-color: var(--pine); }
.chip[aria-pressed="true"] {
  background: var(--pine);
  border-color: var(--pine);
  color: var(--paper);
}
.explorer-toolbar { display: flex; align-items: center; justify-content: space-between; gap: 1rem; margin-top: 1.25rem; padding-top: 1.1rem; border-top: 1px solid var(--border); }
.explorer-count { font-family: var(--font-mono); font-size: 0.8rem; color: var(--ink-soft); }
.explorer-reset {
  font-family: var(--font-body);
  font-size: 0.85rem;
  font-weight: 600;
  color: var(--terracotta);
  background: none;
  border: none;
  cursor: pointer;
  padding: 0.25rem 0;
}
.explorer-reset:hover { color: var(--pine); }
.explorer-results {
  display: grid;
  grid-template-columns: 1fr;
  gap: 1.1rem;
}
.explorer-empty { color: var(--ink-soft); font-style: italic; padding: 2rem 0; }
.role-card {
  background: var(--paper);
  border: 1px solid var(--border);
  border-left: 4px solid var(--terracotta);
  border-radius: var(--radius-sm);
  padding: 1.25rem 1.4rem;
  transition: box-shadow 0.2s ease, transform 0.2s ease;
}
.role-card:nth-child(3n+2) { border-left-color: var(--pine); }
.role-card:nth-child(3n) { border-left-color: var(--ochre); }
.role-card:hover { box-shadow: var(--shadow-md); transform: translateY(-2px); }
.role-card__top { display: flex; align-items: flex-start; justify-content: space-between; gap: 0.75rem; margin-bottom: 0.65rem; }
.role-card__title { margin: 0; font-size: 1.05rem; }
.badge {
  font-family: var(--font-mono);
  font-size: 0.66rem;
  text-transform: uppercase;
  letter-spacing: 0.05em;
  padding: 0.3rem 0.55rem;
  border-radius: 5px;
  white-space: nowrap;
  flex-shrink: 0;
}
.badge--go { background: var(--pine-tint); color: var(--pine-dark); }
.badge--maybe { background: var(--ochre-tint); color: #7A5A16; }
.badge--later { background: var(--terracotta-tint); color: #8A421F; }
.role-card__salary { font-size: 0.85rem; color: var(--ink); margin: 0 0 0.65rem; line-height: 1.5; }
.role-card__salary .eyebrow { color: var(--ink-soft); font-size: 0.66rem; }
.role-card__step { font-size: 0.9rem; color: var(--ink-soft); line-height: 1.6; margin: 0 0 0.85rem; }
.role-card__link { font-family: var(--font-body); font-weight: 600; font-size: 0.85rem; text-decoration: none !important; }

@media (min-width: 700px) {
  .explorer-results { grid-template-columns: repeat(2, 1fr); }
}
@media (min-width: 1100px) {
  .explorer-results { grid-template-columns: repeat(3, 1fr); }
}

/* ---------------- Learning Lab teaser ---------------- */
.lab-grid { display: grid; grid-template-columns: 1fr; gap: 1.25rem; }
.lab-card {
  border-radius: var(--radius-md);
  padding: 1.5rem;
  border: 1px solid var(--border);
}
.lab-card h3 { font-size: 1.05rem; margin: 0 0 0.3rem; }
.lab-card .eyebrow { display: block; margin-bottom: 0.5rem; }
.lab-card p.lab-desc { color: var(--ink-soft); font-size: 0.88rem; margin: 0 0 1rem; }
.lab-logos { display: flex; flex-wrap: wrap; align-items: center; gap: 1rem 1.25rem; }
.lab-logos img { height: 26px; width: auto; max-width: 100px; object-fit: contain; filter: grayscale(15%); opacity: 0.9; }
.lab-card--newsletters { background: var(--pine-tint); }
.lab-card--podcasts { background: var(--pine-dark); border-color: var(--pine-dark); }
.lab-card--podcasts h3, .lab-card--podcasts .lab-desc { color: rgba(247,241,230,0.85); }
.lab-card--podcasts .eyebrow { color: var(--spark); }
.lab-card--courses { background: var(--ochre-tint); }
.lab-card--books { background: var(--terracotta-tint); }
.lab-books-row { display: flex; gap: 0.6rem; }
.lab-books-row img { width: 52px; height: 76px; object-fit: cover; border-radius: 3px; box-shadow: var(--shadow-sm); }
.lab-books-row img:nth-child(2) { transform: translateY(6px) rotate(-2deg); }
.lab-books-row img:nth-child(3) { transform: translateY(-4px) rotate(2deg); }
.lab-more { margin-top: 2rem; }
.lab-more a { font-weight: 600; text-decoration: none !important; }

@media (min-width: 900px) {
  .lab-grid { grid-template-columns: repeat(4, 1fr); }
  .lab-card--newsletters, .lab-card--podcasts { margin-top: 0; }
  .lab-card--courses { margin-top: 1.5rem; }
  .lab-card--books { margin-top: -1rem; }
}

/* ---------------- Myth-buster ---------------- */
.myth-list { display: flex; flex-direction: column; gap: 0; margin-top: 2rem; }
.myth-item { display: grid; grid-template-columns: 1fr; gap: 0.4rem; padding: 1.5rem 0; border-top: 1px solid rgba(247,241,230,0.18); }
.myth-item:first-child { border-top: none; }
.myth-num { font-family: var(--font-mono); font-size: 0.75rem; color: var(--spark); }
.myth-claim { font-family: var(--font-display); font-size: 1.25rem; font-style: italic; color: var(--paper); margin: 0.15rem 0 0.4rem; }
.myth-reality { color: rgba(247,241,230,0.78); font-size: 0.95rem; line-height: 1.7; max-width: 720px; }
.myth-reality strong { color: var(--spark); font-weight: 600; }

@media (min-width: 900px) {
  .myth-item { grid-template-columns: 260px 1fr; align-items: baseline; }
}

/* ---------------- Jargon decoder ---------------- */
.jargon-grid { display: grid; grid-template-columns: 1fr; gap: 1.25rem 2.5rem; margin-top: 2rem; }
.jargon-term { border-bottom: 1px solid var(--border); padding-bottom: 1rem; }
.jargon-term dt { font-family: var(--font-mono); font-size: 0.9rem; font-weight: 600; color: var(--pine-dark); margin-bottom: 0.3rem; }
.jargon-term dd { margin: 0; color: var(--ink-soft); font-size: 0.9rem; line-height: 1.6; }

@media (min-width: 800px) {
  .jargon-grid { grid-template-columns: repeat(2, 1fr); }
}

/* ---------------- Close / get involved ---------------- */
.close-band { text-align: left; }
.close-inner { max-width: 720px; }
.close-inner h2 { font-size: clamp(1.6rem, 3.4vw, 2.3rem); margin: 0.75rem 0 1rem; }
.close-inner p { color: var(--ink-soft); font-size: 1.05rem; line-height: 1.7; margin: 0 0 1.5rem; max-width: 560px; }

/* shared eyebrow spacing on this page */
.hp .eyebrow { margin-bottom: 0.6rem; display: inline-block; }
.hp h2 { font-size: clamp(1.5rem, 3vw, 2rem); margin: 0; }
</style>

<!-- ============ 1. HERO ============ -->
<div class="hp">
  <div class="hero">
    <div class="hero-copy">
      <span class="eyebrow">Student-led biotech access initiative</span>
      <h1>Bridging the gap between <em>curiosity</em> and <span class="accent-pine">careers</span> in biotechnology.</h1>
      <p class="hero-sub">Clear explanations, curated resources, and honest guidance — for anyone who's curious about biotech but doesn't know where to start.</p>
      <div class="hero-actions">
        <a href="/what-is-biotech/" class="btn-start">Start Here &rarr;</a>
        <div class="hero-quiet-links">
          <a href="/career-pathways/">Explore career pathways</a>
          <a href="/resources/">Browse the Learning Lab</a>
        </div>
      </div>
      <p class="hero-honest-line">Started as one student's overflowing DMs — now it's a resource for anyone asking the same questions.</p>
    </div>
    <div class="hero-visual">
      {% include bridge-line.html variant="hero" %}
    </div>
  </div>
</div>

<!-- ============ 2. THE JOURNEY ============ -->
<div class="hp-band hp-band--tint">
  <div class="hp">
    <div class="journey-head">
      <span class="eyebrow">How BioBridge works</span>
      <h2>Three stops on the way in.</h2>
    </div>
    <div class="journey-wrap">
      <div class="journey-spine">{% include bridge-line.html variant="journey" %}</div>
      <div>
        <div class="journey-stop">
          <span class="journey-num">01</span>
          <div class="journey-body">
            <h3>Understand biotech</h3>
            <p>Learn what biotechnology actually is through plain-language explanations and real-world examples — no assumed background required.</p>
            <a href="/what-is-biotech/">Explore the basics &rarr;</a>
          </div>
        </div>
        <div class="journey-stop">
          <span class="journey-num">02</span>
          <div class="journey-body">
            <h3>Discover careers</h3>
            <p>See the major career lanes in biotech, with realistic entry points and salary expectations for every kind of background.</p>
            <a href="/career-pathways/">View pathways &rarr;</a>
          </div>
        </div>
        <div class="journey-stop">
          <span class="journey-num">03</span>
          <div class="journey-body">
            <h3>Access resources</h3>
            <p>Browse newsletters, podcasts, courses, and books that are free, beginner-friendly, and hand-picked for quality.</p>
            <a href="/resources/">Browse resources &rarr;</a>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- ============ 3. FOUNDER STORY ============ -->
<div class="hp-band">
  <div class="hp">
    <span class="eyebrow">The story behind BioBridge</span>
    <div class="story-grid" style="margin-top:1.25rem;">
      <div class="story-photo-col">
        <div>
          <div class="story-photo-frame">
            <img class="story-photo" src="/assets/images/profile-photo.jpg" alt="Jean Tran, founder of BioBridge">
          </div>
          <div class="story-caption">
            <strong>Jean Tran</strong>
            Founder, BioBridge<br>BS/MS Biotechnology
          </div>
        </div>
      </div>
      <div class="story-content">
        <p class="lede">I was certain I would become a doctor. In college, I completed the shadowing hours, the prerequisites, the extracurriculars. But the closer I pushed toward a future in clinical work, the more I questioned whether it was actually right for me.</p>
        <p>While searching for alternatives, I discovered my school offered a combined BS/MS in biotechnology I could finish in four years. I knew almost nothing about biotech when I applied — the program revealed just how expansive the field actually is: not just lab work, but business strategy, regulatory policy, manufacturing operations, and more.</p>
        <p>I started documenting what I was learning on social media, and the audience grew quickly. My messages became a constant stream of the same three questions.</p>
        <blockquote class="pull-quote">"What is biotech? How do I get in? Do I need a PhD?"</blockquote>
        <p>People were curious, but they lacked a practical starting point. BioBridge is the resource I wish had existed when I was trying to figure it out.</p>
        <div class="story-connect">
          <span class="story-connect-label">Follow the journey</span>
          <a href="https://instagram.com/jeans.scenes" target="_blank" rel="noopener"><i class="fab fa-instagram" aria-hidden="true"></i> Instagram</a>
          <a href="https://linkedin.com/in/jeantrann" target="_blank" rel="noopener"><i class="fab fa-linkedin" aria-hidden="true"></i> LinkedIn</a>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- ============ 4. CAREER PATH EXPLORER ============ -->
<div class="hp-band hp-band--tint" id="explorer-section">
  <div class="hp">
    <div class="explorer-head">
      <span class="eyebrow">Interactive · updated by hand</span>
      <h2>Find your lane.</h2>
      <p style="color:var(--ink-soft); margin-top:0.75rem;">Filter by where you're coming from and what you're drawn to. Every range below is a rounded, approximate US entry-level estimate — not a promise.</p>
    </div>

    <div id="career-explorer">
      <div class="explorer-filters">
        <div class="filter-group">
          <span class="filter-group-label">Your background</span>
          <div class="explorer-chips" role="group" aria-label="Filter by background">
            <button type="button" class="chip" data-group="background" data-value="biology" aria-pressed="false">Biology</button>
            <button type="button" class="chip" data-group="background" data-value="chemistry" aria-pressed="false">Chemistry</button>
            <button type="button" class="chip" data-group="background" data-value="cs-data" aria-pressed="false">CS / Data</button>
            <button type="button" class="chip" data-group="background" data-value="business" aria-pressed="false">Business</button>
            <button type="button" class="chip" data-group="background" data-value="engineering" aria-pressed="false">Engineering</button>
            <button type="button" class="chip" data-group="background" data-value="non-stem" aria-pressed="false">Non-STEM</button>
          </div>
        </div>
        <div class="filter-group">
          <span class="filter-group-label">What interests you</span>
          <div class="explorer-chips" role="group" aria-label="Filter by interest area">
            <button type="button" class="chip" data-group="interest" data-value="lab-bench" aria-pressed="false">Lab / bench</button>
            <button type="button" class="chip" data-group="interest" data-value="data-computational" aria-pressed="false">Data / computational</button>
            <button type="button" class="chip" data-group="interest" data-value="business-commercial" aria-pressed="false">Business / commercial</button>
            <button type="button" class="chip" data-group="interest" data-value="regulatory-policy" aria-pressed="false">Regulatory / policy</button>
            <button type="button" class="chip" data-group="interest" data-value="manufacturing-operations" aria-pressed="false">Manufacturing / operations</button>
          </div>
        </div>
        <div class="filter-group">
          <span class="filter-group-label">PhD required?</span>
          <div class="explorer-chips" role="group" aria-label="Filter by PhD requirement">
            <button type="button" class="chip" data-group="phd" data-value="not-required" aria-pressed="false">Not required</button>
            <button type="button" class="chip" data-group="phd" data-value="optional" aria-pressed="false">Optional</button>
            <button type="button" class="chip" data-group="phd" data-value="usually-required" aria-pressed="false">Usually required</button>
          </div>
        </div>
        <div class="explorer-toolbar">
          <span class="explorer-count" aria-live="polite"></span>
          <button type="button" class="explorer-reset">Clear filters</button>
        </div>
      </div>
      <div class="explorer-results" aria-live="polite"></div>
    </div>
  </div>
</div>

<!-- ============ 5. LEARNING LAB TEASER ============ -->
<div class="hp-band">
  <div class="hp">
    <span class="eyebrow">Hand-curated, not algorithmic</span>
    <h2>The Learning Lab.</h2>
    <p style="color:var(--ink-soft); margin-top:0.75rem; max-width:640px;">A running library of the newsletters, podcasts, courses, and books that actually explain biotech well — free and beginner-friendly, every one of them vetted before it's added.</p>

    <div class="lab-grid" style="margin-top:2rem;">
      <div class="lab-card lab-card--newsletters">
        <span class="eyebrow">Newsletters</span>
        <h3>What's happening, weekly</h3>
        <p class="lab-desc">Industry news without the jargon wall.</p>
        <div class="lab-logos">
          <img src="/assets/images/logo-wsj.png" alt="The Wall Street Journal" loading="lazy">
          <img src="/assets/images/logo-nature.png" alt="Nature" loading="lazy">
          <img src="/assets/images/logo-fiercebiotech.png" alt="Fierce Biotech" loading="lazy">
          <img src="/assets/images/logo-endpoints.png" alt="Endpoints News" loading="lazy">
        </div>
      </div>
      <div class="lab-card lab-card--podcasts">
        <span class="eyebrow">Podcasts</span>
        <h3>Listen on the commute</h3>
        <p class="lab-desc">Long-form conversations with scientists and builders.</p>
        <div class="lab-logos">
          <img src="/assets/images/logo-radiolab.png" alt="Radiolab" loading="lazy">
          <img src="/assets/images/logo-ologies.png" alt="Ologies" loading="lazy">
          <img src="/assets/images/hidden-brain.png" alt="Hidden Brain" loading="lazy">
          <img src="/assets/images/logo-shortwave.png" alt="Short Wave" loading="lazy">
        </div>
      </div>
      <div class="lab-card lab-card--courses">
        <span class="eyebrow">Courses</span>
        <h3>Go deeper, at your pace</h3>
        <p class="lab-desc">Free, self-paced, no application required.</p>
        <div class="lab-logos">
          <img src="/assets/images/logo-coursera.png" alt="Coursera" loading="lazy">
          <img src="/assets/images/logo-edx.png" alt="edX" loading="lazy">
          <img src="/assets/images/logo-khanacademy.png" alt="Khan Academy" loading="lazy">
          <img src="/assets/images/logo-mitocw.png" alt="MIT OpenCourseWare" loading="lazy">
        </div>
      </div>
      <div class="lab-card lab-card--books">
        <span class="eyebrow">Books</span>
        <h3>For the long read</h3>
        <p class="lab-desc">The ones people actually finish.</p>
        <div class="lab-books-row">
          <img src="/assets/images/book-the-gene.jpg" alt="The Gene, by Siddhartha Mukherjee" loading="lazy">
          <img src="/assets/images/book-henrietta-lacks.jpg" alt="The Immortal Life of Henrietta Lacks" loading="lazy">
          <img src="/assets/images/book-sapiens.png" alt="Sapiens, by Yuval Noah Harari" loading="lazy">
        </div>
      </div>
    </div>
    <p class="lab-more"><a href="/resources/">See the full Learning Lab &rarr;</a></p>
  </div>
</div>

<!-- ============ 6. "DO I NEED A PHD?" MYTH-BUSTER ============ -->
<div class="hp-band hp-band--dark">
  <div class="hp">
    <span class="eyebrow">The question everyone asks</span>
    <h2>Do I need a PhD?</h2>
    <div class="myth-list">
      <div class="myth-item">
        <div>
          <span class="myth-num">Myth 01</span>
          <p class="myth-claim">"You need a PhD to work in biotech."</p>
        </div>
        <p class="myth-reality"><strong>Reality:</strong> Most biotech jobs — manufacturing, quality, regulatory, business, commercial — don't require one. A PhD is the path for a specific kind of research-leadership role, not a prerequisite for the industry.</p>
      </div>
      <div class="myth-item">
        <div>
          <span class="myth-num">Myth 02</span>
          <p class="myth-claim">"You have to be pre-med or a bio major."</p>
        </div>
        <p class="myth-reality"><strong>Reality:</strong> Engineers, chemists, data scientists, business majors, and career-changers with no STEM degree at all have real, active lanes into the field.</p>
      </div>
      <div class="myth-item">
        <div>
          <span class="myth-num">Myth 03</span>
          <p class="myth-claim">"If you're not at the bench, it's not 'real' biotech."</p>
        </div>
        <p class="myth-reality"><strong>Reality:</strong> Regulatory writing, supply chain, quality assurance, and commercial strategy keep therapies moving as much as the science does.</p>
      </div>
      <div class="myth-item">
        <div>
          <span class="myth-num">Myth 04</span>
          <p class="myth-claim">"You have to know your exact lane before you start."</p>
        </div>
        <p class="myth-reality"><strong>Reality:</strong> Most people — Jean included — find their lane by exploring, not by knowing in advance. That's what the explorer above is for.</p>
      </div>
      <div class="myth-item">
        <div>
          <span class="myth-num">Myth 05</span>
          <p class="myth-claim">"It's too late to switch into biotech."</p>
        </div>
        <p class="myth-reality"><strong>Reality:</strong> Career-changers move in at every stage. The on-ramps just look different than a fresh-grad hire.</p>
      </div>
    </div>
  </div>
</div>

<!-- ============ 7. JARGON DECODER ============ -->
<div class="hp-band">
  <div class="hp">
    <span class="eyebrow">Science-notebook glossary</span>
    <h2>The jargon decoder.</h2>
    <p style="color:var(--ink-soft); margin-top:0.75rem; max-width:640px;">Biotech has its own vocabulary. Here's what the most common terms actually mean, in plain English.</p>
    <dl class="jargon-grid">
      <div class="jargon-term"><dt>IND</dt><dd>Investigational New Drug — the application a company files with the FDA for permission to start testing a new drug in humans.</dd></div>
      <div class="jargon-term"><dt>CRO</dt><dd>Contract Research Organization — a company hired to run studies or trials on behalf of a biotech, instead of doing it in-house.</dd></div>
      <div class="jargon-term"><dt>GMP</dt><dd>Good Manufacturing Practice — the quality rules that govern how a drug is actually made, so every batch is safe and consistent.</dd></div>
      <div class="jargon-term"><dt>Pipeline</dt><dd>The list of drugs or products a company currently has in development, from early research through approval.</dd></div>
      <div class="jargon-term"><dt>Biologics</dt><dd>Medicines made from living cells — like antibodies or vaccines — as opposed to chemically synthesized small-molecule drugs.</dd></div>
      <div class="jargon-term"><dt>Assay</dt><dd>A lab test used to measure whether something, like a drug candidate, does what it's supposed to do.</dd></div>
      <div class="jargon-term"><dt>KOL</dt><dd>Key Opinion Leader — an outside expert, often a doctor or researcher, that a company consults or partners with.</dd></div>
      <div class="jargon-term"><dt>Upstream / Downstream</dt><dd>In manufacturing, "upstream" means growing the cells that make the product; "downstream" means purifying and finishing it.</dd></div>
    </dl>
  </div>
</div>

<!-- ============ 8. GET INVOLVED / CLOSE ============ -->
<div class="hp-band hp-band--tint close-band">
  <div class="hp">
    <div class="close-inner">
      {% include bridge-line.html variant="divider" %}
      <span class="eyebrow" style="margin-top:1.25rem;">One more stop</span>
      <h2>The bridge holds up better with more people on it.</h2>
      <p>If BioBridge helped you get somewhere — or you want to help build the next stretch of it — there's a place for you here, no biotech background required.</p>
      <a href="/get-involved/" class="btn-start">Get involved &rarr;</a>
    </div>
  </div>
</div>

<script src="/assets/js/career-data.js"></script>
<script src="/assets/js/career-explorer.js"></script>
