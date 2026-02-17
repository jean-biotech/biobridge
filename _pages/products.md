---
layout: single
title: "Products"
permalink: /products/
---

<style>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=Playfair+Display:wght@600;700&display=swap');
body { font-family: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif; }
h1, h2, h3 { font-family: 'Playfair Display', Georgia, serif; }

:root {
  --bb-navy: #0f2b3c;
  --bb-teal: #0d7377;
  --bb-teal-light: #14919b;
  --bb-teal-dark: #094f52;
  --bb-teal-bg: #f0f9fa;
  --bb-white: #ffffff;
  --bb-off-white: #f7f9fb;
  --bb-text-secondary: #475569;
  --bb-gray: #64748b;
  --bb-border: #e2e8f0;
}

/* Page Header — Mobile First */
.bb-page-hero {
  background: linear-gradient(160deg, var(--bb-navy) 0%, var(--bb-teal-dark) 100%);
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
  background: radial-gradient(ellipse at 80% 20%, rgba(13,115,119,0.15) 0%, transparent 60%);
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

/* Product Card */
.bb-product-card {
  background: var(--bb-white);
  border: 1px solid var(--bb-border);
  border-radius: 10px;
  padding: 2rem 1.5rem;
  margin-bottom: 2rem;
  box-shadow: 0 4px 16px rgba(0,0,0,0.06);
}
.bb-product-card h2 {
  font-family: 'Inter', sans-serif;
  color: var(--bb-navy);
  font-size: 1.35rem;
  font-weight: 700;
  margin-top: 0;
  margin-bottom: 1rem;
}
.bb-product-card h3 {
  font-family: 'Inter', sans-serif;
  color: var(--bb-navy);
  font-size: 1rem;
  font-weight: 600;
  margin-bottom: 0.75rem;
}
.bb-product-desc {
  color: var(--bb-text-secondary);
  font-size: 0.95rem;
  line-height: 1.7;
  margin-bottom: 1.5rem;
}

/* Feature List */
.bb-feature-list {
  list-style: none;
  padding: 0;
  margin: 0 0 1.5rem;
}
.bb-feature-list li {
  position: relative;
  padding-left: 1.75rem;
  margin-bottom: 0.6rem;
  color: var(--bb-text-secondary);
  font-size: 0.92rem;
  line-height: 1.7;
}
.bb-feature-list li::before {
  content: '\2713';
  position: absolute;
  left: 0;
  color: var(--bb-teal);
  font-weight: 700;
  font-size: 1rem;
}

/* Price & CTA */
.bb-price-tag {
  display: inline-block;
  background: var(--bb-navy);
  color: var(--bb-white);
  padding: 0.5rem 1.5rem;
  border-radius: 6px;
  font-family: 'Inter', sans-serif;
  font-size: 1.35rem;
  font-weight: 700;
  margin-bottom: 1rem;
}
.bb-buy-btn {
  display: inline-block;
  background: var(--bb-teal);
  color: var(--bb-white) !important;
  padding: 0.875rem 2.25rem;
  border-radius: 6px;
  font-family: 'Inter', sans-serif;
  font-weight: 600;
  font-size: 0.95rem;
  text-decoration: none !important;
  transition: all 0.25s ease;
  border: 2px solid var(--bb-teal);
  margin-top: 0.5rem;
  min-height: 44px;
}
.bb-buy-btn:hover {
  background: var(--bb-teal-dark);
  border-color: var(--bb-teal-dark);
  transform: translateY(-2px);
  box-shadow: 0 6px 20px rgba(13,115,119,0.3);
  color: var(--bb-white) !important;
}

/* Why Paid */
.bb-why-paid {
  background: var(--bb-teal-bg);
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
  margin-top: 0;
  margin-bottom: 1rem;
}
.bb-why-paid p {
  color: var(--bb-text-secondary);
  font-size: 0.92rem;
  line-height: 1.75;
  margin-bottom: 0.75rem;
}
.bb-why-paid p:last-child {
  margin-bottom: 0;
}

/* Roadmap */
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
  margin-top: 0;
  margin-bottom: 1.25rem;
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
  background: var(--bb-teal);
  border-radius: 50%;
  margin-top: 0.5rem;
}
.bb-roadmap-item p {
  color: var(--bb-text-secondary);
  font-size: 0.92rem;
  line-height: 1.5;
  margin: 0;
}
.bb-roadmap-item strong {
  color: var(--bb-navy);
}

/* Contact Note */
.bb-contact-note {
  text-align: center;
  color: var(--bb-gray);
  font-size: 0.92rem;
}
.bb-contact-note a {
  color: var(--bb-teal);
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
  .bb-product-card {
    padding: 2.5rem 3rem;
    border-radius: 12px;
  }
  .bb-product-card h2 {
    font-size: 1.6rem;
  }
  .bb-why-paid {
    padding: 2rem 2.5rem;
  }
  .bb-roadmap {
    padding: 2rem 2.5rem;
  }
}
</style>

<div class="bb-page-hero">
  <h1>BioBridge Guides</h1>
  <p>Premium resources designed to accelerate your biotech journey.</p>
</div>

<div class="bb-product-card">
  <h2>The Biotech Starter Guide</h2>
  <p class="bb-product-desc">A comprehensive guide for anyone taking their first step into biotechnology. Everything you need in one place, organized for clarity and action.</p>

  <h3>What is Included</h3>
  <ul class="bb-feature-list">
    <li>Detailed career pathway breakdowns with salary ranges and growth potential</li>
    <li>Step-by-step roadmaps for different backgrounds (high school, college, career changers)</li>
    <li>Resource recommendations with context and guidance on how to use them</li>
    <li>Real-world case studies and profiles from people at different stages</li>
    <li>Actionable next steps for each pathway</li>
    <li>Common pitfalls and how to avoid them</li>
  </ul>

  <h3>Who It is For</h3>
  <ul class="bb-feature-list">
    <li>High school students exploring STEM careers</li>
    <li>College students considering biotech majors or minors</li>
    <li>Career changers curious about transitioning into biotech</li>
    <li>Anyone who wants structured guidance instead of scattered information</li>
  </ul>

  <div class="bb-price-tag">$9.99</div>
  <br>
  <a href="#" class="bb-buy-btn">Purchase on Gumroad</a>
  <p style="color: var(--bb-gray); font-size: 0.85rem; margin-top: 0.75rem;"><em>(Link coming soon)</em></p>
</div>

<div class="bb-why-paid">
  <h2>Why a Paid Guide?</h2>
  <p>BioBridge's core resources -- this website, curated links, and basic guidance -- will always be free.</p>
  <p>The Biotech Starter Guide is a <strong>premium resource</strong> for people who want everything in one place, deeper detail than the free content, a printable and save-able format, and to support BioBridge's mission.</p>
  <p><strong>All proceeds go toward:</strong> hosting costs, expanding free resources, and building mentorship programs.</p>
</div>

<div class="bb-roadmap">
  <h2>Coming Soon</h2>
  <div class="bb-roadmap-item">
    <div class="bb-roadmap-dot"></div>
    <p><strong>Biotech Career Toolkit</strong> -- Templates for resumes, cold emails, informational interviews</p>
  </div>
  <div class="bb-roadmap-item">
    <div class="bb-roadmap-dot"></div>
    <p><strong>Industry-Specific Deep Dives</strong> -- Pharma vs. ag-bio vs. synthetic biology</p>
  </div>
  <div class="bb-roadmap-item">
    <div class="bb-roadmap-dot"></div>
    <p><strong>Mentorship Program Access</strong> -- Connect with biotech professionals directly</p>
  </div>
</div>

<p class="bb-contact-note">Questions about the guide? Email <a href="mailto:contact@biobridge.org">contact@biobridge.org</a></p>
