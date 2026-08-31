---
layout: single
title: "Guides"
permalink: /products/
---

<style>
@import url('https://fonts.googleapis.com/css2?family=Fraunces:ital,opsz,wght@0,9..144,400..600;1,9..144,400..600&family=Instrument+Sans:wght@400;500;600;700&display=swap');
body { font-family: 'Instrument Sans', -apple-system, BlinkMacSystemFont, sans-serif; }
h1, h2, h3 { font-family: 'Fraunces', Georgia, serif; }

:root {
  --bb-green: #24221A;
  --bb-green-accent: #5C6335;
  --bb-green-hover: #3B4223;
  --bb-navy: #24221A;
  --bb-white: #EFE6D2;
  --bb-off-white: #E6DBC2;
  --bb-text-secondary: #5B5745;
  --bb-gray: #5B5745;
  --bb-border: rgba(36,34,26,0.12);
}

/* Main product layout */
.bb-product-layout {
  display: grid;
  grid-template-columns: 1fr;
  gap: 1.75rem;
  margin-bottom: 2.5rem;
}

/* Product image: the one product photo on the site, kept because
   it's the actual guide cover, not decorative stock photography */
.bb-product-img {
  overflow: hidden;
  min-height: 180px;
}
.bb-product-img img {
  width: 100%;
  height: 100%;
  display: block;
  object-fit: cover;
}

/* Product details: no card box, set off by a top rule */
.bb-product-card {
  border-top: 1px solid var(--bb-border);
  padding-top: 1.5rem;
}
.bb-product-eyebrow {
  font-family: 'Instrument Sans', sans-serif;
  font-size: 11px;
  font-weight: 600;
  letter-spacing: 0.16em;
  text-transform: uppercase;
  color: var(--bb-green-accent);
  margin: 0 0 0.5rem;
}
.bb-product-card h2 {
  font-family: 'Fraunces', Georgia, serif;
  color: var(--bb-navy);
  font-size: 30px;
  font-weight: 500;
  margin: 0 0 0.65rem;
  letter-spacing: -0.02em;
  line-height: 1.2;
}
.bb-product-tagline {
  color: var(--bb-text-secondary);
  opacity: 0.82;
  font-family: 'Instrument Sans', sans-serif;
  font-size: 17px;
  line-height: 1.65;
  margin: 0 0 1.25rem;
  max-width: 62ch;
}

/* Section headers inside card */
.bb-section-label {
  font-family: 'Instrument Sans', sans-serif;
  font-size: 11px;
  font-weight: 600;
  letter-spacing: 0.16em;
  text-transform: uppercase;
  color: var(--bb-green-accent);
  margin: 0 0 0.65rem;
  padding-top: 1.5rem;
  border-top: 1px solid var(--bb-border);
}
.bb-section-label:first-of-type {
  border-top: none;
  padding-top: 0;
}

/* Feature list (What's Included) */
.bb-feature-list {
  list-style: none;
  padding: 0;
  margin: 0 0 1.25rem;
  max-width: 62ch;
}
.bb-feature-list li {
  position: relative;
  padding-left: 1.4rem;
  margin-bottom: 0.75rem;
  color: var(--bb-text-secondary);
  opacity: 0.82;
  font-size: 17px;
  line-height: 1.65;
}
.bb-feature-list li::before {
  content: '-';
  position: absolute;
  left: 0;
  color: var(--bb-green-accent);
  font-weight: 700;
}

/* Who It's For prose */
.bb-who-prose {
  color: var(--bb-text-secondary);
  opacity: 0.82;
  font-size: 17px;
  line-height: 1.65;
  margin: 0 0 1.25rem;
  max-width: 62ch;
}

/* Price & CTA */
.bb-price-row {
  display: flex;
  align-items: baseline;
  gap: 0.85rem;
  margin-bottom: 0.85rem;
  flex-wrap: wrap;
}
.bb-price-tag {
  font-family: 'Fraunces', Georgia, serif;
  font-size: 30px;
  font-weight: 500;
  color: var(--bb-navy);
  letter-spacing: -0.01em;
}
.bb-buy-btn {
  display: inline-block;
  background: var(--bb-green-accent);
  color: var(--bb-white) !important;
  padding: 0.85rem 2rem;
  font-family: 'Instrument Sans', sans-serif;
  font-weight: 600;
  font-size: 17px;
  text-decoration: none !important;
  transition: background 0.15s ease;
}
.bb-buy-btn:hover {
  background: var(--bb-green-hover);
  color: var(--bb-white) !important;
}
.bb-coming-soon-note {
  color: var(--bb-gray);
  font-size: 17px;
  opacity: 0.7;
  font-style: italic;
  margin-top: 0.5rem;
}

/* Why a Paid Guide section: rules, not a filled box */
.bb-why-paid {
  border-top: 1px solid var(--bb-border);
  border-bottom: 1px solid var(--bb-border);
  padding: 1.75rem 0;
  margin-bottom: 1.5rem;
}
.bb-why-paid h2 {
  font-family: 'Fraunces', Georgia, serif;
  color: var(--bb-navy);
  font-size: 30px;
  font-weight: 500;
  margin: 0 0 0.85rem;
}
.bb-why-paid p {
  color: var(--bb-text-secondary);
  opacity: 0.82;
  font-size: 17px;
  line-height: 1.65;
  margin: 0 0 0.75rem;
  max-width: 62ch;
}
.bb-why-paid p:last-child { margin-bottom: 0; }

/* Coming Soon roadmap */
.bb-roadmap {
  padding-bottom: 1.5rem;
  margin-bottom: 1.5rem;
  border-bottom: 1px solid var(--bb-border);
}
.bb-roadmap h2 {
  font-family: 'Fraunces', Georgia, serif;
  color: var(--bb-navy);
  font-size: 30px;
  font-weight: 500;
  margin: 0 0 1rem;
}
.bb-roadmap-item {
  padding: 1rem 0;
  border-top: 1px solid var(--bb-border);
  max-width: 62ch;
}
.bb-roadmap-dot { display: none; }
.bb-roadmap-item p {
  color: var(--bb-text-secondary);
  opacity: 0.82;
  font-size: 17px;
  line-height: 1.65;
  margin: 0;
}
.bb-roadmap-item strong {
  color: var(--bb-navy);
}

/* Contact note */
.bb-contact-note {
  color: var(--bb-gray);
  opacity: 0.7;
  font-size: 17px;
}
.bb-contact-note a {
  color: var(--bb-green-accent);
  font-weight: 600;
}

/* Free Preview: a rule-framed callout, not a heavily bordered card */
.bb-preview-card {
  border-top: 1px solid var(--bb-border);
  border-bottom: 1px solid var(--bb-border);
  padding: 1.75rem 0;
  margin-bottom: 2.5rem;
}
.bb-preview-eyebrow {
  font-family: 'Instrument Sans', sans-serif;
  font-size: 11px;
  font-weight: 600;
  letter-spacing: 0.16em;
  text-transform: uppercase;
  color: var(--bb-green-accent);
  margin: 0 0 0.5rem;
}
.bb-preview-card h2 {
  font-family: 'Fraunces', Georgia, serif;
  color: var(--bb-navy);
  font-size: 30px;
  font-weight: 500;
  margin: 0 0 0.6rem;
  letter-spacing: -0.02em;
}
.bb-preview-card p {
  font-family: 'Instrument Sans', sans-serif;
  color: var(--bb-text-secondary);
  opacity: 0.82;
  font-size: 17px;
  line-height: 1.65;
  margin: 0 0 1.1rem;
  max-width: 62ch;
}
.bb-preview-sample {
  display: flex;
  align-items: center;
  gap: 1rem;
  padding: 1rem 0;
  border-top: 1px solid var(--bb-border);
  border-bottom: 1px solid var(--bb-border);
  margin-bottom: 1rem;
  flex-wrap: wrap;
}
.bb-preview-sample-icon { display: none; }
.bb-preview-sample-info {
  flex: 1;
  min-width: 0;
}
.bb-preview-sample-info strong {
  display: block;
  font-family: 'Instrument Sans', sans-serif;
  font-size: 17px;
  font-weight: 600;
  color: var(--bb-navy);
  margin-bottom: 0.25rem;
}
.bb-preview-sample-info span {
  font-family: 'Instrument Sans', sans-serif;
  font-size: 17px;
  color: var(--bb-gray);
  opacity: 0.7;
}
.bb-preview-btn {
  display: inline-block;
  color: var(--bb-green-accent) !important;
  font-family: 'Instrument Sans', sans-serif;
  font-weight: 600;
  font-size: 17px;
  white-space: nowrap;
  flex-shrink: 0;
}
.bb-preview-btn:hover {
  color: var(--bb-green-hover) !important;
}
.bb-preview-coming-soon {
  font-family: 'Instrument Sans', sans-serif;
  font-size: 11px;
  font-weight: 600;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  color: var(--bb-green-hover);
}

/* International callout */
.bb-international-callout {
  border-top: 1px solid var(--bb-border);
  border-bottom: 1px solid var(--bb-border);
  padding: 1.25rem 0;
  margin: 1.5rem 0;
  max-width: 62ch;
}
.bb-international-callout .bb-intl-header {
  font-family: 'Instrument Sans', sans-serif;
  font-size: 11px;
  font-weight: 600;
  letter-spacing: 0.16em;
  text-transform: uppercase;
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

/* Mobile */
@media (max-width: 768px) {
  .bb-preview-sample {
    flex-direction: column;
    align-items: stretch;
    gap: 0.75rem;
  }
  .bb-preview-btn {
    text-align: left;
    display: block;
  }
}

/* Desktop */
@media (min-width: 769px) {
  .bb-product-layout { grid-template-columns: 2fr 3fr; align-items: start; gap: 2.25rem; }
  .bb-product-img { min-height: 260px; }
}
</style>

<header class="bb-page-header">
  <span class="eyebrow">Guides</span>
  <h1>BioBridge Guides</h1>
  <p class="bb-page-header__deck">Structured, experience-backed guidance for anyone figuring out their path into biotech.</p>
</header>

<!-- FREE PREVIEW CARD -->
<div class="bb-preview-card">
  <p class="bb-preview-eyebrow">Try Before You Buy</p>
  <h2>Get a Free Preview &rarr;</h2>
  <p>Not sure if the Blueprint is right for you? Download a free sample and see the level of detail, annotation, and practical guidance you can expect throughout the full guide.</p>
  <div class="bb-preview-sample">
    <div class="bb-preview-sample-info">
      <strong>Free Sample: The Cold Email Template</strong>
      <span>The exact email framework that got responses from senior people at major biotech and pharma companies, annotated line by line.</span>
    </div>
    <a href="/free-preview" class="bb-preview-btn">Get Free Preview &rarr;</a>
  </div>
</div>

<!-- MAIN PRODUCT LAYOUT -->
<div class="bb-product-layout">

  <!-- Product image -->
  <div class="bb-product-img">
    <img src="/assets/images/blueprint-cover.png" alt="The Biotech Blueprint cover">
  </div>

  <!-- Product details -->
  <div class="bb-product-card">
    <p class="bb-product-eyebrow">BioBridge Guide</p>
    <h2>The Biotech Blueprint</h2>
    <p class="bb-product-tagline">A comprehensive, practical guide for anyone taking their first steps into biotechnology. Real materials, annotated and explained, with roadmaps developed from direct experience navigating this field as a student.</p>

    <p class="bb-section-label">What's Included</p>
    <ul class="bb-feature-list">
      <li><strong>A personal resume that landed a biotech internship at a major pharma company:</strong> annotated line by line so you understand every formatting and content choice, not just what it looks like.</li>
      <li><strong>Cold email and outreach templates that got responses from partners at firms and senior people at major biotech and pharma companies:</strong> including the exact framing that works when you have no existing connections.</li>
      <li><strong>A pivot story roadmap based on a real transition from pre-dental to biotech:</strong> with the specific steps, reframing strategies, and application materials that made it work.</li>
      <li><strong>An interview prep guide with actual questions asked at biotech companies, organized by role type:</strong> with guidance on how to approach each one.</li>
      <li><strong>A curated list of biotech-friendly professors and labs organized by research area:</strong> for students trying to get into research without existing connections.</li>
      <li><strong>A career quiz to help identify which biotech role fits your background and goals:</strong> with tailored next steps based on your results.</li>
      <li><strong>A complete career timeline and entry roadmap:</strong> mapping out exactly what to do at each stage, from your first research experience to your first industry role.</li>
      <li><strong>A full interview prep roadmap covering the entire hiring arc:</strong> from application to offer, with what to expect at each stage and how to prepare for it.</li>
    </ul>

    <p class="bb-section-label">Who It's For</p>
    <p class="bb-who-prose">The Blueprint is for anyone who wants more than a list of tips. If you're in high school trying to get ahead before college applications or summer programs, it maps out where to start. If you're a college student (any major) wondering how to connect what you're studying to a real biotech career, it gives you a framework. Recent grads who need to translate their degree into actual next steps will find it useful, and so will career changers who've spent too much time wading through generic advice that doesn't account for where they're actually starting from. This is written for anyone who learns better from real examples and experience-backed reasoning than from scattered internet searches or generic listicles.</p>

    <p class="bb-section-label">Get the Guide</p>
    <div class="bb-price-row">
      <span class="bb-price-tag">$22</span>
    </div>
    <a href="https://tranquility120.gumroad.com/l/the-biotech-blueprint" class="bb-buy-btn gumroad-button" data-gumroad-product-id="the-biotech-blueprint">Purchase on Gumroad</a>
  </div>

</div>

<!-- WHY A PAID GUIDE -->
<div class="bb-why-paid">
  <h2>Why a Paid Guide?</h2>
  <p>I spent months figuring out what no one explains clearly: which resume format actually gets interviews, how to cold email a professor and hear back, what to say in your first biotech internship application. A lot of it was trial and error. The Blueprint is what came out of that process: my actual materials, annotated and explained, alongside roadmaps I developed from my own experience as a student navigating this field.</p>
  <p>Everything on this website (the career pages, the resource library, the FAQ) is free and always will be. The Blueprint is for people who want everything in one place, with more depth, in a format they can save and return to. If you want experience-backed guidance in one place, this is it.</p>
</div>

<!-- International callout: resume/CV context -->
<div class="bb-international-callout">
  <div class="bb-intl-header">Outside the US?</div>
  <p>Canada, the UK, and Australia typically use CVs (curriculum vitae) rather than resumes, and formatting expectations differ: CVs are often longer, include more detail on academic history, and may include a personal statement. The resume materials in the Biotech Blueprint are formatted for US applications. The frameworks and principles apply internationally, but you may want to adapt the formatting to match local conventions in your country.</p>
</div>

<!-- COMING SOON -->
<div class="bb-roadmap">
  <h2>Coming Soon</h2>
  <div class="bb-roadmap-item">
    <div class="bb-roadmap-dot"></div>
    <p><strong>Mentorship Program Access</strong>: Connect directly with biotech professionals who have been where you are and can help you figure out the next step.</p>
  </div>
  <div class="bb-roadmap-item">
    <div class="bb-roadmap-dot"></div>
    <p><strong>BioBridge High School Program Initiative at Thomas Jefferson University:</strong> A structured educational program bringing biotech literacy directly into high school classrooms, modeled after initiatives like First Generation Investors, with the goal of giving students hands-on exposure to the industry before college.</p>
  </div>
</div>

<p class="bb-contact-note">Questions about the guide? Email <a href="mailto:jeans.connects@gmail.com">jeans.connects@gmail.com</a></p>
