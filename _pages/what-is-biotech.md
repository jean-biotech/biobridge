---
layout: single
title: "What is Biotech?"
permalink: /what-is-biotech/
---

<style>
@import url('https://fonts.googleapis.com/css2?family=Fraunces:ital,opsz,wght@0,9..144,400..600;1,9..144,400..600&family=Instrument+Sans:wght@400;500;600;700&display=swap');
body { font-family: 'Instrument Sans', -apple-system, BlinkMacSystemFont, sans-serif; }
h1, h2, h3 { font-family: 'Fraunces', Georgia, serif; }

:root {
  --bb-green: #24221A;
  --bb-green-accent: #5C6335;
  --bb-green-bright: #5C6335;
  --bb-green-hover: #3B4223;
  --bb-green-dark: #3B4223;
  --bb-green-bg: #E6DBC2;
  --bb-green-bg-subtle: #DED2B7;
  --bb-navy: #24221A;
  --bb-charcoal: #24221A;
  --bb-white: #EFE6D2;
  --bb-off-white: #E6DBC2;
  --bb-text-secondary: #5B5745;
  --bb-gray: #5B5745;
  --bb-border: rgba(36,34,26,0.14);
}

/* Definition caption, set beneath the pull-quote statement */
.bb-definition-caption {
  font-family: 'Instrument Sans', sans-serif;
  font-size: 0.85rem;
  color: var(--bb-gray);
  margin: -1rem 0 1.5rem;
}

/* Section intro text */
.bb-intro-text {
  font-family: 'Instrument Sans', sans-serif;
  font-size: 0.9rem;
  color: #24221A;
  line-height: 1.8;
  margin-bottom: 1.25rem;
}

/* Visual divider with label */
.bb-divider {
  display: flex;
  align-items: center;
  gap: 0.85rem;
  margin: 1.75rem 0;
}
.bb-divider-line {
  flex: 1;
  height: 1px;
  background: var(--bb-border);
}
.bb-divider-label {
  font-family: 'Instrument Sans', sans-serif;
  font-size: 0.67rem;
  font-weight: 700;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  color: var(--bb-green-accent);
  white-space: nowrap;
}
.bb-divider-label .bb-num {
  font-family: 'Fraunces', Georgia, serif;
  font-weight: 500;
  text-transform: none;
  letter-spacing: 0;
  margin-right: 0.5em;
  color: var(--bb-gray);
}

/* ============================================
   FLIP CARDS: Real-World Examples
   ============================================ */
.bb-flip-grid {
  display: grid;
  grid-template-columns: 1fr;
  gap: 1rem;
  margin: 1.25rem 0;
}

.bb-flip-card {
  perspective: 1000px;
  height: 220px;
  cursor: pointer;
}

.bb-flip-card-inner {
  position: relative;
  width: 100%;
  height: 100%;
  transition: transform 0.5s cubic-bezier(0.4, 0, 0.2, 1);
  transform-style: preserve-3d;
}

.bb-flip-card.flipped .bb-flip-card-inner {
  transform: rotateY(180deg);
}

.bb-flip-front,
.bb-flip-back {
  position: absolute;
  width: 100%;
  height: 100%;
  backface-visibility: hidden;
  -webkit-backface-visibility: hidden;
  border-radius: 2px;
  border: 1px solid var(--bb-border);
  overflow: hidden;
}

/* Front of card */
.bb-flip-front {
  background: var(--bb-white);
  display: flex;
  flex-direction: column;
}
.bb-flip-front-img {
  background: var(--bb-off-white);
  height: 110px;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-shrink: 0;
  border-bottom: 1px solid var(--bb-border);
}
.bb-flip-front-body {
  padding: 0.85rem 1rem;
  flex: 1;
}
.bb-flip-front-body h3 {
  font-family: 'Instrument Sans', sans-serif;
  color: var(--bb-navy);
  font-size: 0.92rem;
  font-weight: 700;
  margin: 0 0 0.25rem;
}
.bb-flip-front-body p {
  color: var(--bb-gray);
  font-size: 0.75rem;
  margin: 0;
}
.bb-flip-hint {
  font-family: 'Instrument Sans', sans-serif;
  font-size: 0.62rem;
  color: var(--bb-gray);
  letter-spacing: 0.05em;
  text-transform: uppercase;
}

/* Back of card */
.bb-flip-back {
  background: var(--bb-navy);
  transform: rotateY(180deg);
  display: flex;
  flex-direction: column;
  padding: 1.1rem 1.25rem;
  justify-content: center;
}
.bb-flip-back h3 {
  font-family: 'Instrument Sans', sans-serif;
  color: var(--bb-green-hover);
  font-size: 0.82rem;
  font-weight: 700;
  margin: 0 0 0.5rem;
  text-transform: uppercase;
  letter-spacing: 0.05em;
}
.bb-flip-back p {
  color: rgba(255,255,255,0.85);
  font-size: 0.82rem;
  line-height: 1.65;
  margin: 0 0 0.5rem;
}
.bb-flip-back p:last-child { margin-bottom: 0; }
/* Company name badges on flip card back */
.bb-flip-org-badges {
  display: flex;
  flex-wrap: wrap;
  gap: 0.35rem;
  margin-top: 0.65rem;
}
.bb-flip-org-badge {
  display: inline-block;
  background: rgba(142,148,105,0.18);
  border: 1px solid rgba(142,148,105,0.38);
  border-radius: 2px;
  padding: 0.18rem 0.6rem;
  font-family: 'Instrument Sans', sans-serif;
  font-size: 0.875rem;
  font-weight: 500;
  color: #5C6335;
  letter-spacing: 0.01em;
  white-space: nowrap;
}

/* Two-column split */
.bb-two-col {
  display: grid;
  grid-template-columns: 1fr;
  gap: 1.5rem;
  margin: 1.25rem 0;
  align-items: start;
}
.bb-two-col-text p {
  font-family: 'Instrument Sans', sans-serif;
  color: #24221A;
  font-size: 0.9rem;
  line-height: 1.8;
  margin: 0 0 0.85rem;
}
.bb-two-col-text p:last-child { margin-bottom: 0; }

/* Misconception Blocks */
.bb-misconception {
  background: var(--bb-off-white);
  border: 1px solid var(--bb-border);
  border-radius: 2px;
  padding: 1rem 1.25rem;
  margin-bottom: 0.75rem;
}
.bb-misconception strong {
  color: var(--bb-navy);
  font-family: 'Instrument Sans', sans-serif;
  font-size: 0.88rem;
  font-weight: 600;
}
.bb-misconception p {
  color: var(--bb-text-secondary);
  margin: 0.35rem 0 0;
  font-size: 0.85rem;
  line-height: 1.7;
}

/* Flip card front image fill */
.bb-flip-front-img img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  display: block;
}


/* Beyond the Science image */
.bb-beyond-img {
  width: 100%;
  border-radius: 2px;
  display: block;
}

/* Desktop */
@media (min-width: 769px) {
  .bb-flip-grid { grid-template-columns: repeat(2, 1fr); gap: 1.1rem; }
  .bb-flip-card { height: 240px; }
  .bb-flip-front-img { height: 120px; }
  .bb-two-col { grid-template-columns: 3fr 2fr; gap: 2.25rem; }
}
@media (min-width: 1024px) {
  .bb-flip-grid { grid-template-columns: repeat(4, 1fr); }
}

/* International callout (shared style) */
.bb-international-callout {
  background: #EFE6D2;
  border: 1px solid #E6DBC2;
  border-radius: 2px;
  padding: 1rem 1.25rem;
  margin: 1.75rem 0;
}
.bb-international-callout .bb-intl-header {
  font-family: 'Instrument Sans', sans-serif;
  font-size: 0.82rem;
  font-weight: 700;
  color: var(--bb-green);
  margin: 0 0 0.4rem;
  display: flex;
  align-items: center;
  gap: 0.4rem;
}
.bb-international-callout p {
  font-family: 'Instrument Sans', sans-serif;
  font-size: 0.82rem;
  font-style: italic;
  color: var(--bb-text-secondary);
  line-height: 1.7;
  margin: 0;
}
</style>

<header class="bb-page-header">
  <span class="eyebrow">The Basics</span>
  <h1>What is Biotechnology, Really?</h1>
  <p class="bb-page-header__deck">Understanding the science shaping our future, in plain language, no prerequisites required.</p>
</header>

<ol class="bb-contents">
  <li><span class="bb-contents__num">01</span><a href="#real-world-examples">Real-World Examples</a></li>
  <li><span class="bb-contents__num">02</span><a href="#beyond-the-science">Beyond the Science</a></li>
  <li><span class="bb-contents__num">03</span><a href="#common-misconceptions">Common Misconceptions</a></li>
</ol>

<p class="bb-intro-text">Biotechnology is using living systems (cells, bacteria, proteins, DNA) to create useful products or solve real problems.</p>

<p class="pull-quote">Biotech = biology + technology to solve real problems.</p>
<p class="bb-definition-caption">The simplest definition that actually holds up</p>

<p class="bb-intro-text">It sounds vague because biotech is <strong>incredibly broad</strong>. It touches medicine, agriculture, environmental science, manufacturing, and more. The best way to understand it is through examples.</p>

<div class="bb-divider">
  <div class="bb-divider-line"></div>
  <div class="bb-divider-label"><span class="bb-num">01</span>Real-World Examples</div>
  <div class="bb-divider-line"></div>
</div>

## Real-World Examples

<p class="bb-intro-text" style="font-size:0.82rem; color: var(--bb-gray);">Click each card (or tap on mobile) to see more.</p>

<div class="bb-flip-grid">

  <div class="bb-flip-card" role="button" tabindex="0" aria-label="Medicine example: click to flip">
    <div class="bb-flip-card-inner">
      <div class="bb-flip-front">
        <div class="bb-flip-front-img"><img src="/assets/images/biotech-medicine.jpg" alt="Medicine"></div>
        <div class="bb-flip-front-body">
          <h3>Medicine</h3>
          <p class="bb-flip-hint">Click to learn more</p>
        </div>
      </div>
      <div class="bb-flip-back">
        <h3>Medicine</h3>
        <p>Insulin for diabetics is made by bacteria engineered to carry the human insulin gene. CAR-T therapy takes your own immune cells, genetically reprograms them to recognize cancer, and injects them back.</p>
        <div class="bb-flip-org-badges">
          <span class="bb-flip-org-badge">Moderna</span>
          <span class="bb-flip-org-badge">Pfizer</span>
          <span class="bb-flip-org-badge">Genentech</span>
        </div>
      </div>
    </div>
  </div>

  <div class="bb-flip-card" role="button" tabindex="0" aria-label="Agriculture example: click to flip">
    <div class="bb-flip-card-inner">
      <div class="bb-flip-front">
        <div class="bb-flip-front-img"><img src="/assets/images/biotech-agriculture.jpg" alt="Agriculture"></div>
        <div class="bb-flip-front-body">
          <h3>Agriculture</h3>
          <p class="bb-flip-hint">Click to learn more</p>
        </div>
      </div>
      <div class="bb-flip-back">
        <h3>Agriculture</h3>
        <p>Drought-resistant crops can survive on 30% less water. Plant-based meat uses heme (a protein from engineered yeast) to replicate the taste and texture of beef.</p>
        <div class="bb-flip-org-badges">
          <span class="bb-flip-org-badge">Bayer</span>
          <span class="bb-flip-org-badge">Monsanto</span>
          <span class="bb-flip-org-badge">Syngenta</span>
        </div>
      </div>
    </div>
  </div>

  <div class="bb-flip-card" role="button" tabindex="0" aria-label="Environment example: click to flip">
    <div class="bb-flip-card-inner">
      <div class="bb-flip-front">
        <div class="bb-flip-front-img"><img src="/assets/images/biotech-environment.jpg" alt="Environment"></div>
        <div class="bb-flip-front-body">
          <h3>Environment</h3>
          <p class="bb-flip-hint">Click to learn more</p>
        </div>
      </div>
      <div class="bb-flip-back">
        <h3>Environment</h3>
        <p>Bioremediation uses bacteria that break down petroleum into harmless compounds. Bioplastics made from plants instead of petroleum decompose in months, not centuries.</p>
        <div class="bb-flip-org-badges">
          <span class="bb-flip-org-badge">Bolt Threads</span>
          <span class="bb-flip-org-badge">LanzaTech</span>
          <span class="bb-flip-org-badge">Novozymes</span>
        </div>
      </div>
    </div>
  </div>

  <div class="bb-flip-card" role="button" tabindex="0" aria-label="Cutting Edge example: click to flip">
    <div class="bb-flip-card-inner">
      <div class="bb-flip-front">
        <div class="bb-flip-front-img"><img src="/assets/images/biotech-cuttingedge.jpg" alt="The Cutting Edge"></div>
        <div class="bb-flip-front-body">
          <h3>The Cutting Edge</h3>
          <p class="bb-flip-hint">Click to learn more</p>
        </div>
      </div>
      <div class="bb-flip-back">
        <h3>The Cutting Edge</h3>
        <p>Bioprinting uses 3D printers loaded with living cells to build skin grafts, cartilage, and blood vessels. Mini-brains grown from stem cells are helping scientists study Alzheimer's without human trials.</p>
        <div class="bb-flip-org-badges">
          <span class="bb-flip-org-badge">10x Genomics</span>
          <span class="bb-flip-org-badge">CRISPR Therapeutics</span>
          <span class="bb-flip-org-badge">Illumina</span>
        </div>
      </div>
    </div>
  </div>

</div>

<div class="bb-divider">
  <div class="bb-divider-line"></div>
  <div class="bb-divider-label"><span class="bb-num">02</span>Beyond the Lab</div>
  <div class="bb-divider-line"></div>
</div>

## Beyond the Science

<div class="bb-two-col">
  <div class="bb-two-col-text">
    <p>A breakthrough in the lab is just the beginning. Getting from concept to the real world takes an entire team, and most of them aren't scientists.</p>
    <p>Take mRNA vaccines. The underlying science existed for decades. Turning it into something that reached billions of people took business strategists, regulatory experts, manufacturing engineers, ethicists, and communicators working in parallel.</p>
    <p>Someone had to decide what was worth pursuing and who would pay for it. Someone had to design safe trials and navigate the FDA. Someone had to figure out how to manufacture at scale without losing efficacy. Someone had to explain a brand-new technology to a skeptical public.</p>
    <p>That's why biotech needs business people, engineers, lawyers, writers, and project managers just as much as it needs scientists.</p>
  </div>
  <div>
    <img src="/assets/images/team-illustration.jpg?v=2" alt="Cross-functional team behind a biotech breakthrough" class="bb-beyond-img">
  </div>
</div>

<div class="bb-divider">
  <div class="bb-divider-line"></div>
  <div class="bb-divider-label"><span class="bb-num">03</span>Common Misconceptions</div>
  <div class="bb-divider-line"></div>
</div>

## Common Misconceptions

<div class="bb-misconception">
  <strong>"You need to be good at biology to work in the industry."</strong>
  <p>Not necessarily. Biotech employs humanities majors, business students, and engineers just as readily as biology PhDs. Science communication, operations, and regulatory affairs are all viable without a lab background.</p>
</div>

<div class="bb-misconception">
  <strong>"It's all lab work."</strong>
  <p>Lab work is one slice of a much bigger picture. There's also manufacturing, regulatory affairs, sales, policy, data analysis, and more. The <a href="/career-pathways/" style="color: #5C6335; font-weight: 600;">Career Pathways</a> page shows the full range.</p>
</div>

<div class="bb-misconception">
  <strong>"You need a PhD."</strong>
  <p>Only if you want to lead independent research. Most biotech jobs in regulatory, manufacturing, business, and operations require a bachelor's degree or less. Certificate programs can get you there in months, and there are entry points at every level.</p>
</div>

<!-- Regulatory context callout -->
<div class="bb-international-callout">
  <div class="bb-intl-header">Outside the US?</div>
  <p>Regulatory terminology varies by country. FDA = United States Food and Drug Administration. EMA = European Medicines Agency (EU). Health Canada oversees drug approvals in Canada. PMDA (Pharmaceuticals and Medical Devices Agency) regulates in Japan. When you see terms like "IND filing" or "NDA" below, those are US-specific. Equivalent processes exist in other jurisdictions under different names and timelines.</p>
</div>

<script>
// Click-to-flip support for mobile/keyboard
(function() {
  var cards = document.querySelectorAll('.bb-flip-card');
  cards.forEach(function(card) {
    card.addEventListener('click', function() {
      card.classList.toggle('flipped');
    });
    card.addEventListener('keydown', function(e) {
      if (e.key === 'Enter' || e.key === ' ') {
        e.preventDefault();
        card.classList.toggle('flipped');
      }
    });
  });
})();
</script>
