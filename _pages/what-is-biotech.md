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
   Fraunces italic at body size, quiet by voice not by size. */
.bb-definition-caption {
  font-family: 'Fraunces', Georgia, serif;
  font-style: italic;
  font-size: 17px;
  color: var(--bb-navy);
  opacity: 0.8;
  margin: 0 0 var(--s5);
}

/* Contents list: hanging numerals, grouped by space, no rules. */
.bb-contents-notes {
  list-style: none;
  margin: 0 0 var(--s6);
  padding: 0;
}
.bb-contents-notes li {
  display: grid;
  grid-template-columns: 24px 1fr;
  align-items: baseline;
  column-gap: var(--s3);
  row-gap: var(--s1);
  padding: 0 0 var(--s3);
}
.bb-contents-notes__num {
  font-family: 'Fraunces', Georgia, serif;
  font-size: 17px;
  font-weight: 500;
  color: var(--bb-navy);
  opacity: 0.45;
  line-height: 1.6;
}
.bb-contents-notes a {
  font-family: 'Fraunces', Georgia, serif;
  font-size: 17px;
  font-weight: 600;
  color: var(--bb-navy);
}
.bb-contents-notes__hint {
  grid-column: 2;
  font-family: 'Fraunces', Georgia, serif;
  font-style: italic;
  font-size: 17px;
  color: var(--bb-navy);
  opacity: 0.8;
  display: inline-block;
}

/* Section intro text */
.bb-intro-text {
  font-family: 'Instrument Sans', sans-serif;
  font-size: 17px;
  color: #24221A;
  opacity: 0.9;
  line-height: 1.6;
  margin-bottom: var(--s3);
  max-width: var(--measure);
}

/* A one-line instruction under a heading */
.bb-section-hint {
  font-family: 'Instrument Sans', sans-serif;
  font-size: 11px;
  text-transform: uppercase;
  letter-spacing: 0.16em;
  color: var(--bb-gray);
  opacity: 0.8;
  margin: 0 0 var(--s3);
}

/* Chapter marker: a hanging numeral and a label, no flanking rules. */
.bb-divider {
  display: grid;
  grid-template-columns: 24px 1fr;
  align-items: baseline;
  gap: var(--s3);
  margin: var(--s6) 0 var(--s4);
}
.bb-divider .bb-num {
  font-family: 'Fraunces', Georgia, serif;
  font-weight: 500;
  font-size: 17px;
  color: var(--bb-navy);
  opacity: 0.45;
}
.bb-divider-label {
  font-family: 'Instrument Sans', sans-serif;
  font-size: 11px;
  font-weight: 600;
  letter-spacing: 0.16em;
  text-transform: uppercase;
  color: var(--bb-green-accent);
}

/* ============================================
   REAL-WORLD EXAMPLES: expandable entries,
   grouped by space rather than ruled rows.
   ============================================ */
.bb-flip-grid {
  display: grid;
  grid-template-columns: 1fr;
  gap: var(--s5);
  margin: var(--s3) 0 var(--s6);
}
.bb-flip-card {
  padding: 0;
  cursor: pointer;
}
.bb-flip-front-body h3 {
  font-family: 'Fraunces', Georgia, serif;
  color: var(--bb-navy);
  font-size: 17px;
  font-weight: 600;
  margin: 0 0 var(--s1);
}
.bb-flip-front-body p {
  color: var(--bb-gray);
  opacity: 0.9;
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
  margin: 0 0 var(--s2);
}
.bb-flip-back p {
  color: var(--bb-text-secondary);
  opacity: 0.9;
  font-size: 17px;
  line-height: 1.6;
  margin: 0 0 var(--s2);
  max-width: var(--measure);
}
.bb-flip-back p:last-child { margin-bottom: 0; }
.bb-flip-org-badges {
  display: flex;
  flex-wrap: wrap;
  gap: var(--s1) var(--s3);
  margin-top: var(--s2);
}
.bb-flip-org-badge {
  font-family: 'Instrument Sans', sans-serif;
  font-size: 17px;
  color: var(--bb-green-accent);
}

@media (min-width: 769px) {
  .bb-flip-grid { grid-template-columns: repeat(2, 1fr); column-gap: var(--s5); }
}

/* Two-column split: prose beside the photo */
.bb-two-col {
  display: grid;
  grid-template-columns: 1fr;
  gap: var(--s4);
  margin: var(--s3) 0 var(--s6);
  align-items: start;
}
.bb-two-col-text p {
  font-family: 'Instrument Sans', sans-serif;
  color: #24221A;
  opacity: 0.9;
  font-size: 17px;
  line-height: 1.6;
  margin: 0 0 var(--s3);
  max-width: var(--measure);
}
.bb-two-col-text p:last-child { margin-bottom: 0; }

/* The one remaining photo on this page: straight edge, no tilt,
   no shadow. Caption in Fraunces italic at body size. */
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
  font-size: 17px;
  color: var(--bb-navy);
  opacity: 0.8;
  margin-top: var(--s2);
}

/* Misconceptions: the claim in quotes, the answer beneath it.
   Grouped by space, no rules. */
.bb-misconception {
  padding: 0 0 var(--s4);
}
.bb-misconception strong {
  color: var(--bb-navy);
  font-family: 'Fraunces', Georgia, serif;
  font-size: 17px;
  font-weight: 600;
}
.bb-misconception p {
  color: var(--bb-text-secondary);
  opacity: 0.9;
  margin: var(--s1) 0 0;
  font-size: 17px;
  line-height: 1.6;
  max-width: var(--measure);
}

/* The one aside on the page: indented off the margin, not boxed */
.bb-international-callout {
  padding: 0 0 0 var(--s3);
  border-left: 2px solid var(--bb-border);
  margin: var(--s5) 0;
  max-width: var(--measure);
}
.bb-international-callout .bb-intl-header {
  font-family: 'Instrument Sans', sans-serif;
  font-size: 11px;
  font-weight: 600;
  text-transform: uppercase;
  letter-spacing: 0.16em;
  color: var(--bb-green-accent);
  margin: 0 0 var(--s1);
}
.bb-international-callout p {
  font-family: 'Instrument Sans', sans-serif;
  font-size: 17px;
  font-style: italic;
  color: var(--bb-text-secondary);
  opacity: 0.9;
  line-height: 1.6;
  margin: 0;
}

/* Desktop */
@media (min-width: 769px) {
  .bb-two-col { grid-template-columns: 3fr 2fr; gap: var(--s5); }
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
  <span class="bb-num">01</span>
  <div class="bb-divider-label">Real-World Examples</div>
</div>

## Real-World Examples

<p class="bb-section-hint">Click each row (or tap on mobile) to see more.</p>

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
  <span class="bb-num">02</span>
  <div class="bb-divider-label">Beyond the Lab</div>
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
  <span class="bb-num">03</span>
  <div class="bb-divider-label">Common Misconceptions</div>
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
