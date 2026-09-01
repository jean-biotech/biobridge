---
layout: splash
title: " "
classes: wide
---

<style>
/* ================================================================
   Homepage: editorial layout built on the global tokens in
   assets/css/main.scss (--paper, --paper-2, --taupe, --ink,
   --ink-soft, --olive, --olive-deep, --olive-soft, --line).
   Olive is the only accent. No monospace anywhere.
   ================================================================ */

.hp { max-width: 1160px; margin: 0 auto; padding: 0 var(--s3); }
.hp-band { padding: var(--space-section) 0; }
.hp-band + .hp-band { border-top: 1px solid var(--line); }
.hp-band--tint { background: var(--paper-2); }
.hp .eyebrow { margin-bottom: var(--s2); display: inline-block; }
.hp h2 { font-size: var(--fs-heading); margin: 0; }

/* A section's lead-in paragraph. Sits at prose measure even where the
   content below it runs wider. */
.section-deck {
  color: var(--ink);
  opacity: 0.9;
  font-size: var(--fs-body);
  line-height: 1.6;
  margin: var(--s3) 0 0;
  max-width: var(--measure);
}
/* The Learning Lab opens tighter than the other sections: the deck
   hands straight off to the lists rather than sitting in its own band
   of space. */
.lab-deck { margin-bottom: var(--s5); }

/* The one big typographic quote moment on the page: Fraunces italic
   at the section-heading size, standing on its own, no box, no tilt. */
.pull-quote--feature {
  font-size: var(--fs-heading);
  max-width: var(--measure);
  margin: var(--s4) 0;
}

/* ---------------- Hero: single column, full measure, no reserved empty space ---------------- */
.hero {
  padding-top: var(--s4);
  padding-bottom: var(--s4);
}
.hero-copy { max-width: 700px; }
.hero-copy h1 {
  font-size: var(--fs-display);
  font-weight: 500;
  line-height: 1.05;
  letter-spacing: -0.01em;
  margin: var(--s2) 0 var(--s3);
  color: var(--ink);
}
.hero-copy h1 em {
  font-style: italic;
}
.hero-copy .hero-sub {
  font-size: var(--fs-body);
  color: var(--ink);
  opacity: 0.9;
  line-height: 1.6;
  margin: 0 0 var(--s4);
  max-width: var(--measure);
}
.hero-actions { display: flex; flex-wrap: wrap; align-items: center; gap: var(--s4); margin-bottom: var(--s4); }
.btn-start {
  display: inline-flex;
  align-items: center;
  gap: var(--s1);
  background: var(--olive);
  color: var(--paper) !important;
  font-family: var(--font-body);
  font-weight: 600;
  font-size: var(--fs-body);
  padding: var(--s2) var(--s3);
  border-radius: 0;
  text-decoration: none !important;
  transition: background 0.15s ease;
}
.btn-start:hover { background: var(--olive-deep); color: var(--paper) !important; }
.hero-quiet-links { display: flex; flex-direction: column; gap: var(--s1); }
.hero-quiet-links a {
  font-family: var(--font-body);
  font-size: var(--fs-body);
  font-weight: 500;
  color: var(--ink) !important;
  opacity: 0.9;
  text-decoration: underline !important;
  text-decoration-color: rgba(59, 66, 35, 0.35) !important;
  text-underline-offset: 2px;
  width: fit-content;
  transition: color 0.15s ease, opacity 0.15s ease;
}
.hero-quiet-links a:hover { color: var(--olive-deep) !important; opacity: 1; text-decoration-color: currentColor !important; }

/* Where the handwritten Caveat pull quote used to sit: Fraunces
   italic at body size, quieter by voice rather than by a smaller size. */
.hero-honest-line {
  font-family: var(--font-display);
  font-style: italic;
  font-size: var(--fs-body);
  color: var(--ink);
  opacity: 0.8;
  max-width: var(--measure);
  margin-top: var(--s2);
}

/* ---------------- How BioBridge works: hanging numerals, no ruled rows ---------------- */
.works-head { max-width: var(--measure); margin-bottom: var(--s4); }
.works-list { display: flex; flex-direction: column; gap: var(--s4); }
.works-row {
  display: grid;
  grid-template-columns: 24px 1fr;
  align-items: baseline;
  gap: var(--s3);
  text-decoration: none !important;
  color: inherit !important;
}
.works-row__num {
  font-family: var(--font-display);
  font-weight: 500;
  font-size: var(--fs-body);
  color: var(--ink);
  opacity: 0.45;
}
.works-row__title {
  font-family: var(--font-display);
  font-size: var(--fs-body);
  font-weight: 600;
  margin: 0 0 var(--s1);
  color: var(--ink);
  display: inline-block;
  text-decoration: underline;
  text-decoration-color: transparent;
  text-underline-offset: 3px;
  transition: text-decoration-color 0.15s ease;
}
.works-row:hover .works-row__title { text-decoration-color: var(--olive); }
.works-row__desc { font-family: var(--font-body); font-size: var(--fs-body); line-height: 1.6; color: var(--ink); opacity: 0.9; margin: 0; max-width: var(--measure); }
/* The row is a link and the title underline on hover says so, so the
   arrow glyph no longer has to. */
.works-row__arrow { display: none; }

/* ---------------- Founder story: photo + bio side by side ---------------- */
.story-grid { display: grid; grid-template-columns: 1fr; gap: var(--s4); margin-top: var(--s3); }
.story-photo {
  width: 100%;
  max-width: 220px;
  aspect-ratio: 1 / 1;
  object-fit: cover;
  display: block;
}
.story-byline { display: flex; flex-direction: column; gap: var(--s1); margin-top: var(--s2); }
.story-byline .name { font-family: var(--font-display); font-size: var(--fs-body); font-weight: 600; color: var(--ink); }
.story-byline .role { font-family: var(--font-body); font-size: var(--fs-label); text-transform: uppercase; letter-spacing: 0.16em; color: var(--olive); }
.story-content p { color: var(--ink); opacity: 0.9; line-height: 1.6; margin-bottom: var(--s3); font-size: var(--fs-body); max-width: var(--measure); }
.story-connect { display: flex; align-items: baseline; gap: var(--s3); flex-wrap: wrap; margin-top: var(--s4); }
.story-connect-label { font-family: var(--font-body); font-size: var(--fs-label); text-transform: uppercase; letter-spacing: 0.16em; color: var(--olive); }
.story-connect a {
  font-family: var(--font-body); font-weight: 500; font-size: var(--fs-body);
  color: var(--ink) !important;
  opacity: 0.9;
}
.story-connect a:hover { color: var(--olive-deep) !important; opacity: 1; }

@media (min-width: 700px) {
  .story-grid { grid-template-columns: 220px 1fr; gap: var(--s5); align-items: start; }
}

/* ---------------- Career Explorer ---------------- */
.explorer-head { max-width: var(--measure); margin-bottom: var(--s4); }
.explorer-filters {
  padding: 0;
  margin-bottom: var(--s5);
}
.filter-group { margin-bottom: var(--s4); }
.filter-group:last-child { margin-bottom: 0; }
.filter-group-label {
  display: block;
  font-family: var(--font-body);
  font-size: var(--fs-label);
  font-weight: 600;
  text-transform: uppercase;
  letter-spacing: 0.16em;
  color: var(--olive);
  margin-bottom: var(--s1);
}

/* Filters read as a line of choices, not a toolbar: no borders, no
   fills, no rectangles. State is carried by weight, color, underline. */
.explorer-chips { display: flex; flex-wrap: wrap; gap: var(--s2) var(--s3); }
.chip {
  font-family: var(--font-body);
  font-size: var(--fs-body);
  font-weight: 400;
  padding: 0;
  border: none;
  border-radius: 0;
  background: transparent;
  color: var(--ink);
  opacity: 0.7;
  cursor: pointer;
  text-decoration: underline;
  text-decoration-color: transparent;
  text-decoration-thickness: 1px;
  text-underline-offset: 4px;
  transition: color 0.15s ease, opacity 0.15s ease, text-decoration-color 0.15s ease;
}
.chip:hover { opacity: 1; text-decoration-color: var(--line); }
.chip[aria-pressed="true"] {
  color: var(--olive-deep);
  opacity: 1;
  font-weight: 600;
  text-decoration-color: currentColor;
}
.explorer-toolbar { display: flex; align-items: baseline; gap: var(--s3); margin-top: var(--s4); }
.explorer-count { font-family: var(--font-body); font-size: var(--fs-label); text-transform: uppercase; letter-spacing: 0.16em; color: var(--ink); opacity: 0.8; }
.explorer-reset {
  font-family: var(--font-body);
  font-size: var(--fs-label);
  letter-spacing: 0.16em;
  text-transform: uppercase;
  font-weight: 600;
  color: var(--olive-deep);
  background: none;
  border: none;
  cursor: pointer;
  padding: 0;
}
.explorer-reset:hover { color: var(--olive); }
.explorer-results { display: grid; grid-template-columns: 1fr; gap: var(--s4); }
.explorer-empty { color: var(--ink); opacity: 0.8; font-style: italic; padding: var(--s4) 0; }
.role-card {
  padding: 0;
}
.role-card__top { display: flex; align-items: baseline; gap: var(--s2); margin-bottom: var(--s1); flex-wrap: wrap; }
.role-card__title { margin: 0; font-size: var(--fs-body); font-family: var(--font-display); font-weight: 600; color: var(--ink); }
/* Match/maybe/later reads as a small label beside the role name, not a
   bordered tag. */
.badge {
  font-family: var(--font-body);
  font-size: var(--fs-label);
  font-weight: 600;
  text-transform: uppercase;
  letter-spacing: 0.16em;
  padding: 0;
  border: none;
  white-space: nowrap;
  flex-shrink: 0;
}
.badge--go { color: var(--olive); }
.badge--maybe { color: var(--ink); opacity: 0.8; }
.badge--later { color: var(--ink); opacity: 0.8; }
.role-card__salary { font-size: var(--fs-body); color: var(--ink); margin: 0 0 0.65rem; line-height: 1.5; }
.role-card__salary .eyebrow { color: var(--olive); }
.role-card__step { font-size: var(--fs-body); color: var(--ink); opacity: 0.9; line-height: 1.6; margin: 0 0 var(--s2); max-width: var(--measure); }
.role-card__link { font-family: var(--font-body); font-weight: 600; font-size: var(--fs-body); color: var(--olive-deep); }

@media (min-width: 700px) { .explorer-results { grid-template-columns: repeat(2, 1fr); column-gap: var(--s5); } }

/* ---------------- Learning Lab: grouped by space, not ruled ---------------- */
.lab-grid { display: grid; grid-template-columns: 1fr; gap: var(--s5); }
.lab-card { padding: 0; }
.lab-card h3 { font-size: var(--fs-body); font-weight: 600; margin: 0 0 var(--s1); color: var(--ink); }
.lab-card .eyebrow { display: block; margin-bottom: var(--s1); }
.lab-card p.lab-desc { color: var(--ink); opacity: 0.9; font-size: var(--fs-body); line-height: 1.6; margin: 0 0 var(--s3); }
.lab-logos { display: flex; flex-wrap: wrap; align-items: center; gap: var(--s3); }
.lab-logos img { height: 28px; width: auto; max-width: 100px; object-fit: contain; }
.lab-books-row { display: flex; gap: var(--s1); }
.lab-books-row img { width: 52px; height: 76px; object-fit: cover; }
.lab-more { margin-top: var(--s5); }
.lab-more a { font-weight: 600; color: var(--olive-deep); }

@media (min-width: 900px) {
  .lab-grid { grid-template-columns: repeat(2, 1fr); column-gap: var(--s5); row-gap: var(--s5); }
}

/* ---------------- Close ---------------- */
.close-band { text-align: left; }
.close-inner { max-width: var(--measure); }
.close-inner h2 { font-size: var(--fs-heading); margin: 0 0 var(--s3); }
.close-inner p { color: var(--ink); opacity: 0.9; font-size: var(--fs-body); line-height: 1.6; margin: 0 0 var(--s4); max-width: var(--measure); }
</style>

<!-- ============ HERO ============ -->
<div class="hp">
  <div class="hero">
    <div class="hero-copy">
      <span class="eyebrow">Student-led biotech initiative</span>
      <h1>Bridging the gap between <em>curiosity</em> and careers in biotechnology</h1>
      <p class="hero-sub">Clear explanations, curated resources, and practical guidance for anyone exploring the world of biotech.</p>
      <div class="hero-actions">
        <a href="/what-is-biotech/" class="btn-start">Start here</a>
        <div class="hero-quiet-links">
          <a href="/career-pathways/">Explore careers</a>
          <a href="/products/">Browse the guides</a>
        </div>
      </div>
      <p class="hero-honest-line">"My messages became a constant stream of the same questions."</p>
    </div>
  </div>
</div>

<!-- ============ HOW BIOBRIDGE WORKS: numbered editorial list ============ -->
<div class="hp-band hp-band--tint">
  <div class="hp">
    <div class="works-head">
      <span class="eyebrow">What BioBridge offers</span>
      <h2>Clear explanations, curated resources, and honest guidance.</h2>
    </div>
    <div class="works-list">
      <a href="/what-is-biotech/" class="works-row">
        <span class="works-row__num">01</span>
        <span>
          <span class="works-row__title">Understand biotech</span>
          <p class="works-row__desc">Learn what biotechnology really is through real-world examples and plain-language explanations that make the science accessible.</p>
        </span>
        <span class="works-row__arrow">&rarr;</span>
      </a>
      <a href="/career-pathways/" class="works-row">
        <span class="works-row__num">02</span>
        <span>
          <span class="works-row__title">Discover careers</span>
          <p class="works-row__desc">Explore the major career pathways in biotech, with realistic entry points, salary expectations, and guidance for every background.</p>
        </span>
        <span class="works-row__arrow">&rarr;</span>
      </a>
      <a href="/resources/" class="works-row">
        <span class="works-row__num">03</span>
        <span>
          <span class="works-row__title">Access resources</span>
          <p class="works-row__desc">Browse curated newsletters, podcasts, courses, and books that are all free, beginner-friendly, and hand-picked for quality.</p>
        </span>
        <span class="works-row__arrow">&rarr;</span>
      </a>
    </div>
  </div>
</div>

<!-- ============ FOUNDER STORY ============ -->
<div class="hp-band">
  <div class="hp">
    <span class="eyebrow">The story behind BioBridge</span>
    <div class="story-grid">
      <div>
        <img class="story-photo" src="/assets/images/profile-photo.jpg" alt="Jean Tran, founder of BioBridge">
        <div class="story-byline">
          <span class="name">Jean Tran</span>
          <span class="role">Founder, BioBridge &middot; BS/MS Biotechnology</span>
        </div>
      </div>
      <div class="story-content">
        <p class="lede">I was certain I would become a doctor. In college, I completed the shadowing hours, prerequisites, and extracurriculars. But the closer I pushed myself toward a future in clinical work, the more I questioned whether it was actually right for me. I realized I needed a different direction.</p>
        <p>While searching for alternatives, I discovered my school offered a combined BS/MS in biotechnology that I could complete in four years. I knew almost nothing about biotech when I applied, but the program revealed just how expansive the field actually is, spanning lab work, business strategy, regulatory policy, manufacturing operations, and more.</p>
        <p>I started documenting what I was learning on social media, and the audience grew quickly. Tens of thousands of people followed along, and my messages became a constant stream of the same questions.</p>
        <blockquote class="pull-quote pull-quote--feature">"What is biotech? How do I get in? Do I need a PhD?"</blockquote>
        <p>People were curious, but lacked a practical starting point. BioBridge is the resource I wish had existed when I was trying to figure it out.</p>
        <div class="story-connect">
          <span class="story-connect-label">Follow the journey:</span>
          <a href="https://instagram.com/jeans.scenes" target="_blank" rel="noopener">Instagram</a>
          <a href="https://linkedin.com/in/jeantrann" target="_blank" rel="noopener">LinkedIn</a>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- ============ CAREER PATH EXPLORER ============ -->
<div class="hp-band hp-band--tint" id="explorer-section">
  <div class="hp">
    <div class="explorer-head">
      <span class="eyebrow">A tool to try</span>
      <h2>Find your lane.</h2>
      <p class="section-deck">Filter by where you're coming from and what you're drawn to. Every range below is a rounded, approximate US entry-level estimate, not a promise.</p>
    </div>

    <div id="career-explorer">
      <div class="explorer-filters">
        <div class="filter-group">
          <span class="filter-group-label">Your background</span>
          <div class="explorer-chips" role="group" aria-label="Filter by background">
            <button type="button" class="chip" data-group="background" data-value="biology" aria-pressed="false">Biology</button>
            <button type="button" class="chip" data-group="background" data-value="chemistry" aria-pressed="false">Chemistry</button>
            <button type="button" class="chip" data-group="background" data-value="cs-data" aria-pressed="false">CS / data</button>
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

<!-- ============ LEARNING LAB ============ -->
<div class="hp-band">
  <div class="hp">
    <span class="eyebrow">Hand-picked, not algorithmic</span>
    <h2>The Learning Lab.</h2>
    <p class="section-deck lab-deck">A running library of the newsletters, podcasts, courses, and books that actually explain biotech well. Free and beginner-friendly, every one of them checked before it's added.</p>

    <div class="lab-grid">
      <div class="lab-card">
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
      <div class="lab-card">
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
      <div class="lab-card">
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
      <div class="lab-card">
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

<!-- ============ CLOSE ============ -->
<div class="hp-band hp-band--tint close-band">
  <div class="hp">
    <div class="close-inner">
      <span class="eyebrow">Ready to explore biotechnology?</span>
      <h2>Discover career pathways, free resources, and real guidance from someone who has been there.</h2>
      <a href="/what-is-biotech/" class="btn-start">Learn more</a>
    </div>
  </div>
</div>

<script src="/assets/js/career-data.js"></script>
<script src="/assets/js/career-explorer.js"></script>
