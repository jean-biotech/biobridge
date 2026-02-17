---
layout: splash
title: " "
classes: wide
---

<style>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&family=Playfair+Display:wght@600;700;800&display=swap');

/* ================================================================
   BioBridge — Green Biotech Design System
   Color Palette: Forest Green (#2D5F3F) + Navy (#1A1A2E)
   Mobile-first with spacious desktop layout
   ================================================================ */

:root {
  --bb-green: #2D5F3F;
  --bb-green-accent: #3A7D5C;
  --bb-green-bright: #4CAF50;
  --bb-green-hover: #66BB6A;
  --bb-green-dark: #1A3A28;
  --bb-green-bg: #E8F5E9;
  --bb-green-bg-subtle: #F1F8F4;
  --bb-teal-accent: #26A69A;
  --bb-navy: #1A1A2E;
  --bb-charcoal: #2C3E50;
  --bb-white: #ffffff;
  --bb-off-white: #FAFAFA;
  --bb-text: #1e293b;
  --bb-text-secondary: #475569;
  --bb-gray: #757575;
  --bb-gray-light: #9E9E9E;
  --bb-border: #e2e8f0;
  --bb-shadow-sm: 0 1px 3px rgba(0,0,0,0.06);
  --bb-shadow-md: 0 4px 16px rgba(0,0,0,0.08);
  --bb-shadow-lg: 0 12px 32px rgba(0,0,0,0.1);
  --bb-radius: 8px;
  --bb-radius-lg: 12px;
}

body { font-family: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif; }
h1, h2, h3, h4 { font-family: 'Playfair Display', Georgia, serif; }

/* ================================================================
   HERO SECTION — Full-width, green gradient
   ================================================================ */

.bb-hero {
  background: linear-gradient(160deg, var(--bb-navy) 0%, var(--bb-green-dark) 40%, var(--bb-green) 100%);
  color: var(--bb-white);
  text-align: center;
  padding: 3.5rem 1.5rem 3rem;
  position: relative;
  overflow: hidden;
}

.bb-hero::before {
  content: '';
  position: absolute;
  top: 0; left: 0; width: 100%; height: 100%;
  background:
    radial-gradient(ellipse at 20% 80%, rgba(45,95,63,0.25) 0%, transparent 60%),
    radial-gradient(ellipse at 80% 20%, rgba(76,175,80,0.1) 0%, transparent 60%);
  pointer-events: none;
}

.bb-hero::after {
  content: '';
  position: absolute;
  bottom: 0; left: 0; width: 100%; height: 1px;
  background: linear-gradient(90deg, transparent, rgba(76,175,80,0.4), transparent);
}

.bb-hero-inner {
  max-width: 820px;
  margin: 0 auto;
  position: relative;
  z-index: 1;
}

.bb-hero-label {
  display: inline-block;
  font-family: 'Inter', sans-serif;
  font-size: 0.75rem;
  font-weight: 600;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  color: var(--bb-green-hover);
  margin-bottom: 1.25rem;
  padding: 0.4rem 1rem;
  border: 1px solid rgba(102,187,106,0.3);
  border-radius: 100px;
}

.bb-hero h1 {
  font-size: 2.25rem;
  font-weight: 700;
  line-height: 1.2;
  margin: 0 0 1.25rem;
  letter-spacing: -0.02em;
  color: var(--bb-white);
}

.bb-hero-subtitle {
  font-family: 'Inter', sans-serif;
  font-size: 1.05rem;
  font-weight: 300;
  color: rgba(255,255,255,0.75);
  margin: 0 0 2rem;
  line-height: 1.65;
  max-width: 560px;
  margin-left: auto;
  margin-right: auto;
}

.bb-hero-buttons {
  display: flex;
  gap: 0.875rem;
  justify-content: center;
  flex-direction: column;
  align-items: center;
}

.bb-btn-primary {
  display: inline-block;
  background: var(--bb-green-bright);
  color: var(--bb-white) !important;
  padding: 0.875rem 2rem;
  border-radius: 6px;
  font-family: 'Inter', sans-serif;
  font-weight: 600;
  font-size: 0.95rem;
  text-decoration: none !important;
  transition: all 0.25s ease;
  border: 2px solid var(--bb-green-bright);
  width: 100%;
  max-width: 260px;
  text-align: center;
}

.bb-btn-primary:hover {
  background: var(--bb-green);
  border-color: var(--bb-green);
  transform: translateY(-2px);
  box-shadow: 0 6px 20px rgba(45,95,63,0.35);
  color: var(--bb-white) !important;
}

.bb-btn-secondary {
  display: inline-block;
  background: transparent;
  color: rgba(255,255,255,0.9) !important;
  padding: 0.875rem 2rem;
  border-radius: 6px;
  font-family: 'Inter', sans-serif;
  font-weight: 500;
  font-size: 0.95rem;
  text-decoration: none !important;
  transition: all 0.25s ease;
  border: 1.5px solid rgba(255,255,255,0.25);
  width: 100%;
  max-width: 260px;
  text-align: center;
}

.bb-btn-secondary:hover {
  background: rgba(255,255,255,0.08);
  border-color: rgba(255,255,255,0.45);
  color: var(--bb-white) !important;
}

/* ================================================================
   METRICS BAR
   ================================================================ */

.bb-metrics {
  background: var(--bb-green-bg-subtle);
  padding: 1.5rem;
  border-bottom: 1px solid var(--bb-border);
}

.bb-metrics-inner {
  max-width: 1200px;
  margin: 0 auto;
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 1rem;
}

.bb-metric {
  text-align: center;
}

.bb-metric-num {
  font-family: 'Playfair Display', serif;
  font-weight: 700;
  font-size: 1.35rem;
  color: var(--bb-green);
  display: block;
  line-height: 1.2;
}

.bb-metric-label {
  font-family: 'Inter', sans-serif;
  font-size: 0.8rem;
  color: var(--bb-gray);
  font-weight: 500;
  letter-spacing: 0.02em;
}

/* ================================================================
   IMAGE PLACEHOLDER
   ================================================================ */

.bb-image-placeholder {
  background: linear-gradient(135deg, var(--bb-green-bg), var(--bb-green-bg-subtle));
  border: 2px dashed var(--bb-border);
  border-radius: var(--bb-radius-lg);
  padding: 3rem 2rem;
  text-align: center;
  color: var(--bb-gray);
  font-family: 'Inter', sans-serif;
  font-size: 0.85rem;
  font-weight: 500;
  line-height: 1.5;
  margin: 2rem 1.5rem;
}

/* ================================================================
   SECTION — WHAT WE OFFER (PILLARS)
   ================================================================ */

.bb-section {
  padding: 3.5rem 1.5rem;
  max-width: 1200px;
  margin: 0 auto;
}

.bb-section-header {
  text-align: center;
  margin-bottom: 2.5rem;
}

.bb-section-header h2 {
  color: var(--bb-green);
  font-size: 1.75rem;
  font-weight: 700;
  margin: 0 0 0.75rem;
  letter-spacing: -0.02em;
}

.bb-section-header p {
  color: var(--bb-gray);
  font-family: 'Inter', sans-serif;
  font-size: 1rem;
  margin: 0;
  line-height: 1.6;
  max-width: 560px;
  margin-left: auto;
  margin-right: auto;
}

.bb-card-grid {
  display: grid;
  grid-template-columns: 1fr;
  gap: 1.25rem;
}

.bb-card {
  background: var(--bb-white);
  border: 1px solid var(--bb-border);
  border-radius: var(--bb-radius);
  padding: 1.75rem 1.5rem;
  transition: all 0.25s ease;
  position: relative;
}

.bb-card:hover {
  box-shadow: var(--bb-shadow-md);
  transform: translateY(-2px);
  border-color: rgba(45,95,63,0.2);
}

.bb-card-number {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  width: 36px;
  height: 36px;
  background: var(--bb-green-bg);
  color: var(--bb-green);
  font-family: 'Inter', sans-serif;
  font-weight: 700;
  font-size: 0.85rem;
  border-radius: 8px;
  margin-bottom: 1rem;
}

.bb-card h3 {
  font-family: 'Inter', sans-serif;
  color: var(--bb-green);
  font-size: 1.1rem;
  font-weight: 600;
  margin: 0 0 0.75rem;
}

.bb-card p {
  color: var(--bb-text-secondary);
  font-size: 0.92rem;
  line-height: 1.7;
  margin: 0 0 1rem;
}

.bb-card-link {
  font-family: 'Inter', sans-serif;
  color: var(--bb-green-accent) !important;
  font-weight: 600;
  font-size: 0.875rem;
  text-decoration: none !important;
  display: inline-flex;
  align-items: center;
  gap: 0.35rem;
  transition: color 0.2s ease;
}

.bb-card-link:hover {
  color: var(--bb-green) !important;
}

/* ================================================================
   SPLIT SECTION — PROBLEM / SOLUTION
   ================================================================ */

.bb-split {
  display: grid;
  grid-template-columns: 1fr;
  max-width: 1200px;
  margin: 0 auto 3rem;
  border-radius: var(--bb-radius-lg);
  overflow: hidden;
  box-shadow: var(--bb-shadow-md);
}

.bb-split-left {
  background: var(--bb-navy);
  color: var(--bb-white);
  padding: 2.5rem 1.5rem;
}

.bb-split-right {
  background: var(--bb-white);
  padding: 2.5rem 1.5rem;
  border: 1px solid var(--bb-border);
  border-top: none;
}

.bb-split h2 {
  font-size: 1.35rem;
  font-weight: 700;
  margin: 0 0 1rem;
  letter-spacing: -0.01em;
}

.bb-split-left h2 {
  color: var(--bb-green-hover);
}

.bb-split-right h2 {
  color: var(--bb-green);
}

.bb-split p {
  font-family: 'Inter', sans-serif;
  font-size: 0.95rem;
  line-height: 1.8;
  margin: 0;
}

.bb-split-left p {
  color: rgba(255,255,255,0.8);
}

.bb-split-right p {
  color: var(--bb-text-secondary);
}

/* ================================================================
   FOUNDER STORY SECTION
   ================================================================ */

.bb-story {
  background: var(--bb-green-bg-subtle);
  padding: 3.5rem 1.5rem;
  border-top: 1px solid var(--bb-border);
  border-bottom: 1px solid var(--bb-border);
}

.bb-story-inner {
  max-width: 1100px;
  margin: 0 auto;
}

.bb-story h2 {
  color: var(--bb-green);
  font-size: 1.75rem;
  font-weight: 700;
  margin: 0 0 2rem;
  letter-spacing: -0.02em;
}

.bb-story-layout {
  display: flex;
  flex-direction: column;
  gap: 2rem;
  align-items: center;
}

.bb-story-photo-wrap {
  flex-shrink: 0;
}

.bb-story-photo {
  width: 160px;
  height: 160px;
  border-radius: 50%;
  object-fit: cover;
  box-shadow: var(--bb-shadow-md);
  border: 4px solid var(--bb-white);
}

.bb-story-content p {
  font-family: 'Inter', sans-serif;
  font-size: 0.95rem;
  line-height: 1.85;
  color: var(--bb-text-secondary);
  margin: 0 0 1rem;
}

.bb-story-content p:last-of-type {
  margin-bottom: 0;
}

.bb-connect {
  margin-top: 1.75rem;
  padding-top: 1.5rem;
  border-top: 1px solid var(--bb-border);
  display: flex;
  align-items: center;
  gap: 1rem;
  flex-wrap: wrap;
}

.bb-connect-label {
  font-family: 'Inter', sans-serif;
  font-weight: 600;
  font-size: 0.875rem;
  color: var(--bb-green);
}

.bb-connect-link {
  display: inline-flex;
  align-items: center;
  gap: 0.4rem;
  text-decoration: none !important;
  font-family: 'Inter', sans-serif;
  font-size: 0.875rem;
  font-weight: 500;
  color: var(--bb-charcoal) !important;
  padding: 0.4rem 0.85rem;
  border-radius: 6px;
  border: 1px solid var(--bb-border);
  transition: all 0.2s ease;
  background: var(--bb-white);
}

.bb-connect-link:hover {
  border-color: var(--bb-green-accent);
  color: var(--bb-green-accent) !important;
  box-shadow: var(--bb-shadow-sm);
}

/* ================================================================
   BOTTOM CTA
   ================================================================ */

.bb-cta {
  background: linear-gradient(160deg, var(--bb-navy) 0%, var(--bb-green-dark) 100%);
  color: var(--bb-white);
  text-align: center;
  padding: 3.5rem 1.5rem;
  position: relative;
}

.bb-cta::before {
  content: '';
  position: absolute;
  top: 0; left: 0; width: 100%; height: 1px;
  background: linear-gradient(90deg, transparent, rgba(76,175,80,0.3), transparent);
}

.bb-cta h2 {
  font-size: 1.75rem;
  font-weight: 700;
  margin: 0 0 0.75rem;
  color: var(--bb-white);
  letter-spacing: -0.02em;
}

.bb-cta p {
  font-family: 'Inter', sans-serif;
  font-size: 1rem;
  color: rgba(255,255,255,0.7);
  margin: 0 0 2rem;
  font-weight: 300;
  line-height: 1.6;
  max-width: 520px;
  margin-left: auto;
  margin-right: auto;
  margin-bottom: 2rem;
}

.bb-btn-cta {
  display: inline-block;
  background: var(--bb-green-bright);
  color: var(--bb-white) !important;
  padding: 0.875rem 2.25rem;
  border-radius: 6px;
  font-family: 'Inter', sans-serif;
  font-weight: 600;
  font-size: 0.95rem;
  text-decoration: none !important;
  transition: all 0.25s ease;
  border: 2px solid var(--bb-green-bright);
}

.bb-btn-cta:hover {
  background: var(--bb-green-hover);
  border-color: var(--bb-green-hover);
  transform: translateY(-2px);
  box-shadow: 0 6px 20px rgba(45,95,63,0.35);
  color: var(--bb-white) !important;
}

/* ================================================================
   DESKTOP BREAKPOINT (769px and up)
   ================================================================ */

@media (min-width: 769px) {

  /* Hero — Desktop: wide, spacious */
  .bb-hero {
    padding: 6rem 2rem 5.5rem;
  }

  .bb-hero-inner {
    max-width: 900px;
  }

  .bb-hero h1 {
    font-size: 3.5rem;
    line-height: 1.12;
    letter-spacing: -0.03em;
  }

  .bb-hero-subtitle {
    font-size: 1.2rem;
    margin-bottom: 2.5rem;
    max-width: 640px;
  }

  .bb-hero-buttons {
    flex-direction: row;
  }

  .bb-btn-primary,
  .bb-btn-secondary {
    width: auto;
    max-width: none;
  }

  /* Metrics — Desktop */
  .bb-metrics {
    padding: 1.75rem 2rem;
  }

  .bb-metrics-inner {
    flex-direction: row;
    justify-content: center;
    gap: 3.5rem;
  }

  /* Image placeholder — Desktop: much wider */
  .bb-image-placeholder {
    padding: 5rem 3rem;
    margin: 3rem auto;
    max-width: 1200px;
  }

  /* Section — Desktop: wider container */
  .bb-section {
    padding: 5rem 3rem;
  }

  .bb-section-header {
    margin-bottom: 3.5rem;
  }

  .bb-section-header h2 {
    font-size: 2.25rem;
  }

  .bb-card-grid {
    grid-template-columns: repeat(3, 1fr);
    gap: 1.75rem;
  }

  .bb-card {
    padding: 2rem;
  }

  /* Split — Desktop: side by side */
  .bb-split {
    grid-template-columns: 1fr 1fr;
    margin: 0 auto 0;
    max-width: 1200px;
  }

  .bb-split-left {
    padding: 3.5rem 3rem;
  }

  .bb-split-right {
    padding: 3.5rem 3rem;
    border-top: 1px solid var(--bb-border);
    border-left: none;
  }

  .bb-split h2 {
    font-size: 1.5rem;
  }

  /* Story — Desktop: wider, side-by-side layout */
  .bb-story {
    padding: 5rem 3rem;
  }

  .bb-story h2 {
    font-size: 2.25rem;
    margin-bottom: 2.5rem;
  }

  .bb-story-layout {
    flex-direction: row;
    align-items: flex-start;
    gap: 3rem;
  }

  .bb-story-photo {
    width: 200px;
    height: 200px;
  }

  .bb-story-content p {
    font-size: 1rem;
  }

  /* CTA — Desktop */
  .bb-cta {
    padding: 5rem 2rem;
  }

  .bb-cta h2 {
    font-size: 2.5rem;
  }

  .bb-cta p {
    font-size: 1.1rem;
  }
}

/* ================================================================
   LARGE DESKTOP (1200px+)
   ================================================================ */

@media (min-width: 1200px) {
  .bb-hero {
    padding: 7rem 2rem 6.5rem;
  }

  .bb-hero h1 {
    font-size: 3.75rem;
  }

  .bb-hero-inner {
    max-width: 960px;
  }
}
</style>

<!-- Hero Section -->
<div class="bb-hero">
  <div class="bb-hero-inner">
    <div class="bb-hero-label">Student-Led Biotech Initiative</div>
    <h1>Bridging the Gap Between Curiosity and Careers in Biotechnology</h1>
    <p class="bb-hero-subtitle">Clear explanations, curated resources, and practical guidance for anyone exploring the world of biotech.</p>
    <div class="bb-hero-buttons">
      <a href="/what-is-biotech/" class="bb-btn-primary">Learn More</a>
      <a href="/career-pathways/" class="bb-btn-secondary">Explore Careers</a>
    </div>
  </div>
</div>

<!-- Metrics Bar -->
<div class="bb-metrics">
  <div class="bb-metrics-inner">
    <div class="bb-metric">
      <span class="bb-metric-num">10,000+</span>
      <span class="bb-metric-label">Students Reached</span>
    </div>
    <div class="bb-metric">
      <span class="bb-metric-num">6</span>
      <span class="bb-metric-label">Career Pathways</span>
    </div>
    <div class="bb-metric">
      <span class="bb-metric-num">100%</span>
      <span class="bb-metric-label">Free Core Resources</span>
    </div>
  </div>
</div>

<!-- Hero Image Placeholder -->
<div class="bb-image-placeholder">
  [PLACEHOLDER: Header Image - Biotechnology research visualization, such as a wide-angle photo of a modern biotech lab, DNA helix visualization, or students engaged in scientific work]
</div>

<!-- What BioBridge Offers -->
<div class="bb-section">
  <div class="bb-section-header">
    <h2>What BioBridge Offers</h2>
    <p>Clear explanations, curated resources, and honest guidance to help you navigate the world of biotechnology.</p>
  </div>
  <div class="bb-card-grid">
    <div class="bb-card">
      <div class="bb-card-number">01</div>
      <h3>Understand Biotech</h3>
      <p>Learn what biotechnology really is through real-world examples and plain-language explanations that make the science accessible.</p>
      <a href="/what-is-biotech/" class="bb-card-link">Explore the basics &rarr;</a>
    </div>
    <div class="bb-card">
      <div class="bb-card-number">02</div>
      <h3>Discover Careers</h3>
      <p>Explore the major career pathways in biotech with realistic entry points, salary expectations, and guidance for every background.</p>
      <a href="/career-pathways/" class="bb-card-link">View pathways &rarr;</a>
    </div>
    <div class="bb-card">
      <div class="bb-card-number">03</div>
      <h3>Access Resources</h3>
      <p>Browse curated newsletters, podcasts, courses, and books that are all free, beginner-friendly, and hand-picked for quality.</p>
      <a href="/resources/" class="bb-card-link">Browse resources &rarr;</a>
    </div>
  </div>
</div>

<!-- Problem / Solution Split -->
<div class="bb-split">
  <div class="bb-split-left">
    <h2>The Challenge</h2>
    <p>Biotechnology plays a growing role in how we treat disease, produce food, and respond to global challenges. But learning about it can feel overwhelming. Many students are interested in biotech yet don't know what it actually is, what jobs exist, or whether they belong in the field.</p>
  </div>
  <div class="bb-split-right">
    <h2>Our Approach</h2>
    <p>BioBridge is a student-led platform designed to make biotech more understandable and accessible through clear explanations, curated resources, and practical guidance. If you are curious but unsure where to begin, you are in the right place.</p>
  </div>
</div>

<!-- Founder Story -->
<div class="bb-story">
  <div class="bb-story-inner">
    <h2>The Story Behind BioBridge</h2>
    <div class="bb-story-layout">
      <div class="bb-story-photo-wrap">
        <img class="bb-story-photo" src="/assets/images/profile-photo.jpg" alt="Jean Tran, Founder of BioBridge">
      </div>
      <div class="bb-story-content">
        <p>I was certain I would become a doctor. In college, I completed the shadowing hours, prerequisites, and extracurriculars. But the closer I pushed myself toward a future in clinical work, the more I questioned whether it was actually right for me. I realized I needed a different direction.</p>
        <p>While searching for alternatives, I discovered my school offered a combined BS/MS in biotechnology that I could complete in four years. I knew almost nothing about biotech when I applied, but the program revealed just how expansive the field actually is: not just lab work, but business strategy, regulatory policy, manufacturing operations, and more.</p>
        <p>I started documenting what I was learning on social media, and the audience grew quickly. Tens of thousands of people followed along, and my messages became a constant stream of the same questions: What is biotech? How do I get in? Do I need a PhD? People were curious, but lacked a practical starting point. BioBridge is the resource I wish had existed when I was trying to figure it out.</p>
        <div class="bb-connect">
          <span class="bb-connect-label">Follow the journey:</span>
          <a href="https://instagram.com/jeans.scenes" target="_blank" class="bb-connect-link">
            <i class="fab fa-instagram"></i> Instagram
          </a>
          <a href="https://linkedin.com/in/jeantrann" target="_blank" class="bb-connect-link">
            <i class="fab fa-linkedin"></i> LinkedIn
          </a>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- Team Image Placeholder -->
<div class="bb-image-placeholder">
  [PLACEHOLDER: Team Photo - Group of diverse students in a lab setting, or a candid photo from a BioBridge event, workshop, or community gathering]
</div>

<!-- Bottom CTA -->
<div class="bb-cta">
  <h2>Ready to explore biotechnology?</h2>
  <p>Discover career pathways, free resources, and real guidance from someone who has been there.</p>
  <a href="/what-is-biotech/" class="bb-btn-cta">Learn More</a>
</div>
