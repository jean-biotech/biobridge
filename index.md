---
layout: splash
title: " "
classes: wide
---

<style>
/* Import Fonts */
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=Poppins:wght@500;600;700&display=swap');

/* Apply Fonts Globally */
body {
  font-family: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
}

h1, h2, h3 {
  font-family: 'Poppins', sans-serif;
}

/* Hover Animations */
.card-hover {
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.card-hover:hover {
  transform: translateY(-4px);
  box-shadow: 0 6px 16px rgba(0,0,0,0.12) !important;
}

.btn-hover {
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.btn-hover:hover {
  transform: translateY(-2px);
  box-shadow: 0 4px 12px rgba(122, 155, 118, 0.3);
}

/* Pull Quote */
.pull-quote {
  background: linear-gradient(135deg, #7a9b76 0%, #6b8b67 100%);
  color: white;
  padding: 1.5rem 2rem;
  border-radius: 12px;
  margin: 2rem 0;
  border-left: 4px solid #5a7a56;
  font-size: 1.1rem;
  font-weight: 500;
  line-height: 1.7;
  font-style: italic;
}

/* Story Grid - Responsive */
.story-grid {
  display: grid;
  grid-template-columns: 220px 1fr;
  gap: 2.5rem;
  align-items: start;
}

@media (max-width: 768px) {
  .story-grid {
    grid-template-columns: 1fr;
    gap: 1.5rem;
  }
  
  .story-grid img {
    max-width: 200px;
    margin: 0 auto;
  }
}
</style>

<!-- Hero Section -->
<div class="card-hover" style="text-align: center; padding: 2rem 1.5rem; background: linear-gradient(135deg, #7a9b76 0%, #5a7a56 100%); color: white; margin: 1rem auto; max-width: 1200px; border-radius: 15px; box-shadow: 0 4px 12px rgba(0,0,0,0.15);">
  <h1 style="font-size: clamp(1.6rem, 5vw, 2.4rem); font-weight: 700; margin-bottom: 0.8rem; line-height: 1.3; letter-spacing: -0.02em;">Making Biotechnology Accessible to Everyone</h1>
  <p style="font-size: clamp(1rem, 3vw, 1.15rem); margin-bottom: 1.5rem; color: white; font-weight: 300; line-height: 1.6;">Your bridge into biotechnology starts here.</p>
  <a href="/what-is-biotech/" class="btn btn--primary btn--large btn-hover" style="background: white !important; color: #7a9b76 !important; font-weight: 600; padding: 0.85rem 2rem; font-size: clamp(0.95rem, 2.5vw, 1.05rem); display: inline-block;">Get Started</a>
</div>

<!-- Icon Grid Section -->
<div class="card-hover" style="padding: 2rem 1.5rem; background: white; margin: 1.5rem auto; max-width: 1000px; border-radius: 15px; box-shadow: 0 2px 8px rgba(0,0,0,0.08); border: 1px solid #e8e8e8;">
  <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(120px, 1fr)); gap: 2rem;">
    <div style="text-align: center;">
      <div style="font-size: 2.5rem; margin-bottom: 0.8rem;">🧬</div>
      <h3 style="color: #7a9b76; margin: 0; font-size: clamp(1rem, 3vw, 1.2rem); font-weight: 600; letter-spacing: -0.01em;">Learn Biotech</h3>
    </div>
    <div style="text-align: center;">
      <div style="font-size: 2.5rem; margin-bottom: 0.8rem;">🛤️</div>
      <h3 style="color: #7a9b76; margin: 0; font-size: clamp(1rem, 3vw, 1.2rem); font-weight: 600; letter-spacing: -0.01em;">Explore Careers</h3>
    </div>
    <div style="text-align: center;">
      <div style="font-size: 2.5rem; margin-bottom: 0.8rem;">📚</div>
      <h3 style="color: #7a9b76; margin: 0; font-size: clamp(1rem, 3vw, 1.2rem); font-weight: 600; letter-spacing: -0.01em;">Get Resources</h3>
    </div>
  </div>
</div>

<!-- Two-Column Section -->
<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 1.5rem; margin: 1.5rem auto; max-width: 1100px; padding: 0 1rem;">
  
  <div class="card-hover" style="background: white; padding: 2rem; border-radius: 12px; border: 1px solid #e8e8e8; box-shadow: 0 2px 6px rgba(0,0,0,0.05);">
    <h2 style="color: #7a9b76; font-size: clamp(1.25rem, 4vw, 1.5rem); margin-bottom: 1rem; font-weight: 700; letter-spacing: -0.02em; line-height: 1.3;">What is BioBridge?</h2>
    <p style="font-size: clamp(0.9rem, 2.5vw, 0.95rem); line-height: 2; color: #333; margin: 0; font-weight: 400;">BioBridge is a student-led platform designed to make biotech more understandable and accessible through clear explanations, curated resources, and honest guidance. If you're curious but unsure where to begin, you're in the right place.</p>
  </div>
  
  <div class="card-hover" style="background: white; padding: 2rem; border-radius: 12px; border: 1px solid #e8e8e8; box-shadow: 0 2px 6px rgba(0,0,0,0.05);">
    <h2 style="color: #7a9b76; font-size: clamp(1.25rem, 4vw, 1.5rem); margin-bottom: 1rem; font-weight: 700; letter-spacing: -0.02em; line-height: 1.3;">The Problem</h2>
    <p style="font-size: clamp(0.9rem, 2.5vw, 0.95rem); line-height: 2; color: #333; margin: 0; font-weight: 400;">Biotechnology plays a growing role in how we treat disease, produce food, and respond to global challenges, but learning about it can feel overwhelming at first. Many students are interested in biotech but don't know what it actually is, what jobs exist, or whether they belong in the field.</p>
  </div>

</div>

<!-- Why I Built This Section -->
<div class="card-hover" style="max-width: 1100px; margin: 1rem auto 2rem; padding: 2.5rem 2rem; background: #fafaf8; border-radius: 15px; border: 1px solid #e8e8e8; box-shadow: 0 2px 8px rgba(0,0,0,0.05);">
  
  <h2 style="color: #7a9b76; margin-bottom: 2rem; font-size: clamp(1.4rem, 4vw, 1.8rem); font-weight: 700; letter-spacing: -0.02em; line-height: 1.3;">Why I Built This</h2>
  
  <div class="story-grid">
    
    <div>
      <img src="/assets/images/profile-photo.jpg" alt="Profile Photo" style="width: 100%; border-radius: 12px; box-shadow: 0 4px 12px rgba(0,0,0,0.12);">
    </div>
    
    <div>
      <p style="font-size: clamp(0.9rem, 2.5vw, 0.95rem); line-height: 2; color: #333; margin-bottom: 1.5rem; font-weight: 400;">I was certain I'd become a doctor. In college, I even completed the shadowing hours, prerequisites, and extracurriculars. But the closer I pushed myself to a future in clinical work, the more I questioned whether it was actually right for me and I realized I needed a different direction.</p>
      
      <p style="font-size: clamp(0.9rem, 2.5vw, 0.95rem); line-height: 2; color: #333; margin-bottom: 1.5rem; font-weight: 400;">While anxiously searching for alternatives, I discovered my school offered a combined BS/MS in biotechnology that I could complete in four years. I knew almost nothing about biotech when I applied, but the program revealed just how expansive the field actually is—not
