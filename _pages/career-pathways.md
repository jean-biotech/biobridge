---
layout: single
title: "Career Pathways"
permalink: /career-pathways/
---

<style>
@import url('https://fonts.googleapis.com/css2?family=Fraunces:ital,opsz,wght@0,9..144,400..600;1,9..144,400..600&family=Instrument+Sans:wght@400;500;600;700&display=swap');
body { font-family: 'Instrument Sans', -apple-system, BlinkMacSystemFont, sans-serif; }
h1, h2, h3, h4 { font-family: 'Fraunces', Georgia, serif; }

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
  --bb-border: rgba(36,34,26,0.12);
  --bb-teal: #8E9469;
}

/* ============================================
   PATHWAY ROWS: no cards, no carousel. Every
   pathway stacks vertically, separated by a
   1px hairline rule, all visible at once.
   ============================================ */
.bb-path-list {
  border-top: 1px solid var(--bb-border);
  margin-bottom: 1rem;
}
.bb-path-row {
  padding: 2.5rem 0;
  border-bottom: 1px solid var(--bb-border);
}
.bb-path-row__head {
  display: flex;
  align-items: baseline;
  gap: 1rem;
  margin-bottom: 1.1rem;
}
.bb-path-row__num {
  font-family: 'Instrument Sans', sans-serif;
  font-size: 11px;
  font-weight: 600;
  letter-spacing: 0.1em;
  color: var(--bb-gray);
}
.bb-path-row__title {
  font-family: 'Fraunces', Georgia, serif;
  color: var(--bb-navy);
  font-size: 30px;
  font-weight: 500;
  margin: 0;
  letter-spacing: -0.01em;
}
.bb-path-fields {
  display: grid;
  grid-template-columns: 1fr;
  gap: 1.1rem;
  max-width: 62ch;
}
.bb-detail-label {
  font-family: 'Instrument Sans', sans-serif;
  color: var(--bb-green-accent);
  font-size: 11px;
  text-transform: uppercase;
  letter-spacing: 0.16em;
  font-weight: 600;
  margin-bottom: 0.3rem;
}
.bb-detail-value {
  color: var(--bb-charcoal);
  opacity: 0.82;
  font-size: 17px;
  line-height: 1.65;
  margin: 0;
}
.bb-detail-value ul {
  margin: 0;
  padding-left: 1.1rem;
}
.bb-detail-value li {
  margin-bottom: 0.25rem;
  font-size: 17px;
}
.bb-companies-label {
  font-family: 'Instrument Sans', sans-serif;
  color: var(--bb-gray);
  font-size: 11px;
  text-transform: uppercase;
  letter-spacing: 0.16em;
  font-weight: 600;
  margin-bottom: 0.4rem;
}
.bb-org-list {
  color: var(--bb-charcoal);
  opacity: 0.82;
  font-size: 17px;
  line-height: 1.65;
}

@media (min-width: 769px) {
  .bb-path-row__title { font-size: 30px; }
}

/* ============================================
   NEXT STEPS
   ============================================ */
.bb-next-steps {
  border-top: 1px solid var(--bb-border);
  border-bottom: 1px solid var(--bb-border);
  padding: 1.5rem 0;
  margin-top: 0.5rem;
}
.bb-next-steps h2 {
  font-family: 'Instrument Sans', sans-serif;
  color: var(--bb-navy);
  font-size: 17px;
  font-weight: 700;
  margin-top: 0;
  margin-bottom: 0.75rem;
}
.bb-next-steps ul {
  padding-left: 1.1rem;
  margin: 0;
}
.bb-next-steps li {
  margin-bottom: 0.4rem;
  color: var(--bb-text-secondary);
  opacity: 0.82;
  font-size: 17px;
}
.bb-next-steps a {
  color: var(--bb-green-accent);
  font-weight: 600;
}

/* ============================================
   CREAM SECTION BACKGROUNDS
   ============================================ */
.bb-cream-wrap {
  background: #EFE6D2;
  border-top: 1px solid #E6DBC2;
  border-bottom: 1px solid #E6DBC2;
  margin: 2rem -48px;
  padding: 2rem 48px;
}
@media (min-width: 1200px) {
  .bb-cream-wrap {
    margin: 2rem -72px;
    padding: 2rem 72px;
  }
}

/* ============================================
   CHAPTER MARK: a numeral and a label, set off
   by a hairline rule instead of a filled tile.
   ============================================ */
.bb-chapter-mark {
  display: flex;
  align-items: baseline;
  gap: 1rem;
  margin: 5rem 0 1.75rem;
  padding-top: 1.5rem;
  border-top: 1px solid var(--bb-border);
}
.bb-chapter-mark__num {
  font-family: 'Fraunces', Georgia, serif;
  font-size: 30px;
  font-weight: 500;
  color: var(--bb-green-accent);
}
.bb-chapter-mark__label {
  font-family: 'Instrument Sans', sans-serif;
  font-size: 11px;
  font-weight: 600;
  letter-spacing: 0.16em;
  text-transform: uppercase;
  color: var(--bb-navy);
  opacity: 0.7;
}

/* ============================================
   INTERNSHIP SECTION
   ============================================ */
.bb-internship-section h2 {
  font-family: 'Fraunces', Georgia, serif;
  color: var(--bb-green);
  font-size: 30px;
  font-weight: 500;
  margin: 0 0 0.5rem;
  letter-spacing: -0.02em;
}
.bb-internship-section .bb-section-intro {
  font-family: 'Instrument Sans', sans-serif;
  color: var(--bb-text-secondary);
  font-size: 17px;
  line-height: 1.65;
  margin: 0 0 1.5rem;
  max-width: 62ch;
}
.bb-internship-grid {
  display: grid;
  grid-template-columns: 1fr;
  gap: 0;
  margin-bottom: 1.25rem;
  border-top: 1px solid var(--bb-border);
}
@media (min-width: 769px) {
  .bb-internship-grid { grid-template-columns: repeat(2, 1fr); column-gap: 64px; }
}
.bb-internship-block {
  padding: 1.5rem 0;
  border-bottom: 1px solid var(--bb-border);
}
.bb-internship-block h3 {
  font-family: 'Instrument Sans', sans-serif;
  font-size: 11px;
  font-weight: 600;
  color: var(--bb-green-accent);
  text-transform: uppercase;
  letter-spacing: 0.16em;
  margin: 0 0 0.65rem;
}
.bb-internship-block p {
  font-family: 'Instrument Sans', sans-serif;
  font-size: 17px;
  color: var(--bb-text-secondary);
  line-height: 1.65;
  margin: 0 0 0.4rem;
}
.bb-internship-block p:last-child { margin-bottom: 0; }
.bb-internship-block ul {
  margin: 0;
  padding-left: 1.1rem;
}
.bb-internship-block li {
  font-size: 17px;
  color: var(--bb-text-secondary);
  line-height: 1.65;
  margin-bottom: 0.35rem;
}
.bb-program-badges {
  display: flex;
  flex-wrap: wrap;
  gap: 0.5rem 0.9rem;
  margin-top: 0.75rem;
}
.bb-program-badge {
  font-family: 'Instrument Sans', sans-serif;
  font-size: 15px;
  color: var(--bb-text-secondary);
  opacity: 0.82;
}
.bb-program-badge::after {
  content: '';
}

/* ============================================
   WHERE BIOTECH IS HEADING SECTION
   ============================================ */
.bb-future-section h2 {
  font-family: 'Fraunces', Georgia, serif;
  color: var(--bb-green);
  font-size: 30px;
  font-weight: 500;
  margin: 0 0 0.5rem;
  letter-spacing: -0.02em;
}
.bb-future-section .bb-section-intro {
  font-family: 'Instrument Sans', sans-serif;
  color: var(--bb-text-secondary);
  font-size: 17px;
  line-height: 1.65;
  margin: 0 0 1.5rem;
  max-width: 62ch;
}
.bb-future-grid {
  display: grid;
  grid-template-columns: 1fr;
  gap: 0;
  border-top: 1px solid var(--bb-border);
}
@media (min-width: 769px) {
  .bb-future-grid { grid-template-columns: repeat(2, 1fr); column-gap: 64px; }
}
.bb-future-card {
  padding: 1.5rem 0;
  border-bottom: 1px solid var(--bb-border);
  cursor: pointer;
}
.bb-future-card h3 {
  font-family: 'Instrument Sans', sans-serif;
  font-size: 17px;
  font-weight: 600;
  color: var(--bb-navy);
  margin: 0 0 0.6rem;
}
.bb-future-card p {
  font-family: 'Instrument Sans', sans-serif;
  font-size: 17px;
  color: var(--bb-text-secondary);
  opacity: 0.82;
  line-height: 1.65;
  margin: 0;
}

/* ============================================
   INTERNATIONAL CALLOUT
   ============================================ */
.bb-international-callout {
  padding: 1.5rem 0;
  border-top: 1px solid var(--bb-border);
  border-bottom: 1px solid var(--bb-border);
  margin: 1.5rem 0;
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
  line-height: 1.65;
  margin: 0;
}

/* ============================================
   PROGRAM CATEGORY ACCORDIONS
   ============================================ */
.bb-program-category {
  margin-bottom: 0.5rem;
  border-bottom: 1px solid var(--bb-border);
}
.bb-program-category summary {
  padding: 0.6rem 0;
  font-family: 'Instrument Sans', sans-serif;
  font-size: 17px;
  font-weight: 600;
  color: var(--bb-green);
  cursor: pointer;
  list-style: none;
  display: flex;
  align-items: center;
  user-select: none;
}
.bb-program-category summary::-webkit-details-marker { display: none; }
.bb-program-category summary::after {
  content: '+';
  margin-left: auto;
  font-size: 17px;
  color: var(--bb-green-accent);
  font-weight: 700;
}
.bb-program-category[open] summary::after { content: '\2212'; }
.bb-program-category .bb-program-badges {
  padding: 0 0 0.85rem;
}

/* ============================================
   FLIP CARDS: Industry Trends
   ============================================ */
.bb-flip-icon {
  font-family: 'Fraunces', Georgia, serif;
  font-size: 30px;
  color: var(--bb-green-accent);
  margin-bottom: 0.5rem;
  display: block;
}
.bb-flip-front h3 {
  font-size: 17px;
  color: var(--bb-navy);
  margin: 0 0 0.5rem;
}
.bb-flip-teaser {
  font-size: 17px;
  color: var(--bb-text-secondary);
  opacity: 0.82;
  line-height: 1.65;
  margin: 0 0 0.75rem;
}
.bb-flip-hint {
  display: inline-block;
  font-size: 11px;
  text-transform: uppercase;
  letter-spacing: 0.16em;
  color: var(--bb-green-accent);
  font-weight: 600;
}
.bb-flip-card.is-flipped .bb-flip-front { display: none; }
.bb-flip-back { display: none; }
.bb-flip-card.is-flipped .bb-flip-back { display: block; }
.bb-flip-back h3 {
  color: var(--bb-navy);
  font-size: 17px;
  margin: 0 0 0.6rem;
}
.bb-flip-back p {
  color: var(--bb-text-secondary);
  opacity: 0.82;
  font-size: 17px;
  line-height: 1.65;
  margin: 0 0 0.75rem;
}
.bb-flip-back-link {
  display: inline-block;
  font-size: 17px;
  color: var(--bb-green-accent);
  font-weight: 600;
}
.bb-flip-close {
  display: block;
  font-size: 11px;
  text-transform: uppercase;
  letter-spacing: 0.1em;
  color: var(--bb-gray);
  opacity: 0.6;
  margin-top: 1rem;
  cursor: pointer;
}
</style>

<header class="bb-page-header">
  <span class="eyebrow">Field Guide</span>
  <h1>Careers in Biotechnology</h1>
  <p class="bb-page-header__deck">There is no single path into biotech. Explore the major routes below, with realistic entry points for every background.</p>
</header>

<!-- PATHWAYS: stacked list, no carousel -->
<div class="bb-path-list">

  <!-- Research -->
  <div class="bb-path-row">
    <div class="bb-path-row__head">
      <span class="bb-path-row__num">01</span>
      <h2 class="bb-path-row__title">Research</h2>
    </div>
    <div class="bb-path-fields">
      <div>
        <div class="bb-detail-label">What it is</div>
        <p class="bb-detail-value">Discovering new knowledge, developing therapies, studying biological systems at the molecular and cellular level.</p>
      </div>
      <div>
        <div class="bb-detail-label">Where you'll work</div>
        <p class="bb-detail-value">Universities, research institutes, pharmaceutical companies, government labs (NIH, CDC).</p>
      </div>
      <div>
        <div class="bb-detail-label">Entry points</div>
        <div class="bb-detail-value"><ul>
          <li>Lab technician (Bachelor's degree)</li>
          <li>Research associate (Bachelor's + experience)</li>
          <li>PhD scientist (for independent research leads)</li>
        </ul></div>
      </div>
      <div>
        <div class="bb-detail-label">Skills needed</div>
        <p class="bb-detail-value">Experimental design, data analysis, patience, intellectual curiosity.</p>
      </div>
      <div>
        <div class="bb-companies-label">Example Organizations</div>
        <div class="bb-org-list">Genentech, NIH, Pfizer, Broad Institute</div>
      </div>
    </div>
  </div>

  <!-- Industry & Manufacturing -->
  <div class="bb-path-row">
    <div class="bb-path-row__head">
      <span class="bb-path-row__num">02</span>
      <h2 class="bb-path-row__title">Industry &amp; Manufacturing</h2>
    </div>
    <div class="bb-path-fields">
      <div>
        <div class="bb-detail-label">What it is</div>
        <p class="bb-detail-value">Scaling up production, quality control, and process optimization: turning lab discoveries into real-world products.</p>
      </div>
      <div>
        <div class="bb-detail-label">Where you'll work</div>
        <p class="bb-detail-value">Biotech companies, pharmaceutical manufacturers, contract manufacturing organizations (CMOs).</p>
      </div>
      <div>
        <div class="bb-detail-label">Entry points</div>
        <div class="bb-detail-value"><ul>
          <li>Manufacturing associate (High school + training)</li>
          <li>Process engineer (Bachelor's in engineering)</li>
          <li>Quality assurance specialist (Bachelor's in science)</li>
        </ul></div>
      </div>
      <div>
        <div class="bb-detail-label">Skills needed</div>
        <p class="bb-detail-value">Attention to detail, problem-solving, regulatory knowledge (GMP, GLP).</p>
      </div>
      <div>
        <div class="bb-companies-label">Example Organizations</div>
        <div class="bb-org-list">Lonza, Thermo Fisher, Amgen, Catalent</div>
      </div>
    </div>
  </div>

  <!-- Clinical -->
  <div class="bb-path-row">
    <div class="bb-path-row__head">
      <span class="bb-path-row__num">03</span>
      <h2 class="bb-path-row__title">Clinical</h2>
    </div>
    <div class="bb-path-fields">
      <div>
        <div class="bb-detail-label">What it is</div>
        <p class="bb-detail-value">Testing therapies in humans, managing clinical trials, ensuring patient safety throughout the drug development process.</p>
      </div>
      <div>
        <div class="bb-detail-label">Where you'll work</div>
        <p class="bb-detail-value">Hospitals, clinical research organizations (CROs), pharmaceutical companies.</p>
      </div>
      <div>
        <div class="bb-detail-label">Entry points</div>
        <div class="bb-detail-value"><ul>
          <li>Clinical research coordinator (Bachelor's)</li>
          <li>Clinical trial manager (Bachelor's + experience)</li>
          <li>Medical science liaison (Advanced degree)</li>
        </ul></div>
      </div>
      <div>
        <div class="bb-detail-label">Skills needed</div>
        <p class="bb-detail-value">Organization, communication, ethics, regulatory compliance (FDA, ICH guidelines).</p>
      </div>
      <div>
        <div class="bb-companies-label">Example Organizations</div>
        <div class="bb-org-list">IQVIA, Covance, Johnson &amp; Johnson, Medpace</div>
      </div>
    </div>
  </div>

  <!-- Regulatory & Policy -->
  <div class="bb-path-row">
    <div class="bb-path-row__head">
      <span class="bb-path-row__num">04</span>
      <h2 class="bb-path-row__title">Regulatory &amp; Policy</h2>
    </div>
    <div class="bb-path-fields">
      <div>
        <div class="bb-detail-label">What it is</div>
        <p class="bb-detail-value">Navigating FDA approval, ensuring compliance, and shaping public health policy at the bridge between science and government.</p>
      </div>
      <div>
        <div class="bb-detail-label">Where you'll work</div>
        <p class="bb-detail-value">Government agencies (FDA, NIH, EPA), consulting firms, pharmaceutical and biotech companies.</p>
      </div>
      <div>
        <div class="bb-detail-label">Entry points</div>
        <div class="bb-detail-value"><ul>
          <li>Regulatory affairs specialist (Bachelor's)</li>
          <li>Policy analyst (Bachelor's in science or policy)</li>
          <li>Compliance officer (Bachelor's + certifications)</li>
        </ul></div>
      </div>
      <div>
        <div class="bb-detail-label">Skills needed</div>
        <p class="bb-detail-value">Writing, attention to detail, deep understanding of regulations and policy processes.</p>
      </div>
      <div>
        <div class="bb-companies-label">Example Organizations</div>
        <div class="bb-org-list">FDA, Roche, Merck, PAREXEL</div>
      </div>
    </div>
  </div>

  <!-- Business & Operations -->
  <div class="bb-path-row">
    <div class="bb-path-row__head">
      <span class="bb-path-row__num">05</span>
      <h2 class="bb-path-row__title">Business &amp; Operations</h2>
    </div>
    <div class="bb-path-fields">
      <div>
        <div class="bb-detail-label">What it is</div>
        <p class="bb-detail-value">Strategy, partnerships, operations, and project management: the business side of bringing biotech innovations to market.</p>
      </div>
      <div>
        <div class="bb-detail-label">Where you'll work</div>
        <p class="bb-detail-value">Biotech startups, consulting firms, venture capital firms, established pharma companies.</p>
      </div>
      <div>
        <div class="bb-detail-label">Entry points</div>
        <div class="bb-detail-value"><ul>
          <li>Business analyst (Bachelor's in business or science)</li>
          <li>Project manager (Bachelor's + experience)</li>
          <li>Sales representative (Bachelor's)</li>
        </ul></div>
      </div>
      <div>
        <div class="bb-detail-label">Skills needed</div>
        <p class="bb-detail-value">Communication, business acumen, strategic thinking, networking.</p>
      </div>
      <div>
        <div class="bb-companies-label">Example Organizations</div>
        <div class="bb-org-list">Gilead, BCG, Vertex, Flagship Pioneering</div>
      </div>
    </div>
  </div>

  <!-- Science Communication -->
  <div class="bb-path-row">
    <div class="bb-path-row__head">
      <span class="bb-path-row__num">06</span>
      <h2 class="bb-path-row__title">Science Communication</h2>
    </div>
    <div class="bb-path-fields">
      <div>
        <div class="bb-detail-label">What it is</div>
        <p class="bb-detail-value">Translating complex science for public audiences through journalism, education, content creation, and advocacy.</p>
      </div>
      <div>
        <div class="bb-detail-label">Where you'll work</div>
        <p class="bb-detail-value">Media outlets, nonprofits, science museums, biotech marketing teams.</p>
      </div>
      <div>
        <div class="bb-detail-label">Entry points</div>
        <div class="bb-detail-value"><ul>
          <li>Science writer (Bachelor's + writing portfolio)</li>
          <li>Public engagement coordinator (Bachelor's)</li>
          <li>Medical communications specialist (Bachelor's + experience)</li>
        </ul></div>
      </div>
      <div>
        <div class="bb-detail-label">Skills needed</div>
        <p class="bb-detail-value">Writing, storytelling, scientific literacy, ability to simplify complexity without losing accuracy.</p>
      </div>
      <div>
        <div class="bb-companies-label">Example Organizations</div>
        <div class="bb-org-list">STAT News, NIH Communications, Ology, Science Friday</div>
      </div>
    </div>
  </div>

  <!-- Bioinformatics & Computational Biology -->
  <div class="bb-path-row">
    <div class="bb-path-row__head">
      <span class="bb-path-row__num">07</span>
      <h2 class="bb-path-row__title">Bioinformatics &amp; Computational Biology</h2>
    </div>
    <div class="bb-path-fields">
      <div>
        <div class="bb-detail-label">What it is</div>
        <p class="bb-detail-value">Using coding, statistics, and algorithms to analyze biological data: genomics, proteomics, drug discovery, and more.</p>
      </div>
      <div>
        <div class="bb-detail-label">Where you'll work</div>
        <p class="bb-detail-value">Biotech and pharma companies, academic research labs, hospitals, government agencies (NIH, FDA), and tech companies entering healthcare.</p>
      </div>
      <div>
        <div class="bb-detail-label">Entry points</div>
        <div class="bb-detail-value"><ul>
          <li>Bioinformatics analyst (Bachelor's in CS, biology, or bioinformatics)</li>
          <li>Data scientist in biotech (Bachelor's + Python/R skills)</li>
          <li>Computational biologist (Master's or PhD for research-focused roles)</li>
        </ul></div>
      </div>
      <div>
        <div class="bb-detail-label">Skills needed</div>
        <p class="bb-detail-value">Python, R, SQL, statistics, genomics tools (BLAST, Galaxy, GATK), and comfort with large datasets.</p>
      </div>
      <div>
        <div class="bb-companies-label">Example Organizations</div>
        <div class="bb-org-list">23andMe, Illumina, Broad Institute, DNAnexus</div>
      </div>
    </div>
  </div>

</div>

<div class="bb-next-steps">
  <h2>Ready to go deeper?</h2>
  <ul>
    <li>Browse <a href="/resources/">The Learning Lab</a> for career-specific media and resources</li>
    <li>Check out <a href="/products/">The Biotech Blueprint</a>, a step-by-step guide built for your starting point</li>
    <li>Learn what biotech actually is on the <a href="/what-is-biotech/">What is Biotech?</a> page</li>
  </ul>
</div>

<!-- International callout -->
<div class="bb-international-callout">
  <span class="bb-intl-header">Outside the US?</span>
  <p>The biotech industry structure differs internationally. Europe and Asia have more publicly funded research conducted through universities and government institutes, with fewer venture-backed startups than you'd find in Boston or the Bay Area. In the UK, Germany, and the Netherlands, many biotech roles are embedded within academic medical centers or government research councils. If you're outside the US, look for roles with national research institutes (e.g., the Wellcome Sanger Institute, EMBL, or RIKEN in Japan) alongside commercial opportunities.</p>
</div>

<!-- SECTION DIVIDER -->
<div class="bb-chapter-mark">
  <span class="bb-chapter-mark__num">01</span>
  <span class="bb-chapter-mark__label">Getting Started</span>
</div>

<div class="bb-cream-wrap">
<!-- FINDING YOUR FIRST INTERNSHIP -->
<div class="bb-internship-section">
  <h2>Finding Your First Internship</h2>
  <p class="bb-section-intro">Your first biotech internship doesn't need to be at Pfizer. It needs to get you in the room. Here's a practical guide to navigating the process, from well-known formal programs to cold outreach to academic labs.</p>

  <div class="bb-internship-grid">

    <div class="bb-internship-block">
      <h3>Well-Known Programs to Apply To</h3>
      <p>These are competitive but well worth applying. They're structured, paid, and recognized by hiring managers. Browse by sector:</p>

      <details class="bb-program-category">
        <summary>Research, Pharma &amp; Biotech</summary>
        <div class="bb-program-badges">
          <span class="bb-program-badge">Pfizer Summer Internship</span>
          <span class="bb-program-badge">Genentech SURGE</span>
          <span class="bb-program-badge">Amgen Scholars</span>
          <span class="bb-program-badge">AstraZeneca Internship</span>
          <span class="bb-program-badge">Merck Internship</span>
          <span class="bb-program-badge">J&amp;J Intern Program</span>
          <span class="bb-program-badge">Eli Lilly Summer Internship</span>
          <span class="bb-program-badge">AbbVie Internship</span>
          <span class="bb-program-badge">BMS Discovery Fellowship</span>
          <span class="bb-program-badge">Regeneron Internship</span>
          <span class="bb-program-badge">Moderna Internship</span>
          <span class="bb-program-badge">Abbott Internship</span>
        </div>
      </details>

      <details class="bb-program-category">
        <summary>Consulting &amp; Life Sciences Strategy</summary>
        <div class="bb-program-badges">
          <span class="bb-program-badge">Simon-Kucher &amp; Partners</span>
          <span class="bb-program-badge">Clearview Healthcare Partners</span>
          <span class="bb-program-badge">L.E.K. Consulting</span>
          <span class="bb-program-badge">ZS Associates</span>
          <span class="bb-program-badge">Putnam Associates</span>
          <span class="bb-program-badge">Analysis Group</span>
          <span class="bb-program-badge">Guidehouse Life Sciences</span>
          <span class="bb-program-badge">Huron Consulting</span>
          <span class="bb-program-badge">Avalere Health</span>
          <span class="bb-program-badge">IQVIA Consulting</span>
        </div>
      </details>

      <details class="bb-program-category">
        <summary>Government &amp; Academic</summary>
        <div class="bb-program-badges">
          <span class="bb-program-badge">NIH Summer Internship Program</span>
          <span class="bb-program-badge">NSF REU</span>
          <span class="bb-program-badge">FDA Commissioner's Fellowship</span>
          <span class="bb-program-badge">CDC Public Health Associate Program</span>
          <span class="bb-program-badge">NCI Cancer Research Internship</span>
        </div>
      </details>

      <details class="bb-program-category">
        <summary>Medical Devices &amp; Diagnostics</summary>
        <div class="bb-program-badges">
          <span class="bb-program-badge">Medtronic Internship</span>
          <span class="bb-program-badge">Boston Scientific Internship</span>
          <span class="bb-program-badge">Abbott Diagnostics</span>
          <span class="bb-program-badge">Becton Dickinson</span>
          <span class="bb-program-badge">Illumina Internship</span>
          <span class="bb-program-badge">Thermo Fisher Internship</span>
        </div>
      </details>

      <p style="margin-top:0.65rem;">Check each company's careers page directly. Most open applications between October and February for summer positions.</p>
    </div>

    <div class="bb-internship-block">
      <h3>Application Timeline</h3>
      <ul>
        <li><strong>August to October (fall):</strong> Start researching programs. Update your resume. Identify 15 to 20 target programs and companies.</li>
        <li><strong>October to December:</strong> Major pharma/biotech applications open. Apply early. Most use rolling review.</li>
        <li><strong>January to February:</strong> Academic lab programs (REU, NIH SIP) open, and startup internship postings spike on LinkedIn. This is also when you should start hearing back from fall applications to major pharma programs: responses typically take 8 to 12 weeks, so don't panic if your inbox is still quiet.</li>
        <li><strong>March to April:</strong> Follow-up and interviews. Smaller companies often post well into spring.</li>
        <li><strong>May to June:</strong> Last-minute opportunities. Keep checking even if you haven't heard back from early applications.</li>
      </ul>
    </div>

    <div class="bb-internship-block">
      <h3>What to Include in Your Application</h3>
      <ul>
        <li><strong>Resume:</strong> 1 page, reverse chronological, tailored to each role. Lead with relevant coursework and skills if you don't yet have experience.</li>
        <li><strong>Cover letter:</strong> Short (3 paragraphs). Why this company, why this role, what you bring. Skip generic openers.</li>
        <li><strong>Research statement (for academic labs):</strong> 1 to 2 paragraphs on your interests and what you hope to learn.</li>
        <li><strong>References:</strong> Have 2 to 3 professors or supervisors ready. Ask them in advance.</li>
        <li><strong>Writing sample (if requested):</strong> A lab report, class paper, or anything that demonstrates your ability to communicate science clearly.</li>
      </ul>
      <p style="margin-top:0.75rem; font-size:15px; color:var(--bb-text-secondary); font-style:italic;">Want real examples? <a href="/products/">The Biotech Blueprint</a> includes annotated resume samples, cover letter templates, and cold email scripts built specifically for biotech applications. If you want to see what a strong application actually looks like, start there.</p>
    </div>

    <div class="bb-internship-block">
      <h3>Where to Search</h3>
      <ul>
        <li><strong>LinkedIn:</strong> Filter by "Internship" and "Biotech" or "Pharmaceutical." Set alerts for new postings.</li>
        <li><strong>Handshake:</strong> Best for university-specific postings, especially for smaller regional biotech companies that recruit campus-to-campus.</li>
        <li><strong>Company career pages:</strong> Always check directly. Many roles aren't posted on aggregators. Bookmark 10 to 15 companies you'd want to work for.</li>
        <li><strong>University career center:</strong> Often has exclusive postings from alumni-affiliated companies. Ask about biotech-specific fairs.</li>
        <li><strong>Cold outreach:</strong> Email professors with funded labs. A well-written cold email to a principal investigator can get you into a research lab even without a formal posting.</li>
      </ul>
    </div>

    <div class="bb-internship-block">
      <h3>What to Expect: Pharma vs. Startup vs. Gov/Academic</h3>
      <ul>
        <li><strong>Big Pharma (Pfizer, Merck, J&J):</strong> Structured programs, assigned mentors, formal presentations, intern cohort events. Slower-paced, process-heavy. Good for learning how large organizations operate and building a network.</li>
        <li><strong>Biotech Startup:</strong> Less structure, broader responsibilities, often more hands-on from day one. You may be the only intern. Fast-paced and unpredictable: you'll learn a lot, but you'll need to drive your own experience.</li>
        <li><strong>Government/Academic Lab (NIH, university labs, REU):</strong> Research-focused, usually stipend-based. Excellent for students considering graduate school. Slower publication cycles but deep scientific exposure. Independent project work is common.</li>
      </ul>
    </div>

    <div class="bb-internship-block">
      <h3>Quick Tips That Actually Help</h3>
      <ul>
        <li>Apply broadly early, then narrow your focus in February. Don't wait for your "dream" company to post before applying anywhere.</li>
        <li>Tailor your resume keywords to match each job posting. Many companies use ATS screening before a human sees your application.</li>
        <li>A warm introduction beats a cold application every time. LinkedIn alumni tools and professor connections are underutilized by most students.</li>
        <li>Don't overlook smaller CROs, CDMOs, and regional biotech companies. They often offer more hands-on work than large programs.</li>
      </ul>
    </div>

  </div>
</div>
</div><!-- /.bb-cream-wrap -->

<!-- SECTION DIVIDER -->
<div class="bb-chapter-mark">
  <span class="bb-chapter-mark__num">02</span>
  <span class="bb-chapter-mark__label">Industry Trends</span>
</div>

<!-- WHERE BIOTECH IS HEADING -->
<div class="bb-future-section">
  <h2>Where Biotech Is Heading</h2>
  <p class="bb-section-intro">The biotech industry is changing faster than most career guides acknowledge. These five areas are shaping where the jobs, funding, and scientific energy are flowing in the next decade, and what that means for you.</p>

  <p style="font-size:11px; text-transform:uppercase; letter-spacing:0.16em; color:var(--bb-gray); margin: -0.75rem 0 1.25rem; font-family:'Instrument Sans',sans-serif;">Click any item to expand the full picture.</p>

  <div class="bb-future-grid">

    <div class="bb-future-card bb-flip-card">
      <div class="bb-flip-front">
        <span class="bb-flip-icon">01</span>
        <h3>AI &amp; Drug Discovery</h3>
        <p class="bb-flip-teaser">AlphaFold changed what computational biology teams can do in months. New career paths are emerging fast at the intersection of ML and biology.</p>
        <span class="bb-flip-hint">Click to explore &rarr;</span>
      </div>
      <div class="bb-flip-back">
        <h3>AI &amp; Drug Discovery</h3>
        <p>AlphaFold's protein structure predictions changed what computational biology teams can accomplish in months rather than years. AI-assisted clinical trial design is reducing the time it takes to identify patient cohorts and predict drug responses. New roles are emerging at the intersection of machine learning and wet lab science: computational biologists, AI research scientists, and data engineers focused on genomics pipelines are among the fastest-growing positions in pharma and early-stage biotech. You don't need to be a programmer to contribute: biology domain expertise is increasingly what distinguishes useful AI tools from ones that fail in practice.</p>
        <a href="https://www.statnews.com" class="bb-flip-back-link" target="_blank" rel="noopener">Explore on STAT News &rarr;</a>
        <span class="bb-flip-close">&larr; Click to flip back</span>
      </div>
    </div>

    <div class="bb-future-card bb-flip-card">
      <div class="bb-flip-front">
        <span class="bb-flip-icon">02</span>
        <h3>Synthetic Biology</h3>
        <p class="bb-flip-teaser">Engineering organisms for fragrances, therapeutics, and industrial materials. Biomanufacturing is pulling in serious investment and a new category of roles.</p>
        <span class="bb-flip-hint">Click to explore &rarr;</span>
      </div>
      <div class="bb-flip-back">
        <h3>Synthetic Biology</h3>
        <p>Companies like Ginkgo Bioworks have built platform-level infrastructure for engineering organisms to produce everything from fragrances to industrial chemicals to therapeutic proteins. Biomanufacturing (using engineered microbes and cell lines to produce products that previously required petroleum chemistry or animal agriculture) is attracting significant investment. Roles range from metabolic engineering and strain development to process scale-up and fermentation operations. Synthetic biology also intersects with food, materials, and agriculture, making it one of the broader application areas for biology training outside traditional pharma.</p>
        <a href="https://www.nature.com" class="bb-flip-back-link" target="_blank" rel="noopener">Read on Nature &rarr;</a>
        <span class="bb-flip-close">&larr; Click to flip back</span>
      </div>
    </div>

    <div class="bb-future-card bb-flip-card">
      <div class="bb-flip-front">
        <span class="bb-flip-icon">03</span>
        <h3>Longevity &amp; Aging Biotech</h3>
        <p class="bb-flip-teaser">VC interest in aging science is real and growing. Here's what it means for early-career researchers entering this scientifically exciting niche.</p>
        <span class="bb-flip-hint">Click to explore &rarr;</span>
      </div>
      <div class="bb-flip-back">
        <h3>Longevity &amp; Aging Biotech</h3>
        <p>Venture capital interest in longevity science has grown substantially, with firms like Calico (backed by Alphabet) and Unity Biotechnology pursuing interventions targeting the biology of aging itself rather than individual diseases. The field remains scientifically early-stage, but it's generating roles in translational research, clinical development, and biomarker science. For students interested in this space, a strong foundation in cell biology, metabolism, or genetics (combined with an understanding of the long and uncertain clinical timelines involved) puts you ahead of most applicants entering this niche.</p>
        <a href="https://www.nia.nih.gov" class="bb-flip-back-link" target="_blank" rel="noopener">Explore at NIA (NIH) &rarr;</a>
        <span class="bb-flip-close">&larr; Click to flip back</span>
      </div>
    </div>

    <div class="bb-future-card bb-flip-card">
      <div class="bb-flip-front">
        <span class="bb-flip-icon">04</span>
        <h3>Personalized Medicine &amp; Diagnostics</h3>
        <p class="bb-flip-teaser">Sequencing costs have dropped dramatically. Companion diagnostics are now FDA-required for many oncology drugs. The clinical genomics job market is expanding.</p>
        <span class="bb-flip-hint">Click to explore &rarr;</span>
      </div>
      <div class="bb-flip-back">
        <h3>Personalized Medicine &amp; Diagnostics</h3>
        <p>Genomic sequencing costs have dropped dramatically, making population-scale genomics programs feasible. Companion diagnostics (tests that determine whether a patient will respond to a specific therapy) are now required for many oncology drug approvals. Liquid biopsy, which detects cancer-related DNA fragments in blood rather than tissue, is reshaping early detection. Roles in this space include clinical genomics scientists, bioinformatics analysts, regulatory affairs specialists focused on IVD (in vitro diagnostics), and commercial teams that work with oncologists and hospital systems to implement these tools in clinical practice.</p>
        <a href="https://www.genome.gov" class="bb-flip-back-link" target="_blank" rel="noopener">Explore at genome.gov &rarr;</a>
        <span class="bb-flip-close">&larr; Click to flip back</span>
      </div>
    </div>

    <div class="bb-future-card bb-flip-card" style="grid-column: 1 / -1;">
      <div class="bb-flip-front">
        <span class="bb-flip-icon">05</span>
        <h3>How AI Is Changing (Not Eliminating) Wet Lab Roles</h3>
        <p class="bb-flip-teaser">The most common student concern, addressed directly: AI accelerates hypothesis generation; it doesn't pipette, troubleshoot assays, or navigate biological unpredictability.</p>
        <span class="bb-flip-hint">Click to explore &rarr;</span>
      </div>
      <div class="bb-flip-back">
        <h3>How AI Is Changing (Not Eliminating) Wet Lab Roles</h3>
        <p>A common concern among students is that AI will automate laboratory work and reduce the need for bench scientists. This misreads what AI actually does in a biotech context. AI accelerates hypothesis generation and data interpretation; it does not yet pipette, culture cells, troubleshoot failed assays, or navigate the physical unpredictability of biological systems. What is changing: scientists spend less time on routine data analysis and more time on experimental design, interpretation, and cross-functional communication. The human skills that remain essential are precisely the ones that are hardest to automate: deep domain intuition, the ability to recognize when something unexpected in your data is noise versus signal, and the judgment to know when to abandon a hypothesis and why. If anything, the growing role of AI in biotech increases the premium on scientists who can both run experiments and engage meaningfully with computational outputs, a combination that is currently rare and therefore valuable.</p>
        <a href="https://www.nature.com" class="bb-flip-back-link" target="_blank" rel="noopener">Read on Nature &rarr;</a>
        <span class="bb-flip-close">&larr; Click to flip back</span>
      </div>
    </div>

  </div>
</div>

<script>
// Flip cards: industry trends
(function() {
  document.querySelectorAll('.bb-flip-card').forEach(function(card) {
    card.addEventListener('click', function(e) {
      if (e.target.tagName === 'A') return; // let link clicks through
      card.classList.toggle('is-flipped');
    });
  });
})();
</script>
