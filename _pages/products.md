---
layout: single
title: "Guides"
permalink: /products/
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
  --bb-gray: #64748b;
  --bb-border: #e2e8f0;
}

/* Page Header */
.bb-page-hero {
  background: linear-gradient(160deg, var(--bb-navy) 0%, var(--bb-green-dark) 100%);
  color: var(--bb-white);
  padding: 2.5rem 1.5rem;
  border-radius: 10px;
  margin-bottom: 2.5rem;
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
  font-size: 1.75rem;
  font-weight: 700;
  margin: 0 0 0.75rem;
  color: var(--bb-white);
  letter-spacing: -0.02em;
  position: relative;
}
.bb-page-hero p {
  font-family: 'Inter', sans-serif;
  font-size: 1rem;
  color: rgba(255,255,255,0.8);
  margin: 0;
  font-weight: 300;
  line-height: 1.6;
  position: relative;
}

/* Main product layout */
.bb-product-layout {
  display: grid;
  grid-template-columns: 1fr;
  gap: 2rem;
  margin-bottom: 2.5rem;
}

/* Product image placeholder */
.bb-product-img {
  background: linear-gradient(145deg, #e8f0ea, #d4e8d9);
  border: 2px dashed rgba(45,95,63,0.25);
  border-radius: 10px;
  padding: 2.5rem 1.5rem;
  text-align: center;
  color: var(--bb-gray);
  font-family: 'Inter', sans-serif;
  font-size: 0.82rem;
  font-weight: 500;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  gap: 0.75rem;
  min-height: 200px;
}
.bb-product-img-icon {
  font-size: 2.5rem;
  opacity: 0.45;
}
.bb-product-img-label {
  display: inline-block;
  background: rgba(45,95,63,0.1);
  border: 1px dashed rgba(45,95,63,0.3);
  border-radius: 6px;
  padding: 0.4rem 1rem;
  letter-spacing: 0.02em;
}

/* Product card */
.bb-product-card {
  background: var(--bb-white);
  border: 1px solid var(--bb-border);
  border-radius: 10px;
  padding: 2rem 1.5rem;
  box-shadow: 0 4px 20px rgba(0,0,0,0.06);
}
.bb-product-eyebrow {
  font-family: 'Inter', sans-serif;
  font-size: 0.72rem;
  font-weight: 700;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  color: var(--bb-green-accent);
  margin: 0 0 0.5rem;
}
.bb-product-card h2 {
  font-family: 'Playfair Display', Georgia, serif;
  color: var(--bb-navy);
  font-size: 1.65rem;
  font-weight: 700;
  margin: 0 0 0.75rem;
  letter-spacing: -0.02em;
  line-height: 1.2;
}
.bb-product-tagline {
  color: var(--bb-text-secondary);
  font-family: 'Inter', sans-serif;
  font-size: 0.95rem;
  line-height: 1.7;
  margin: 0 0 1.5rem;
}

/* Section headers inside card */
.bb-section-label {
  font-family: 'Inter', sans-serif;
  font-size: 0.75rem;
  font-weight: 700;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  color: var(--bb-green);
  margin: 0 0 0.75rem;
  padding-top: 1.25rem;
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
  margin: 0 0 1.5rem;
}
.bb-feature-list li {
  position: relative;
  padding-left: 1.85rem;
  margin-bottom: 0.7rem;
  color: var(--bb-text-secondary);
  font-size: 0.92rem;
  line-height: 1.65;
}
.bb-feature-list li::before {
  content: '\2713';
  position: absolute;
  left: 0;
  color: var(--bb-green-accent);
  font-weight: 700;
  font-size: 1rem;
  line-height: 1.65;
}

/* Price & CTA */
.bb-price-row {
  display: flex;
  align-items: center;
  gap: 1rem;
  margin-bottom: 1rem;
  flex-wrap: wrap;
}
.bb-price-tag {
  display: inline-block;
  background: var(--bb-navy);
  color: var(--bb-white);
  padding: 0.5rem 1.5rem;
  border-radius: 6px;
  font-family: 'Inter', sans-serif;
  font-size: 1.5rem;
  font-weight: 700;
  letter-spacing: -0.02em;
}
.bb-buy-btn {
  display: inline-block;
  background: var(--bb-green-accent);
  color: var(--bb-white) !important;
  padding: 0.875rem 2.25rem;
  border-radius: 6px;
  font-family: 'Inter', sans-serif;
  font-weight: 600;
  font-size: 0.95rem;
  text-decoration: none !important;
  transition: all 0.25s ease;
  border: 2px solid var(--bb-green-accent);
  min-height: 44px;
}
.bb-buy-btn:hover {
  background: var(--bb-green);
  border-color: var(--bb-green);
  transform: translateY(-2px);
  box-shadow: 0 6px 20px rgba(45,95,63,0.3);
  color: var(--bb-white) !important;
}
.bb-coming-soon-note {
  color: var(--bb-gray);
  font-size: 0.83rem;
  font-style: italic;
  margin-top: 0.4rem;
}

/* Why a Paid Guide section */
.bb-why-paid {
  background: var(--bb-green-bg);
  border: 1px solid var(--bb-border);
  border-radius: 8px;
  padding: 1.75rem 1.5rem;
  margin-bottom: 2rem;
}
.bb-why-paid h2 {
  font-family: 'Inter', sans-serif;
  color: var(--bb-navy);
  font-size: 1.1rem;
  font-weight: 700;
  margin: 0 0 1rem;
}
.bb-why-paid p {
  color: var(--bb-text-secondary);
  font-size: 0.93rem;
  line-height: 1.8;
  margin: 0 0 0.85rem;
}
.bb-why-paid p:last-child { margin-bottom: 0; }

/* Coming Soon roadmap */
.bb-roadmap {
  background: var(--bb-white);
  border: 1px solid var(--bb-border);
  border-radius: 8px;
  padding: 1.75rem 1.5rem;
  margin-bottom: 2rem;
}
.bb-roadmap h2 {
  font-family: 'Inter', sans-serif;
  color: var(--bb-navy);
  font-size: 1.1rem;
  font-weight: 700;
  margin: 0 0 1.25rem;
}
.bb-roadmap-item {
  display: flex;
  align-items: flex-start;
  gap: 1rem;
  margin-bottom: 1rem;
  padding-bottom: 1rem;
  border-bottom: 1px solid #f1f5f9;
}
.bb-roadmap-item:last-child {
  border-bottom: none;
  margin-bottom: 0;
  padding-bottom: 0;
}
.bb-roadmap-dot {
  width: 10px;
  height: 10px;
  min-width: 10px;
  background: var(--bb-green-accent);
  border-radius: 50%;
  margin-top: 0.45rem;
}
.bb-roadmap-item p {
  color: var(--bb-text-secondary);
  font-size: 0.92rem;
  line-height: 1.55;
  margin: 0;
}
.bb-roadmap-item strong {
  color: var(--bb-navy);
}

/* Contact note */
.bb-contact-note {
  text-align: center;
  color: var(--bb-gray);
  font-size: 0.9rem;
}
.bb-contact-note a {
  color: var(--bb-green-accent);
  font-weight: 600;
}

/* Desktop */
@media (min-width: 769px) {
  .bb-page-hero { padding: 3.5rem 3rem; border-radius: 12px; }
  .bb-page-hero h1 { font-size: 2.25rem; }
  .bb-page-hero p { font-size: 1.1rem; }
  .bb-product-layout { grid-template-columns: 2fr 3fr; align-items: start; gap: 2.5rem; }
  .bb-product-card { padding: 2.5rem 2.75rem; }
  .bb-product-card h2 { font-size: 2rem; }
  .bb-product-img { min-height: 280px; }
  .bb-why-paid { padding: 2rem 2.5rem; }
  .bb-roadmap { padding: 2rem 2.5rem; }
}
</style>

<div class="bb-page-hero">
  <h1>BioBridge Guides</h1>
  <p>Structured, experience-backed guidance for anyone figuring out their path into biotech.</p>
</div>

<!-- MAIN PRODUCT LAYOUT -->
<div class="bb-product-layout">

  <!-- Product image -->
  <div class="bb-product-img">
    <div class="bb-product-img-icon">📘</div>
    <div class="bb-product-img-label">Guide Preview / Cover Image</div>
    <div style="font-size:0.75rem; color: var(--bb-gray); margin-top:0.25rem;">Placeholder — final mockup coming</div>
  </div>

  <!-- Product details -->
  <div class="bb-product-card">
    <p class="bb-product-eyebrow">BioBridge Guide</p>
    <h2>The Biotech Blueprint</h2>
    <p class="bb-product-tagline">A comprehensive, practical guide for anyone taking their first steps into biotechnology. Not a textbook — a roadmap, built from real experience.</p>

    <p class="bb-section-label">What's Included</p>
    <ul class="bb-feature-list">
      <li>A real resume example that landed a biotech internship, with annotations explaining every choice.</li>
      <li>An interview question prep guide with actual questions asked at biotech companies — and how to answer them.</li>
      <li>Cold email templates for reaching out to researchers and hiring managers that actually get responses.</li>
      <li>A curated contact list of biotech-friendly professors and labs, organized by research area.</li>
      <li>A step-by-step breakdown of how to read a scientific paper as a beginner — no science background needed.</li>
      <li>Roadmaps for four different starting points: high school, non-biology college major, career changer, and graduate student.</li>
      <li>Common mistakes people make applying to biotech roles — and exactly how to fix them.</li>
    </ul>

    <p class="bb-section-label">Who It's For</p>
    <ul class="bb-feature-list">
      <li>High school students who want a head start before college applications or summer programs.</li>
      <li>College students of any major — including those with no science background — who are curious about biotech careers.</li>
      <li>Recent graduates figuring out how to translate their degree into a real job in the industry.</li>
      <li>Career changers who want structured, honest guidance rather than scattered Google results.</li>
      <li>Anyone who learns better from experience-backed advice than from a textbook or a generic listicle.</li>
    </ul>

    <p class="bb-section-label">Get the Guide</p>
    <div class="bb-price-row">
      <span class="bb-price-tag">$22</span>
    </div>
    <a href="#" class="bb-buy-btn">Purchase on Gumroad</a>
    <p class="bb-coming-soon-note">Link coming soon — guide in final review.</p>
  </div>

</div>

<!-- WHY A PAID GUIDE -->
<div class="bb-why-paid">
  <h2>Why a Paid Guide?</h2>
  <p>I spent months figuring out what no one explains clearly. This guide is what I wish I'd had — written from my own experience navigating biotech as a student, not from a textbook.</p>
  <p>Everything on this website — the career pages, the resource library, the FAQ — will always be free. The Blueprint is for people who want everything in one place, with more depth, in a format they can save and return to.</p>
  <p><strong>All proceeds go toward</strong> hosting costs, expanding free resources, and building the mentorship program.</p>
</div>

<!-- COMING SOON -->
<div class="bb-roadmap">
  <h2>Coming Soon</h2>
  <div class="bb-roadmap-item">
    <div class="bb-roadmap-dot"></div>
    <p><strong>Mentorship Program Access</strong> — Connect directly with biotech professionals who have been where you are and can help you figure out the next step.</p>
  </div>
</div>

<p class="bb-contact-note">Questions about the guide? Email <a href="mailto:contact@biobridge.org">contact@biobridge.org</a></p>
