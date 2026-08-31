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
  --bb-navy: #24221A;
  --bb-white: #EFE6D2;
  --bb-off-white: #E6DBC2;
  --bb-text-secondary: #5B5745;
  --bb-gray: #5B5745;
  --bb-border: rgba(36,34,26,0.12);
}

/* Definition caption, set beneath the pull-quote statement:
   Fraunces italic, quiet, 60% opacity, no rotation. */
.bb-definition-caption {
  font-family: 'Fraunces', Georgia, serif;
  font-style: italic;
  font-size: 15px;
  color: var(--bb-navy);
  opacity: 0.6;
  margin: -1rem 0 1.5rem;
}

/* Contents list: large graphic numerals, plain hairline rows. */
.bb-contents-notes {
  list-style: none;
  margin: 0 0 2.5rem;
  padding: 0;
  border-top: 1px solid var(--bb-border);
}
.bb-contents-notes li {
  display: flex;
  align-items: baseline;
  flex-wrap: wrap;
  column-gap: 0.9rem;
  row-gap: 0.15rem;
  padding: 0.9rem 0;
  border-bottom: 1px solid var(--bb-border);
}
.bb-contents-notes__num {
  font-family: 'Fraunces', Georgia, serif;
  font-size: 30px;
  font-weight: 500;
  color: var(--bb-green-accent);
  line-height: 1;
  min-width: 2.4rem;
}
.bb-contents-notes a {
  font-family: 'Fraunces', Georgia, serif;
  font-size: 17px;
  font-weight: 600;
  color: var(--bb-navy);
}
.bb-contents-notes__hint {
  font-family: 'Fraunces', Georgia, serif;
  font-style: italic;
  font-size: 15px;
  color: var(--bb-navy);
  opacity: 0.6;
  display: inline-block;
}

/* Section intro text */
.bb-intro-text {
  font-family: 'Instrument Sans', sans-serif;
  font-size: 17px;
  color: #24221A;
  opacity: 0.82;
  line-height: 1.65;
  margin-bottom: 1.25rem;
  max-width: 62ch;
}

/* Visual divider with label: a hairline rule and a label, no box */
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
  font-size: 11px;
  font-weight: 600;
  letter-spacing: 0.16em;
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
   REAL-WORLD EXAMPLES: rule-divided rows, not
   flip cards with stock photography.
   ============================================ */
.bb-flip-grid {
  border-top: 1px solid var(--bb-border);
  margin: 1.25rem 0;
}
.bb-flip-card {
  border-bottom: 1px solid var(--bb-border);
  padding: 1.5rem 0;
  cursor: pointer;
}
.bb-flip-front-body h3 {
  font-family: 'Fraunces', Georgia, serif;
  color: var(--bb-navy);
  font-size: 17px;
  font-weight: 600;
  margin: 0 0 0.4rem;
}
.bb-flip-front-body p {
  color: var(--bb-gray);
  opacity: 0.7;
  font-size: 17px;
  margin: 0;
}
.bb-flip-hint {
  font-family: 'Instrument Sans', sans-serif;
  font-size: 11px;
  letter-spacing: 0.16em;
  text-transform: uppercase;
  color: var(--bb-green-accent);
}

.bb-flip-card.flipped .bb-flip-front { display: none; }
.bb-flip-back { display: none; }
.bb-flip-card.flipped .bb-flip-back { display: block; }
.bb-flip-back h3 {
  font-family: 'Fraunces', Georgia, serif;
  color: var(--bb-navy);
  font-size: 17px;
  font-weight: 600;
  margin: 0 0 0.6rem;
}
.bb-flip-back p {
  color: var(--bb-text-secondary);
  opacity: 0.82;
  font-size: 17px;
  line-height: 1.65;
  margin: 0 0 0.65rem;
}
.bb-flip-back p:last-child { margin-bottom: 0; }
.bb-flip-org-badges {
  display: flex;
  flex-wrap: wrap;
  gap: 0.4rem 0.9rem;
  margin-top: 0.75rem;
}
.bb-flip-org-badge {
  font-family: 'Instrument Sans', sans-serif;
  font-size: 15px;
  color: var(--bb-green-accent);
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
  opacity: 0.82;
  font-size: 17px;
  line-height: 1.65;
  margin: 0 0 0.85rem;
  max-width: 62ch;
}
.bb-two-col-text p:last-child { margin-bottom: 0; }

/* The one remaining photo on this page: straight edge, no tilt,
   no shadow. Caption sits where the handwritten Caveat mark used
   to: Fraunces italic, quiet, 60% opacity. */
.bb-photo-frame {
  display: block;
  max-width: 100%;
}
.bb-photo-frame img {
  display: block;
  width: 100%;
  height: auto;
  border: 1px solid var(--bb-border);
}
.bb-photo-frame__caption {
  display: block;
  font-family: 'Fraunces', Georgia, serif;
  font-style: italic;
  font-size: 15px;
  color: var(--bb-navy);
  opacity: 0.6;
  margin-top: 0.5rem;
}

/* Misconception rows: a rule, not a filled block */
.bb-misconception {
  border-top: 1px solid var(--bb-border);
  padding: 1.1rem 0;
}
.bb-misconception:last-of-type {
  border-bottom: 1px solid var(--bb-border);
}
.bb-misconception strong {
  color: var(--bb-navy);
  font-family: 'Instrument Sans', sans-serif;
  font-size: 17px;
  font-weight: 600;
}
.bb-misconception p {
  color: var(--bb-text-secondary);
  opacity: 0.82;
  margin: 0.4rem 0 0;
  font-size: 17px;
  line-height: 1.65;
  max-width: 62ch;
}

/* International callout (shared style): rules, no box */
.bb-international-callout {
  border-top: 1px solid var(--bb-border);
  border-bottom: 1px solid var(--bb-border);
  padding: 1.5rem 0;
  margin: 1.75rem 0;
  max-width: 62ch;
}
.bb-international-callout .bb-intl-header {
  font-family: 'Instrument Sans', sans-serif;
  font-size: 11px;
  font-weight: 600;
  text-transform: uppercase;
  letter-spacing: 0.16em;
  color: var(--bb-green-accent);
  margin: 0 0 0.5rem;
}
.bb-international-callout p {
  font-family: 'Instrument Sans', sans-serif;
  font-size: 17px;
  font-style: italic;
  color: var(--bb-text-secondary);
  opacity: 0.82;
  line-height: 1.65;
  margin: 0;
}

/* Desktop */
@media (min-width: 769px) {
  .bb-two-col { grid-template-columns: 3fr 2fr; gap: 2.25rem; }
}
</style>

<header class="bb-page-header">
  <span class="eyebrow">The Basics</span>
  <h1>What is Biotechnology, Really?</h1>
  <p class="bb-page-header__deck">Understanding the science shaping our future, in plain language, no prerequisites required.</p>
</header>

<ul class="bb-contents-notes">
  <li>
    <span class="bb-contents-notes__num">01</span>
    <a href="#real-world-examples">Real-World Examples</a>
    <span class="bb-contents-notes__hint">skip to the good stuff</span>
  </li>
  <li>
    <span class="bb-contents-notes__num">02</span>
    <a href="#beyond-the-science">Beyond the Science</a>
    <span class="bb-contents-notes__hint">more than lab coats, promise</span>
  </li>
  <li>
    <span class="bb-contents-notes__num">03</span>
    <a href="#common-misconceptions">Common Misconceptions</a>
    <span class="bb-contents-notes__hint">read this if you're unsure you belong</span>
  </li>
</ul>

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

<p class="bb-intro-text" style="font-size:15px; color: var(--bb-gray); opacity: 0.7;">Click each row (or tap on mobile) to see more.</p>

<div class="bb-flip-grid">

  <div class="bb-flip-card" role="button" tabindex="0" aria-label="Medicine example: click to flip">
    <div class="bb-flip-front">
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

  <div class="bb-flip-card" role="button" tabindex="0" aria-label="Agriculture example: click to flip">
    <div class="bb-flip-front">
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

  <div class="bb-flip-card" role="button" tabindex="0" aria-label="Environment example: click to flip">
    <div class="bb-flip-front">
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

  <div class="bb-flip-card" role="button" tabindex="0" aria-label="Cutting Edge example: click to flip">
    <div class="bb-flip-front">
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
    <div class="bb-photo-frame">
      <img src="/assets/images/team-illustration.jpg?v=2" alt="Cross-functional team behind a biotech breakthrough">
    </div>
    <span class="bb-photo-frame__caption">not a single lab coat in sight</span>
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
  <p>Lab work is one slice of a much bigger picture. There's also manufacturing, regulatory affairs, sales, policy, data analysis, and more. The <a href="/career-pathways/">Career Pathways</a> page shows the full range.</p>
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
