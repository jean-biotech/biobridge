---
layout: splash
title: " "
classes: wide
---

<style>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=Poppins:wght@500;600;700;800&display=swap');

body { font-family: 'Inter', sans-serif; }
h1, h2, h3, h4 { font-family: 'Poppins', sans-serif; }

/* ── Hero ── */
.bb-hero {
  background: linear-gradient(135deg, #064e3b 0%, #047857 50%, #065f46 100%);
  color: #ffffff;
  text-align: center;
  padding: 5rem 2rem 4.5rem;
  position: relative;
  overflow: hidden;
}
.bb-hero::before {
  content: '';
  position: absolute;
  top: -50%;
  left: -50%;
  width: 200%;
  height: 200%;
  background: radial-gradient(circle at 30% 70%, rgba(16,185,129,0.15) 0%, transparent 50%),
              radial-gradient(circle at 70% 30%, rgba(217,119,6,0.08) 0%, transparent 50%);
  pointer-events: none;
}
.bb-hero-inner {
  max-width: 800px;
  margin: 0 auto;
  position: relative;
  z-index: 1;
}
.bb-hero h1 {
  font-size: 3.5rem;
  font-weight: 800;
  line-height: 1.15;
  margin: 0 0 1.25rem;
  letter-spacing: -0.03em;
  color: #ffffff;
}
.bb-hero p {
  font-size: 1.25rem;
  font-weight: 300;
  color: rgba(255,255,255,0.85);
  margin: 0 0 2.5rem;
  line-height: 1.6;
}
.bb-hero-buttons {
  display: flex;
  gap: 1rem;
  justify-content: center;
  flex-wrap: wrap;
}
.bb-btn-gold {
  display: inline-block;
  background: #d97706;
  color: #ffffff !important;
  padding: 0.875rem 2.25rem;
  border-radius: 8px;
  font-weight: 600;
  font-size: 1.05rem;
  text-decoration: none !important;
  transition: all 0.2s ease;
  border: 2px solid #d97706;
}
.bb-btn-gold:hover {
  background: #b45309;
  border-color: #b45309;
  transform: translateY(-2px);
  box-shadow: 0 6px 20px rgba(217,119,6,0.35);
  color: #ffffff !important;
}
.bb-btn-outline {
  display: inline-block;
  background: transparent;
  color: #ffffff !important;
  padding: 0.875rem 2.25rem;
  border-radius: 8px;
  font-weight: 600;
  font-size: 1.05rem;
  text-decoration: none !important;
  transition: all 0.2s ease;
  border: 2px solid rgba(255,255,255,0.4);
}
.bb-btn-outline:hover {
  background: rgba(255,255,255,0.1);
  border-color: rgba(255,255,255,0.7);
  color: #ffffff !important;
}

/* ── Social Proof ── */
.bb-proof {
  background: #f0fdf4;
  padding: 1.5rem 2rem;
  text-align: center;
  border-bottom: 1px solid #e2e8f0;
}
.bb-proof-inner {
  max-width: 900px;
  margin: 0 auto;
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 2.5rem;
  flex-wrap: wrap;
}
.bb-proof-item {
  display: flex;
  align-items: center;
  gap: 0.5rem;
  font-size: 0.95rem;
  color: #064e3b;
  font-weight: 500;
}
.bb-proof-item .num {
  font-family: 'Poppins', sans-serif;
  font-weight: 700;
  font-size: 1.15rem;
  color: #047857;
}

/* ── Pillars / Features ── */
.bb-pillars {
  padding: 4.5rem 2rem;
  max-width: 1100px;
  margin: 0 auto;
}
.bb-pillars-header {
  text-align: center;
  margin-bottom: 3rem;
}
.bb-pillars-header h2 {
  color: #064e3b;
  font-size: 2rem;
  font-weight: 700;
  margin: 0 0 0.75rem;
  letter-spacing: -0.02em;
}
.bb-pillars-header p {
  color: #64748b;
  font-size: 1.05rem;
  margin: 0;
}
.bb-pillars-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 2rem;
}
.bb-pillar-card {
  background: #ffffff;
  border: 1px solid #e2e8f0;
  border-left: 4px solid #10b981;
  border-radius: 10px;
  padding: 2rem 1.75rem;
  transition: all 0.2s ease;
}
.bb-pillar-card:hover {
  box-shadow: 0 8px 24px rgba(0,0,0,0.06);
  transform: translateY(-2px);
}
.bb-pillar-card .card-num {
  display: inline-block;
  background: #f0fdf4;
  color: #047857;
  font-family: 'Poppins', sans-serif;
  font-weight: 700;
  font-size: 0.85rem;
  width: 32px;
  height: 32px;
  line-height: 32px;
  text-align: center;
  border-radius: 8px;
  margin-bottom: 1rem;
}
.bb-pillar-card h3 {
  color: #064e3b;
  font-size: 1.25rem;
  font-weight: 600;
  margin: 0 0 0.75rem;
}
.bb-pillar-card p {
  color: #475569;
  font-size: 0.95rem;
  line-height: 1.7;
  margin: 0 0 1rem;
}
.bb-pillar-card a {
  color: #d97706;
  font-weight: 600;
  font-size: 0.9rem;
  text-decoration: none;
}
.bb-pillar-card a:hover {
  color: #b45309;
  text-decoration: underline;
}

/* ── Problem / Solution ── */
.bb-split {
  display: grid;
  grid-template-columns: 1fr 1fr;
  max-width: 1100px;
  margin: 0 auto 4rem;
  border-radius: 14px;
  overflow: hidden;
  box-shadow: 0 4px 16px rgba(0,0,0,0.08);
}
.bb-split-problem {
  background: #064e3b;
  color: #ffffff;
  padding: 3rem 2.5rem;
}
.bb-split-solution {
  background: #ffffff;
  padding: 3rem 2.5rem;
  border: 1px solid #e2e8f0;
  border-left: none;
}
.bb-split h2 {
  font-size: 1.5rem;
  font-weight: 700;
  margin: 0 0 1.25rem;
  letter-spacing: -0.01em;
}
.bb-split-problem h2 {
  color: #fcd34d;
}
.bb-split-solution h2 {
  color: #064e3b;
}
.bb-split p {
  font-size: 1rem;
  line-height: 1.8;
  margin: 0;
}
.bb-split-problem p {
  color: rgba(255,255,255,0.88);
}
.bb-split-solution p {
  color: #475569;
}

/* ── Founder Story ── */
.bb-story {
  background: #f8fafc;
  padding: 4.5rem 2rem;
  border-top: 1px solid #e2e8f0;
  border-bottom: 1px solid #e2e8f0;
}
.bb-story-inner {
  max-width: 1000px;
  margin: 0 auto;
}
.bb-story h2 {
  color: #064e3b;
  font-size: 2rem;
  font-weight: 700;
  margin: 0 0 2.5rem;
  letter-spacing: -0.02em;
}
.bb-story-grid {
  display: grid;
  grid-template-columns: 200px 1fr;
  gap: 2.5rem;
  align-items: start;
}
.bb-story-photo {
  width: 100%;
  border-radius: 14px;
  box-shadow: 0 4px 16px rgba(0,0,0,0.1);
}
.bb-story-text p {
  font-size: 1rem;
  line-height: 1.85;
  color: #334155;
  margin: 0 0 1.25rem;
}
.bb-social-links {
  margin-top: 1.75rem;
  padding-top: 1.75rem;
  border-top: 1px solid #e2e8f0;
  display: flex;
  align-items: center;
  gap: 1.25rem;
  flex-wrap: wrap;
}
.bb-social-links strong {
  color: #0f172a;
  font-size: 0.95rem;
}
.bb-social-link {
  display: inline-flex;
  align-items: center;
  gap: 0.4rem;
  text-decoration: none !important;
  font-size: 0.95rem;
  font-weight: 500;
  color: #475569 !important;
  padding: 0.4rem 0.75rem;
  border-radius: 6px;
  border: 1px solid #e2e8f0;
  transition: all 0.2s ease;
}
.bb-social-link:hover {
  background: #f0fdf4;
  border-color: #10b981;
  color: #064e3b !important;
}

/* ── Bottom CTA ── */
.bb-cta-banner {
  background: linear-gradient(135deg, #064e3b 0%, #047857 100%);
  color: #ffffff;
  text-align: center;
  padding: 4rem 2rem;
}
.bb-cta-banner h2 {
  font-size: 2.25rem;
  font-weight: 700;
  margin: 0 0 1rem;
  color: #ffffff;
  letter-spacing: -0.02em;
}
.bb-cta-banner p {
  font-size: 1.1rem;
  color: rgba(255,255,255,0.8);
  margin: 0 0 2rem;
  font-weight: 300;
}

/* ── Mobile Responsive ── */
@media (max-width: 768px) {
  .bb-hero {
    padding: 3rem 1.5rem 2.5rem;
  }
  .bb-hero h1 {
    font-size: 2rem;
  }
  .bb-hero p {
    font-size: 1.05rem;
  }
  .bb-hero-buttons {
    flex-direction: column;
    align-items: center;
  }
  .bb-btn-gold, .bb-btn-outline {
    width: 100%;
    max-width: 280px;
    text-align: center;
  }

  .bb-proof-inner {
    flex-direction: column;
    gap: 0.75rem;
  }

  .bb-pillars {
    padding: 3rem 1.25rem;
  }
  .bb-pillars-grid {
    grid-template-columns: 1fr;
    gap: 1.25rem;
  }

  .bb-split {
    grid-template-columns: 1fr;
    margin: 0 1rem 3rem;
  }
  .bb-split-problem, .bb-split-solution {
    padding: 2rem 1.5rem;
  }
  .bb-split-solution {
    border-left: 1px solid #e2e8f0;
  }

  .bb-story {
    padding: 3rem 1.25rem;
  }
  .bb-story-grid {
    grid-template-columns: 1fr;
    gap: 1.5rem;
  }
  .bb-story-photo {
    width: 160px;
    margin: 0 auto;
    display: block;
  }
  .bb-story-text p {
    font-size: 0.95rem;
  }

  .bb-cta-banner {
    padding: 3rem 1.5rem;
  }
  .bb-cta-banner h2 {
    font-size: 1.6rem;
  }
}
</style>

<!-- Hero Section -->
<div class="bb-hero">
  <div class="bb-hero-inner">
    <h1>Making Biotechnology Accessible to Everyone</h1>
    <p>Your bridge into biotechnology starts here.</p>
    <div class="bb-hero-buttons">
      <a href="/what-is-biotech/" class="bb-btn-gold">Get Started</a>
      <a href="/career-pathways/" class="bb-btn-outline">Explore Careers</a>
    </div>
  </div>
</div>

<!-- Social Proof Bar -->
<div class="bb-proof">
  <div class="bb-proof-inner">
    <div class="bb-proof-item">
      <span class="num">10,000+</span> students reached
    </div>
    <div class="bb-proof-item">
      <span class="num">6</span> career pathways mapped
    </div>
    <div class="bb-proof-item">
      <span class="num">100%</span> free core resources
    </div>
  </div>
</div>

<!-- Three Pillars Section -->
<div class="bb-pillars">
  <div class="bb-pillars-header">
    <h2>What BioBridge Offers</h2>
    <p>Clear explanations, curated resources, and honest guidance into biotech.</p>
  </div>
  <div class="bb-pillars-grid">
    <div class="bb-pillar-card">
      <div class="card-num">01</div>
      <h3>Learn Biotech</h3>
      <p>Understand what biotechnology really is through real-world examples and plain-language explanations.</p>
      <a href="/what-is-biotech/">Learn more &rarr;</a>
    </div>
    <div class="bb-pillar-card">
      <div class="card-num">02</div>
      <h3>Explore Careers</h3>
      <p>Discover the major career pathways in biotech with realistic entry points for every background.</p>
      <a href="/career-pathways/">Learn more &rarr;</a>
    </div>
    <div class="bb-pillar-card">
      <div class="card-num">03</div>
      <h3>Get Resources</h3>
      <p>Access curated newsletters, podcasts, courses, and books that are all beginner-friendly.</p>
      <a href="/resources/">Learn more &rarr;</a>
    </div>
  </div>
</div>

<!-- Problem / Solution Split -->
<div class="bb-split">
  <div class="bb-split-problem">
    <h2>The Problem</h2>
    <p>Biotechnology plays a growing role in how we treat disease, produce food, and respond to global challenges, but learning about it can feel overwhelming at first. Many students are interested in biotech but don't know what it actually is, what jobs exist, or whether they belong in the field.</p>
  </div>
  <div class="bb-split-solution">
    <h2>What is BioBridge?</h2>
    <p>BioBridge is a student-led platform designed to make biotech more understandable and accessible through clear explanations, curated resources, and honest guidance. If you're curious but unsure where to begin, you're in the right place.</p>
  </div>
</div>

<!-- Founder Story -->
<div class="bb-story">
  <div class="bb-story-inner">
    <h2>Why I Built This</h2>
    <div class="bb-story-grid">
      <div>
        <img class="bb-story-photo" src="/assets/images/profile-photo.jpg" alt="Profile Photo">
      </div>
      <div class="bb-story-text">
        <p>I was certain I'd become a doctor. In college, I even completed the shadowing hours, prerequisites, and extracurriculars. But the closer I pushed myself to a future in clinical work, the more I questioned whether it was actually right for me and I realized I needed a different direction.</p>
        <p>While anxiously searching for alternatives, I discovered my school offered a combined BS/MS in biotechnology that I could complete in four years. I knew almost nothing about biotech when I applied, but the program revealed just how expansive the field actually is—not just lab work, but business strategy, regulatory policy, manufacturing operations, and more.</p>
        <p>I started documenting what I was learning on social media, and the audience grew fast. Tens of thousands of people, and my DMs turned into a constant stream of the same questions: What is biotech? How do I break in? Do I need a PhD? People were curious, but lacked a practical starting point. So, I built BioBridge as the resource I wish had existed when I was trying to figure it out.</p>
        <div class="bb-social-links">
          <strong>Follow the journey:</strong>
          <a href="https://instagram.com/jeans.scenes" target="_blank" class="bb-social-link">
            <span style="color: #E4405F;"><i class="fab fa-instagram"></i></span> Instagram
          </a>
          <a href="https://linkedin.com/in/jeantrann" target="_blank" class="bb-social-link">
            <span style="color: #0A66C2;"><i class="fab fa-linkedin"></i></span> LinkedIn
          </a>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- Bottom CTA Banner -->
<div class="bb-cta-banner">
  <h2>Ready to start your biotech journey?</h2>
  <p>Explore career pathways, free resources, and real guidance from someone who's been there.</p>
  <a href="/what-is-biotech/" class="bb-btn-gold">Get Started Now</a>
</div>
