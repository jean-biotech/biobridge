---
layout: single
title: "Resource Hub"
permalink: /resources/
toc: true
toc_label: "Categories"
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

/* Page Header — Mobile First */
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

/* Resource Section Headers */
.bb-resource-section h2 {
  font-family: 'Inter', sans-serif;
  color: var(--bb-navy);
  font-size: 1.15rem;
  font-weight: 700;
  padding-bottom: 0.75rem;
  border-bottom: 2px solid var(--bb-green-accent);
  margin-bottom: 1.25rem;
}

/* Resource Grid — Mobile First */
.bb-resource-grid {
  display: grid;
  grid-template-columns: 1fr;
  gap: 1rem;
  margin-bottom: 2.5rem;
}
.bb-resource-card {
  background: var(--bb-white);
  border: 1px solid var(--bb-border);
  border-radius: 8px;
  padding: 1.25rem 1.5rem;
  transition: all 0.25s ease;
}
.bb-resource-card:hover {
  box-shadow: 0 4px 16px rgba(0,0,0,0.08);
  transform: translateY(-1px);
}
.bb-resource-card h3 {
  margin: 0 0 0.4rem;
  font-family: 'Inter', sans-serif;
  font-size: 0.95rem;
  font-weight: 600;
}
.bb-resource-card h3 a {
  color: var(--bb-navy);
  text-decoration: none;
  transition: color 0.2s ease;
}
.bb-resource-card h3 a:hover {
  color: var(--bb-green-accent);
}
.bb-resource-card p {
  color: var(--bb-gray);
  font-size: 0.85rem;
  line-height: 1.6;
  margin: 0;
}
.bb-book-card h3 {
  font-style: italic;
}

/* CTA Footer */
.bb-cta-footer {
  text-align: center;
  padding: 1.75rem 1.5rem;
  background: var(--bb-green-bg);
  border-radius: 8px;
  border: 1px solid var(--bb-border);
}
.bb-cta-footer p {
  color: var(--bb-text-secondary);
  font-size: 0.95rem;
  margin: 0;
}
.bb-cta-footer a {
  color: var(--bb-green-accent);
  font-weight: 600;
}

/* Desktop */
@media (min-width: 769px) {
  .bb-page-hero {
    padding: 3.5rem 3rem;
    border-radius: 12px;
  }
  .bb-page-hero h1 {
    font-size: 2.25rem;
  }
  .bb-page-hero p {
    font-size: 1.1rem;
  }
  .bb-resource-grid {
    grid-template-columns: repeat(3, 1fr);
    gap: 1.25rem;
  }
  .bb-resource-section h2 {
    font-size: 1.35rem;
  }
  .bb-cta-footer {
    padding: 2rem 2.5rem;
  }
}
</style>

<div class="bb-page-hero">
  <h1>Curated Resources for Biotech Beginners</h1>
  <p>All resources are free (or have free tiers) and beginner-friendly. Hand-picked for quality and accessibility.</p>
</div>

<div class="bb-resource-section">

## Newsletters

<div class="bb-resource-grid">
  <div class="bb-resource-card">
    <h3><a href="https://www.statnews.com/newsletters/" target="_blank">The Readout</a></h3>
    <p>STAT News weekly biotech/pharma roundup</p>
  </div>
  <div class="bb-resource-card">
    <h3><a href="https://endpts.com/" target="_blank">Endpoints News</a></h3>
    <p>Biotech industry news and analysis</p>
  </div>
  <div class="bb-resource-card">
    <h3><a href="https://www.nature.com/briefing" target="_blank">Nature Briefing</a></h3>
    <p>Daily science news from Nature</p>
  </div>
</div>

</div>

<div class="bb-resource-section">

## Podcasts

<div class="bb-resource-grid">
  <div class="bb-resource-card">
    <h3><a href="https://biotechstartups.com/podcast/" target="_blank">The Biotech Startups Podcast</a></h3>
    <p>Founder stories and industry insights</p>
  </div>
  <div class="bb-resource-card">
    <h3><a href="https://mendelspod.com/" target="_blank">Mendelspod</a></h3>
    <p>Science communication and genetics</p>
  </div>
  <div class="bb-resource-card">
    <h3><a href="https://www.statnews.com/category/readout-loud/" target="_blank">The Readout Loud</a></h3>
    <p>STAT's weekly biotech news discussion</p>
  </div>
</div>

</div>

<div class="bb-resource-section">

## Beginner-Friendly Reads

<div class="bb-resource-grid">
  <div class="bb-resource-card">
    <h3><a href="https://www.alextelford.com/cells-are-very-small" target="_blank">Cells Are Very Small</a></h3>
    <p>Visual introduction to cell biology</p>
  </div>
  <div class="bb-resource-card">
    <h3><a href="https://learn.genetics.utah.edu/" target="_blank">Learn.Genetics</a></h3>
    <p>Interactive genetics tutorials</p>
  </div>
  <div class="bb-resource-card">
    <h3><a href="https://www.nature.com/scitable" target="_blank">Scitable by Nature</a></h3>
    <p>Free science education resource</p>
  </div>
</div>

</div>

<div class="bb-resource-section">

## YouTube Channels

<div class="bb-resource-grid">
  <div class="bb-resource-card">
    <h3><a href="https://www.youtube.com/c/inanutshell" target="_blank">Kurzgesagt</a></h3>
    <p>Animated science explainers on genetic engineering and more</p>
  </div>
  <div class="bb-resource-card">
    <h3><a href="https://www.youtube.com/c/PrimerBlobs" target="_blank">Primer</a></h3>
    <p>Evolution and biology simulations</p>
  </div>
  <div class="bb-resource-card">
    <h3><a href="https://www.youtube.com/c/veritasium" target="_blank">Veritasium</a></h3>
    <p>Science and engineering deep dives</p>
  </div>
</div>

</div>

<div class="bb-resource-section">

## Online Courses (Free)

<div class="bb-resource-grid">
  <div class="bb-resource-card">
    <h3><a href="https://ocw.mit.edu/courses/biology/" target="_blank">MIT OpenCourseWare - Biology</a></h3>
    <p>Full MIT courses, completely free</p>
  </div>
  <div class="bb-resource-card">
    <h3><a href="https://www.khanacademy.org/science/biology" target="_blank">Khan Academy - Biology</a></h3>
    <p>Comprehensive, self-paced learning</p>
  </div>
  <div class="bb-resource-card">
    <h3><a href="https://www.ibiology.org/" target="_blank">iBiology</a></h3>
    <p>Talks by leading scientists</p>
  </div>
</div>

</div>

<div class="bb-resource-section">

## Books (Accessible)

<div class="bb-resource-grid">
  <div class="bb-resource-card bb-book-card">
    <h3>"The Gene" by Siddhartha Mukherjee</h3>
    <p>History of genetics, written for a general audience</p>
  </div>
  <div class="bb-resource-card bb-book-card">
    <h3>"The Immortal Life of Henrietta Lacks"</h3>
    <p>Ethics and cell biology</p>
  </div>
  <div class="bb-resource-card bb-book-card">
    <h3>"Spillover" by David Quammen</h3>
    <p>Infectious diseases and ecology</p>
  </div>
</div>

</div>

<div class="bb-cta-footer">
  <p>Have a resource to suggest? <a href="/get-involved/">Get in touch</a> and help us grow this collection.</p>
</div>
