---
layout: single
title: "What is Biotech?"
permalink: /what-is-biotech/
toc: true
toc_label: "On This Page"
---

<style>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=Playfair+Display:wght@600;700&display=swap');
body { font-family: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif; }
h1, h2, h3 { font-family: 'Playfair Display', Georgia, serif; }

:root {
  --bb-green: #2D5F3F;
  --bb-green-accent: #3A7D5C;
  --bb-green-bright: #4CAF50;
  --bb-green-hover: #66BB6A;
  --bb-green-dark: #1A3A28;
  --bb-green-bg: #E8F5E9;
  --bb-green-bg-subtle: #F1F8F4;
  --bb-navy: #1A1A2E;
  --bb-charcoal: #2C3E50;
  --bb-white: #ffffff;
  --bb-off-white: #FAFAFA;
  --bb-text-secondary: #475569;
  --bb-gray: #757575;
  --bb-border: #e2e8f0;
}

/* Page Header */
.bb-page-hero {
  background: linear-gradient(160deg, var(--bb-navy) 0%, var(--bb-green-dark) 100%);
  color: var(--bb-white);
  padding: 2rem 2rem;
  border-radius: 8px;
  margin-bottom: 2rem;
  position: relative;
  overflow: hidden;
}
.bb-page-hero::before {
  content: '';
  position: absolute;
  top: 0; left: 0; width: 100%; height: 100%;
  background: radial-gradient(ellipse at 80% 20%, rgba(45,95,63,0.15) 0%, transparent 60%);
  pointer-events: none;
}
.bb-page-hero h1 {
  font-size: 1.4rem;
  font-weight: 700;
  margin: 0 0 0.4rem;
  color: var(--bb-white);
  letter-spacing: -0.02em;
  position: relative;
}
.bb-page-hero p {
  font-family: 'Inter', sans-serif;
  font-size: 0.88rem;
  color: rgba(255,255,255,0.8);
  margin: 0;
  font-weight: 300;
  line-height: 1.6;
  position: relative;
}

/* Image Placeholder */
.bb-img-placeholder {
  background: linear-gradient(135deg, var(--bb-green-bg), #e8f4f5);
  border: 1px dashed var(--bb-border);
  border-radius: 8px;
  padding: 1.5rem 1rem;
  text-align: center;
  color: var(--bb-gray);
  font-family: 'Inter', sans-serif;
  font-size: 0.75rem;
  font-weight: 500;
  line-height: 1.5;
}

/* Reduced callout box */
.bb-callout {
  background: var(--bb-navy);
  border-radius: 8px;
  padding: 1rem 1.25rem;
  margin: 1.5rem 0;
  position: relative;
  overflow: hidden;
  display: inline-block;
  width: 100%;
}
.bb-callout::before {
  content: '';
  position: absolute;
  top: 0; left: 0;
  width: 3px; height: 100%;
  background: linear-gradient(180deg, var(--bb-green-bright), var(--bb-green-accent));
}
.bb-callout p {
  font-family: 'Inter', sans-serif;
  font-size: 0.95rem;
  font-weight: 600;
  color: var(--bb-white);
  margin: 0;
  line-height: 1.5;
  letter-spacing: -0.01em;
  padding-left: 0.75rem;
}
.bb-callout span {
  display: block;
  font-family: 'Inter', sans-serif;
  font-size: 0.68rem;
  font-weight: 400;
  color: rgba(255,255,255,0.5);
  margin-top: 0.35rem;
  letter-spacing: 0.04em;
  text-transform: uppercase;
  padding-left: 0.75rem;
}

/* Section intro text */
.bb-intro-text {
  font-family: 'Inter', sans-serif;
  font-size: 0.9rem;
  color: #334155;
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
  font-family: 'Inter', sans-serif;
  font-size: 0.67rem;
  font-weight: 700;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  color: var(--bb-green-accent);
  white-space: nowrap;
}

/* ============================================
   FLIP CARDS — Real-World Examples
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

.bb-flip-card.flipped .bb-flip-card-inner,
.bb-flip-card:hover .bb-flip-card-inner {
  transform: rotateY(180deg);
}

.bb-flip-front,
.bb-flip-back {
  position: absolute;
  width: 100%;
  height: 100%;
  backface-visibility: hidden;
  -webkit-backface-visibility: hidden;
  border-radius: 8px;
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
  background: linear-gradient(135deg, #d1e8d8, #e8f4ea);
  height: 110px;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-shrink: 0;
  border-bottom: 1px solid var(--bb-border);
}
.bb-flip-front-img span {
  font-family: 'Inter', sans-serif;
  font-size: 0.68rem;
  font-weight: 500;
  color: var(--bb-green);
  background: rgba(45,95,63,0.1);
  border: 1px dashed rgba(45,95,63,0.3);
  border-radius: 4px;
  padding: 0.25rem 0.6rem;
}
.bb-flip-front-body {
  padding: 0.85rem 1rem;
  flex: 1;
}
.bb-flip-front-body h3 {
  font-family: 'Inter', sans-serif;
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
  font-family: 'Inter', sans-serif;
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
  font-family: 'Inter', sans-serif;
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
  background: rgba(14,116,144,0.18);
  border: 1px solid rgba(14,116,144,0.38);
  border-radius: 20px;
  padding: 0.18rem 0.6rem;
  font-family: 'Inter', sans-serif;
  font-size: 0.875rem;
  font-weight: 500;
  color: #7ECFE0;
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
  font-family: 'Inter', sans-serif;
  color: #334155;
  font-size: 0.9rem;
  line-height: 1.8;
  margin: 0 0 0.85rem;
}
.bb-two-col-text p:last-child { margin-bottom: 0; }

/* Misconception Blocks */
.bb-misconception {
  background: var(--bb-off-white);
  border: 1px solid var(--bb-border);
  border-left: 3px solid var(--bb-green-accent);
  border-radius: 7px;
  padding: 1rem 1.25rem;
  margin-bottom: 0.75rem;
}
.bb-misconception strong {
  color: var(--bb-navy);
  font-family: 'Inter', sans-serif;
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
  border-radius: 8px;
  display: block;
}

/* Desktop */
@media (min-width: 769px) {
  .bb-page-hero { padding: 2.5rem 2.5rem; border-radius: 10px; }
  .bb-page-hero h1 { font-size: 1.65rem; }
  .bb-page-hero p { font-size: 0.93rem; }
  .bb-flip-grid { grid-template-columns: repeat(2, 1fr); gap: 1.1rem; }
  .bb-flip-card { height: 240px; }
  .bb-flip-front-img { height: 120px; }
  .bb-two-col { grid-template-columns: 3fr 2fr; gap: 2.25rem; }
  .bb-callout p { font-size: 1rem; }
}
@media (min-width: 1024px) {
  .bb-flip-grid { grid-template-columns: repeat(4, 1fr); }
}

/* ============================================
   KEY TERMS ACCORDION
   ============================================ */
.bb-terms-section {
  margin-top: 2.5rem;
}
.bb-terms-intro {
  font-family: 'Inter', sans-serif;
  font-size: 0.88rem;
  color: var(--bb-text-secondary);
  line-height: 1.7;
  margin-bottom: 1.5rem;
}
.bb-terms-letter-group {
  margin-bottom: 0.25rem;
}
.bb-terms-letter-header {
  font-family: 'Playfair Display', Georgia, serif;
  font-size: 0.92rem;
  font-weight: 700;
  color: var(--bb-green);
  letter-spacing: 0.06em;
  text-transform: uppercase;
  margin: 1.1rem 0 0.35rem;
  padding-bottom: 0.3rem;
  border-bottom: 1px solid var(--bb-border);
}
.bb-accordion-item {
  border: 1px solid var(--bb-border);
  border-radius: 6px;
  margin-bottom: 0.4rem;
  overflow: hidden;
}
.bb-accordion-trigger {
  width: 100%;
  background: none;
  border: none;
  padding: 0.75rem 1rem;
  text-align: left;
  display: flex;
  align-items: center;
  justify-content: space-between;
  cursor: pointer;
  font-family: 'Inter', sans-serif;
  font-size: 0.88rem;
  font-weight: 600;
  color: var(--bb-green);
  transition: background 0.18s ease;
  gap: 0.5rem;
}
.bb-accordion-trigger:hover {
  background: var(--bb-green-bg-subtle);
}
.bb-accordion-trigger .bb-acc-chevron {
  flex-shrink: 0;
  width: 16px;
  height: 16px;
  border-right: 2px solid var(--bb-green);
  border-bottom: 2px solid var(--bb-green);
  transform: rotate(45deg);
  transition: transform 0.25s ease;
  margin-top: -3px;
}
.bb-accordion-item.open .bb-acc-chevron {
  transform: rotate(-135deg);
  margin-top: 3px;
}
.bb-accordion-body {
  max-height: 0;
  overflow: hidden;
  transition: max-height 0.3s ease;
  background: #FAFAF8;
}
.bb-accordion-body-inner {
  padding: 0.75rem 1rem 0.85rem;
  font-family: 'Inter', sans-serif;
  font-size: 0.84rem;
  color: var(--bb-text-secondary);
  line-height: 1.75;
}
.bb-terms-footer-note {
  font-family: 'Inter', sans-serif;
  font-size: 0.78rem;
  font-style: italic;
  color: var(--bb-gray);
  margin-top: 1.25rem;
  padding-top: 1rem;
  border-top: 1px solid var(--bb-border);
}

/* International callout (shared style) */
.bb-international-callout {
  background: #FAF7F2;
  border: 1px solid #e8dfd0;
  border-left: 4px solid var(--bb-green-accent);
  border-radius: 7px;
  padding: 1rem 1.25rem;
  margin: 1.75rem 0;
}
.bb-international-callout .bb-intl-header {
  font-family: 'Inter', sans-serif;
  font-size: 0.82rem;
  font-weight: 700;
  color: var(--bb-green);
  margin: 0 0 0.4rem;
  display: flex;
  align-items: center;
  gap: 0.4rem;
}
.bb-international-callout p {
  font-family: 'Inter', sans-serif;
  font-size: 0.82rem;
  font-style: italic;
  color: var(--bb-text-secondary);
  line-height: 1.7;
  margin: 0;
}
</style>

<div class="bb-page-hero">
  <h1>What is Biotechnology, Really?</h1>
  <p>Understanding the science shaping our future, in plain language, no prerequisites required.</p>
</div>

<p class="bb-intro-text">Biotechnology is using living systems (cells, bacteria, proteins, DNA) to create useful products or solve real problems.</p>

<div class="bb-callout">
  <p>Biotech = biology + technology to solve real problems.</p>
  <span>The simplest definition that actually holds up</span>
</div>

<p class="bb-intro-text">It sounds vague because biotech is <strong>incredibly broad</strong>. It touches medicine, agriculture, environmental science, manufacturing, and more. The best way to understand it is through examples.</p>

<div class="bb-divider">
  <div class="bb-divider-line"></div>
  <div class="bb-divider-label">Real-World Examples</div>
  <div class="bb-divider-line"></div>
</div>

## Real-World Examples

<p class="bb-intro-text" style="font-size:0.82rem; color: var(--bb-gray);">Hover over each card (or tap on mobile) to see more.</p>

<div class="bb-flip-grid">

  <div class="bb-flip-card" role="button" tabindex="0" aria-label="Medicine example: click to flip">
    <div class="bb-flip-card-inner">
      <div class="bb-flip-front">
        <div class="bb-flip-front-img"><img src="/assets/images/biotech-medicine.jpg" alt="Medicine"></div>
        <div class="bb-flip-front-body">
          <h3>Medicine</h3>
          <p class="bb-flip-hint">Hover to learn more</p>
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
          <p class="bb-flip-hint">Hover to learn more</p>
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
          <p class="bb-flip-hint">Hover to learn more</p>
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
          <p class="bb-flip-hint">Hover to learn more</p>
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
  <div class="bb-divider-label">Beyond the Lab</div>
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
  <div class="bb-divider-label">Common Misconceptions</div>
  <div class="bb-divider-line"></div>
</div>

## Common Misconceptions

<div class="bb-misconception">
  <strong>"You need to be good at biology to work in the industry."</strong>
  <p>Not necessarily. Biotech employs humanities majors, business students, and engineers just as readily as biology PhDs. Science communication, operations, and regulatory affairs are all viable without a lab background.</p>
</div>

<div class="bb-misconception">
  <strong>"It's all lab work."</strong>
  <p>Lab work is one slice of a much bigger picture. There's also manufacturing, regulatory affairs, sales, policy, data analysis, and more. The <a href="/career-pathways/" style="color: #3A7D5C; font-weight: 600;">Career Pathways</a> page shows the full range.</p>
</div>

<div class="bb-misconception">
  <strong>"You need a PhD."</strong>
  <p>Only if you want to lead independent research. Most biotech jobs in regulatory, manufacturing, business, and operations require a bachelor's degree or less. Certificate programs can get you there in months, and there are entry points at every level.</p>
</div>

<!-- Regulatory context callout -->
<div class="bb-international-callout">
  <div class="bb-intl-header">🌍 Outside the US?</div>
  <p>Regulatory terminology varies by country. FDA = United States Food and Drug Administration. EMA = European Medicines Agency (EU). Health Canada oversees drug approvals in Canada. PMDA (Pharmaceuticals and Medical Devices Agency) regulates in Japan. When you see terms like "IND filing" or "NDA" below, those are US-specific — equivalent processes exist in other jurisdictions under different names and timelines.</p>
</div>

<div class="bb-divider">
  <div class="bb-divider-line"></div>
  <div class="bb-divider-label">Vocabulary Reference</div>
  <div class="bb-divider-line"></div>
</div>

## Key Terms

<div class="bb-terms-section">
<p class="bb-terms-intro">New to the vocabulary? Here's a quick reference. Click any term to expand its definition.</p>

<!-- A -->
<div class="bb-terms-letter-group">
<div class="bb-terms-letter-header">A</div>

<div class="bb-accordion-item">
<button class="bb-accordion-trigger" aria-expanded="false">Antibody <span class="bb-acc-chevron"></span></button>
<div class="bb-accordion-body"><div class="bb-accordion-body-inner">A protein produced by the immune system (or engineered in a lab) that binds specifically to a target molecule called an antigen. Therapeutic antibodies — including monoclonal antibodies — are among the most important drug classes in modern biotech, used to treat cancers, autoimmune diseases, and infectious diseases.</div></div>
</div>

<div class="bb-accordion-item">
<button class="bb-accordion-trigger" aria-expanded="false">Assay <span class="bb-acc-chevron"></span></button>
<div class="bb-accordion-body"><div class="bb-accordion-body-inner">A laboratory test or procedure used to measure the presence, activity, or quantity of a substance — such as a protein, cell, or drug compound. Common types include ELISA assays, cell viability assays, and binding assays. Assay development is a foundational skill in both research and clinical settings.</div></div>
</div>

</div>

<!-- B -->
<div class="bb-terms-letter-group">
<div class="bb-terms-letter-header">B</div>

<div class="bb-accordion-item">
<button class="bb-accordion-trigger" aria-expanded="false">Bioinformatics <span class="bb-acc-chevron"></span></button>
<div class="bb-accordion-body"><div class="bb-accordion-body-inner">The use of computational tools, algorithms, and statistical methods to analyze and interpret biological data — particularly large datasets from genomics, proteomics, and structural biology. Bioinformaticians write code (often Python or R) to process sequencing data, identify gene variants, and model protein structures.</div></div>
</div>

<div class="bb-accordion-item">
<button class="bb-accordion-trigger" aria-expanded="false">Biologics <span class="bb-acc-chevron"></span></button>
<div class="bb-accordion-body"><div class="bb-accordion-body-inner">Drugs derived from biological sources — living cells, proteins, or nucleic acids — rather than synthesized through chemical reactions. Examples include monoclonal antibodies, vaccines, and gene therapies. Biologics are typically more complex to manufacture than small molecule drugs and require specialized regulatory pathways (e.g., BLA in the US rather than NDA).</div></div>
</div>

<div class="bb-accordion-item">
<button class="bb-accordion-trigger" aria-expanded="false">BLA (Biologics License Application) <span class="bb-acc-chevron"></span></button>
<div class="bb-accordion-body"><div class="bb-accordion-body-inner">The application submitted to the FDA to request approval to market a biologic drug product in the United States. Unlike an NDA (used for small molecule drugs), a BLA is required for biologics such as therapeutic proteins and monoclonal antibodies. The FDA reviews safety, efficacy, and manufacturing data before granting approval.</div></div>
</div>

</div>

<!-- C -->
<div class="bb-terms-letter-group">
<div class="bb-terms-letter-header">C</div>

<div class="bb-accordion-item">
<button class="bb-accordion-trigger" aria-expanded="false">CDMO (Contract Development and Manufacturing Organization) <span class="bb-acc-chevron"></span></button>
<div class="bb-accordion-body"><div class="bb-accordion-body-inner">A company that provides development and manufacturing services to biotech and pharma companies on a contract basis, handling both process development and large-scale production. CDMOs like Lonza, Catalent, and Samsung Biologics are critical partners for companies that don't have their own manufacturing infrastructure.</div></div>
</div>

<div class="bb-accordion-item">
<button class="bb-accordion-trigger" aria-expanded="false">Cell Line <span class="bb-acc-chevron"></span></button>
<div class="bb-accordion-body"><div class="bb-accordion-body-inner">A population of cells that can be grown indefinitely in a laboratory because they've been derived from a tumor or genetically modified to divide continuously. Cell lines like HeLa (derived from Henrietta Lacks) and CHO (Chinese hamster ovary) cells are used extensively in research and to produce therapeutic proteins at scale.</div></div>
</div>

<div class="bb-accordion-item">
<button class="bb-accordion-trigger" aria-expanded="false">Clinical Trial (Phase I / II / III) <span class="bb-acc-chevron"></span></button>
<div class="bb-accordion-body"><div class="bb-accordion-body-inner">The staged process of testing a new drug or therapy in humans. <strong>Phase I</strong> tests safety and dosing in a small group (typically 20–80 healthy volunteers or patients). <strong>Phase II</strong> expands to a larger group to evaluate efficacy and further assess safety. <strong>Phase III</strong> involves thousands of patients in a randomized, controlled study to confirm efficacy, monitor side effects, and compare to existing treatments. Successful Phase III trials lead to an NDA or BLA submission.</div></div>
</div>

<div class="bb-accordion-item">
<button class="bb-accordion-trigger" aria-expanded="false">CMO (Contract Manufacturing Organization) <span class="bb-acc-chevron"></span></button>
<div class="bb-accordion-body"><div class="bb-accordion-body-inner">A company that manufactures drug products or active pharmaceutical ingredients (APIs) on a contract basis. CMOs specialize in scaling up production for clinical trials or commercial supply without requiring the hiring company to build its own manufacturing plant. Many CDMOs now offer both development and manufacturing services.</div></div>
</div>

<div class="bb-accordion-item">
<button class="bb-accordion-trigger" aria-expanded="false">CRO (Contract Research Organization) <span class="bb-acc-chevron"></span></button>
<div class="bb-accordion-body"><div class="bb-accordion-body-inner">A company that provides research and clinical trial management services to the pharmaceutical, biotech, and medical device industries. CROs can handle everything from preclinical studies and regulatory submissions to patient recruitment and data management. Major CROs include IQVIA, Covance, and Medpace.</div></div>
</div>

<div class="bb-accordion-item">
<button class="bb-accordion-trigger" aria-expanded="false">CRISPR <span class="bb-acc-chevron"></span></button>
<div class="bb-accordion-body"><div class="bb-accordion-body-inner">Clustered Regularly Interspaced Short Palindromic Repeats — a natural bacterial immune system repurposed as a precise gene-editing tool. CRISPR-Cas9 allows scientists to cut DNA at specific sequences, enabling gene deletion, correction, or insertion. It's used in research, drug development, and increasingly in approved therapies for genetic diseases like sickle cell disease.</div></div>
</div>

</div>

<!-- D -->
<div class="bb-terms-letter-group">
<div class="bb-terms-letter-header">D</div>

<div class="bb-accordion-item">
<button class="bb-accordion-trigger" aria-expanded="false">Dry Lab <span class="bb-acc-chevron"></span></button>
<div class="bb-accordion-body"><div class="bb-accordion-body-inner">A laboratory or research environment where work is computational rather than experimental — analyzing data, building models, writing code, or running simulations. Dry lab scientists work alongside wet lab scientists and typically use tools like Python, R, MATLAB, or specialized bioinformatics platforms. The distinction is increasingly blurred as computational methods become integral to all areas of biology.</div></div>
</div>

</div>

<!-- E -->
<div class="bb-terms-letter-group">
<div class="bb-terms-letter-header">E</div>

<div class="bb-accordion-item">
<button class="bb-accordion-trigger" aria-expanded="false">ELISA (Enzyme-Linked Immunosorbent Assay) <span class="bb-acc-chevron"></span></button>
<div class="bb-accordion-body"><div class="bb-accordion-body-inner">A plate-based assay technique used to detect and quantify proteins, antibodies, or hormones in a sample. ELISA uses antibodies conjugated to enzymes that produce a measurable signal when the target molecule is present. It's one of the most widely used assays in biotech research, diagnostics, and quality control.</div></div>
</div>

</div>

<!-- F -->
<div class="bb-terms-letter-group">
<div class="bb-terms-letter-header">F</div>

<div class="bb-accordion-item">
<button class="bb-accordion-trigger" aria-expanded="false">Flow Cytometry <span class="bb-acc-chevron"></span></button>
<div class="bb-accordion-body"><div class="bb-accordion-body-inner">A technology that analyzes thousands of cells per second by passing them through a laser beam and measuring light scatter and fluorescence. Used to characterize cell populations, measure protein expression, and sort cells for downstream experiments. Widely used in immunology, oncology, and drug development.</div></div>
</div>

</div>

<!-- G -->
<div class="bb-terms-letter-group">
<div class="bb-terms-letter-header">G</div>

<div class="bb-accordion-item">
<button class="bb-accordion-trigger" aria-expanded="false">GLP (Good Laboratory Practice) <span class="bb-acc-chevron"></span></button>
<div class="bb-accordion-body"><div class="bb-accordion-body-inner">A regulatory framework that governs preclinical laboratory studies intended to support drug applications. GLP compliance ensures that study data is reliable, reproducible, and properly documented — essential for FDA acceptance of safety data. GLP studies are distinct from general research and require formal documentation, validation, and auditing.</div></div>
</div>

<div class="bb-accordion-item">
<button class="bb-accordion-trigger" aria-expanded="false">GMP (Good Manufacturing Practice) <span class="bb-acc-chevron"></span></button>
<div class="bb-accordion-body"><div class="bb-accordion-body-inner">Regulations enforced by the FDA (and equivalent global agencies) that govern the manufacturing, testing, and quality control of pharmaceutical and biologic products. GMP compliance ensures that drugs are consistently produced to quality standards appropriate for human use. Working in a GMP facility involves strict documentation, environmental monitoring, and deviation reporting.</div></div>
</div>

</div>

<!-- I -->
<div class="bb-terms-letter-group">
<div class="bb-terms-letter-header">I</div>

<div class="bb-accordion-item">
<button class="bb-accordion-trigger" aria-expanded="false">IND (Investigational New Drug) <span class="bb-acc-chevron"></span></button>
<div class="bb-accordion-body"><div class="bb-accordion-body-inner">An application submitted to the FDA before a new drug can be tested in humans. The IND includes preclinical data, manufacturing information, and a proposed clinical trial protocol. If the FDA does not place a clinical hold within 30 days, the company can proceed with human trials. Filing an IND is a major milestone in drug development.</div></div>
</div>

<div class="bb-accordion-item">
<button class="bb-accordion-trigger" aria-expanded="false">IPO (Initial Public Offering) <span class="bb-acc-chevron"></span></button>
<div class="bb-accordion-body"><div class="bb-accordion-body-inner">The process by which a private company offers shares to the public for the first time on a stock exchange, raising capital from public investors. In biotech, IPOs are a common way for companies that haven't yet generated revenue to fund late-stage clinical trials. The timing of biotech IPOs is highly sensitive to market conditions and clinical data readouts.</div></div>
</div>

</div>

<!-- N -->
<div class="bb-terms-letter-group">
<div class="bb-terms-letter-header">N</div>

<div class="bb-accordion-item">
<button class="bb-accordion-trigger" aria-expanded="false">NDA (New Drug Application) <span class="bb-acc-chevron"></span></button>
<div class="bb-accordion-body"><div class="bb-accordion-body-inner">The formal application submitted to the FDA requesting approval to market a new small molecule drug in the United States. An NDA includes all preclinical and clinical data, proposed labeling, and manufacturing information. The FDA has a standard review period of 10–12 months, with a priority review pathway (6 months) available for certain drugs.</div></div>
</div>

</div>

<!-- P -->
<div class="bb-terms-letter-group">
<div class="bb-terms-letter-header">P</div>

<div class="bb-accordion-item">
<button class="bb-accordion-trigger" aria-expanded="false">PCR (Polymerase Chain Reaction) <span class="bb-acc-chevron"></span></button>
<div class="bb-accordion-body"><div class="bb-accordion-body-inner">A technique that amplifies small amounts of DNA into millions of copies, making it detectable and analyzable. PCR is foundational to molecular biology and is used in diagnostics (including COVID-19 testing), genetic research, forensics, and manufacturing quality control. It works by cycling the sample through different temperatures to denature, anneal, and extend the DNA strands.</div></div>
</div>

<div class="bb-accordion-item">
<button class="bb-accordion-trigger" aria-expanded="false">Pharmacodynamics (PD) <span class="bb-acc-chevron"></span></button>
<div class="bb-accordion-body"><div class="bb-accordion-body-inner">The study of how a drug affects the body — including its mechanism of action, biochemical and physiological effects, and dose-response relationships. Pharmacodynamics answers the question: what does the drug do to the body? It's studied alongside pharmacokinetics throughout drug development to understand both how a drug behaves and how it exerts its therapeutic effect.</div></div>
</div>

<div class="bb-accordion-item">
<button class="bb-accordion-trigger" aria-expanded="false">Pharmacokinetics (PK) <span class="bb-acc-chevron"></span></button>
<div class="bb-accordion-body"><div class="bb-accordion-body-inner">The study of how the body absorbs, distributes, metabolizes, and eliminates a drug — often summarized as ADME. Pharmacokinetics answers: what does the body do to the drug? PK data is critical for determining appropriate dosing regimens, predicting drug-drug interactions, and understanding why a drug may fail in clinical trials despite promising preclinical results.</div></div>
</div>

<div class="bb-accordion-item">
<button class="bb-accordion-trigger" aria-expanded="false">Plasmid <span class="bb-acc-chevron"></span></button>
<div class="bb-accordion-body"><div class="bb-accordion-body-inner">A small, circular DNA molecule that exists separately from the chromosomal DNA in bacteria and some other organisms. Plasmids are widely used in molecular biology as vectors to introduce genes into cells. They're essential tools in cloning, gene expression studies, and the production of recombinant proteins like insulin.</div></div>
</div>

<div class="bb-accordion-item">
<button class="bb-accordion-trigger" aria-expanded="false">Postdoc (Postdoctoral Researcher) <span class="bb-acc-chevron"></span></button>
<div class="bb-accordion-body"><div class="bb-accordion-body-inner">A temporary research position held after completing a PhD, typically lasting 2–5 years. Postdocs work in academic labs or research institutes to develop independent research programs, build publication records, and acquire skills needed for faculty or senior industry positions. Postdoc salaries are generally low relative to industry roles requiring equivalent expertise.</div></div>
</div>

<div class="bb-accordion-item">
<button class="bb-accordion-trigger" aria-expanded="false">Preclinical (Studies) <span class="bb-acc-chevron"></span></button>
<div class="bb-accordion-body"><div class="bb-accordion-body-inner">Research conducted before a drug is tested in humans — typically in cell cultures (in vitro) and animal models (in vivo). Preclinical studies evaluate whether a drug candidate is safe enough and has biological activity that justifies human trials. Successful preclinical data supports an IND filing with the FDA.</div></div>
</div>

<div class="bb-accordion-item">
<button class="bb-accordion-trigger" aria-expanded="false">Principal Investigator (PI) <span class="bb-acc-chevron"></span></button>
<div class="bb-accordion-body"><div class="bb-accordion-body-inner">The lead scientist responsible for the design, conduct, and reporting of a research project. In academic settings, the PI is typically a faculty member who runs a lab and secures grant funding. In clinical trials, the PI is the physician or researcher at each site who oversees patient enrollment and protocol compliance. Becoming a PI is the traditional goal of an academic research career.</div></div>
</div>

</div>

<!-- Q -->
<div class="bb-terms-letter-group">
<div class="bb-terms-letter-header">Q</div>

<div class="bb-accordion-item">
<button class="bb-accordion-trigger" aria-expanded="false">qPCR (Quantitative PCR) <span class="bb-acc-chevron"></span></button>
<div class="bb-accordion-body"><div class="bb-accordion-body-inner">A variation of PCR that measures the quantity of DNA or RNA in a sample in real time, using fluorescent dyes or probes. qPCR is used to measure gene expression levels, detect pathogens, and quantify viral loads. It's one of the most commonly used techniques in biotech research and diagnostics, valued for its sensitivity and reproducibility.</div></div>
</div>

</div>

<!-- R -->
<div class="bb-terms-letter-group">
<div class="bb-terms-letter-header">R</div>

<div class="bb-accordion-item">
<button class="bb-accordion-trigger" aria-expanded="false">Regulatory Affairs <span class="bb-acc-chevron"></span></button>
<div class="bb-accordion-body"><div class="bb-accordion-body-inner">The function within a biotech or pharma company responsible for managing interactions with regulatory agencies (FDA, EMA, etc.), preparing and submitting regulatory documents, and ensuring that products are developed and marketed in compliance with applicable laws. Regulatory affairs professionals bridge science, law, and strategy — a career path accessible without a PhD.</div></div>
</div>

</div>

<!-- S -->
<div class="bb-terms-letter-group">
<div class="bb-terms-letter-header">S</div>

<div class="bb-accordion-item">
<button class="bb-accordion-trigger" aria-expanded="false">Sequencing (DNA/RNA) <span class="bb-acc-chevron"></span></button>
<div class="bb-accordion-body"><div class="bb-accordion-body-inner">The process of determining the exact order of nucleotides (A, T, C, G) in a DNA or RNA molecule. Next-generation sequencing (NGS) technologies can sequence entire genomes in hours at a fraction of the cost of earlier methods. Sequencing is foundational to genomics research, cancer diagnostics, infectious disease monitoring, and personalized medicine.</div></div>
</div>

<div class="bb-accordion-item">
<button class="bb-accordion-trigger" aria-expanded="false">Series A / B / C Funding <span class="bb-acc-chevron"></span></button>
<div class="bb-accordion-body"><div class="bb-accordion-body-inner">Rounds of venture capital investment at successive stages of a company's development. <strong>Series A</strong> typically funds early product development or clinical proof-of-concept studies. <strong>Series B</strong> supports scale-up and larger clinical trials. <strong>Series C</strong> (and beyond) funds commercial preparation or expansion. Each round dilutes existing shareholders but provides capital to reach the next value-creating milestone.</div></div>
</div>

<div class="bb-accordion-item">
<button class="bb-accordion-trigger" aria-expanded="false">Small Molecule <span class="bb-acc-chevron"></span></button>
<div class="bb-accordion-body"><div class="bb-accordion-body-inner">A low-molecular-weight compound — typically a chemical drug — that can enter cells and interact with biological targets. Small molecules include most traditional pharmaceuticals (aspirin, statins, antibiotics) and are synthesized through chemical processes rather than biological ones. They're generally cheaper to manufacture than biologics but face different challenges in terms of specificity and off-target effects.</div></div>
</div>

</div>

<!-- T -->
<div class="bb-terms-letter-group">
<div class="bb-terms-letter-header">T</div>

<div class="bb-accordion-item">
<button class="bb-accordion-trigger" aria-expanded="false">Tech Transfer <span class="bb-acc-chevron"></span></button>
<div class="bb-accordion-body"><div class="bb-accordion-body-inner">The process of transferring scientific discoveries or technologies from research institutions (universities, national labs) to the private sector for commercial development. Tech transfer offices at universities manage intellectual property, negotiate licenses, and support the formation of spinout companies. Many successful biotech companies were founded on technologies licensed from academic labs.</div></div>
</div>

<div class="bb-accordion-item">
<button class="bb-accordion-trigger" aria-expanded="false">Transfection <span class="bb-acc-chevron"></span></button>
<div class="bb-accordion-body"><div class="bb-accordion-body-inner">The process of introducing foreign DNA or RNA into eukaryotic cells (cells with a nucleus, like human or animal cells). Transfection can be transient (temporary expression) or stable (permanent integration into the genome). Common methods include lipofection (using lipid nanoparticles), electroporation (using electric pulses), and viral vectors. It's a fundamental technique in cell biology and gene therapy development.</div></div>
</div>

</div>

<!-- W -->
<div class="bb-terms-letter-group">
<div class="bb-terms-letter-header">W</div>

<div class="bb-accordion-item">
<button class="bb-accordion-trigger" aria-expanded="false">Wet Lab <span class="bb-acc-chevron"></span></button>
<div class="bb-accordion-body"><div class="bb-accordion-body-inner">A laboratory where researchers work with biological samples, chemicals, and physical materials — involving actual hands-on experiments like cell culture, PCR, western blots, and assays. Called "wet" because experiments typically involve liquids and reagents. Wet lab skills are valued in research, manufacturing, and quality control roles, and are distinct from the computational ("dry lab") side of modern biology.</div></div>
</div>

</div>

<p class="bb-terms-footer-note">Definitions are written for a US biotech context unless otherwise noted.</p>

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

<script>
// Key Terms Accordion
(function() {
  var items = document.querySelectorAll('.bb-accordion-item');
  items.forEach(function(item) {
    var trigger = item.querySelector('.bb-accordion-trigger');
    var body = item.querySelector('.bb-accordion-body');
    if (!trigger || !body) return;
    trigger.addEventListener('click', function() {
      var isOpen = item.classList.contains('open');
      // Close all
      items.forEach(function(other) {
        other.classList.remove('open');
        var otherTrigger = other.querySelector('.bb-accordion-trigger');
        var otherBody = other.querySelector('.bb-accordion-body');
        if (otherTrigger) otherTrigger.setAttribute('aria-expanded', 'false');
        if (otherBody) otherBody.style.maxHeight = '0';
      });
      // Toggle current
      if (!isOpen) {
        item.classList.add('open');
        trigger.setAttribute('aria-expanded', 'true');
        body.style.maxHeight = body.scrollHeight + 'px';
      }
    });
  });
})();
</script>
