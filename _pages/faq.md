---
layout: single
title: "FAQ"
permalink: /faq/
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

/* Accordion container */
.bb-accordion {
  max-width: 760px;
  margin: 0 auto;
}

/* Individual accordion item */
.bb-accordion-item {
  border: 1px solid var(--bb-border);
  border-radius: 8px;
  margin-bottom: 0.75rem;
  background: var(--bb-white);
  overflow: hidden;
  transition: box-shadow 0.2s ease;
}
.bb-accordion-item.open {
  box-shadow: 0 4px 16px rgba(0,0,0,0.07);
}

/* Question button */
.bb-accordion-btn {
  width: 100%;
  text-align: left;
  background: none;
  border: none;
  padding: 1.1rem 1.25rem;
  cursor: pointer;
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 1rem;
  font-family: 'Inter', sans-serif;
  font-size: 0.97rem;
  font-weight: 600;
  color: var(--bb-navy);
  line-height: 1.45;
  transition: background 0.15s ease;
}
.bb-accordion-btn:hover {
  background: var(--bb-green-bg-subtle);
}
.bb-accordion-item.open .bb-accordion-btn {
  background: var(--bb-green-bg-subtle);
  color: var(--bb-green);
}

/* Chevron icon */
.bb-chevron {
  flex-shrink: 0;
  width: 20px;
  height: 20px;
  border: 1.5px solid var(--bb-border);
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  transition: all 0.25s ease;
  color: var(--bb-gray);
  font-size: 0.75rem;
}
.bb-accordion-item.open .bb-chevron {
  background: var(--bb-green-accent);
  border-color: var(--bb-green-accent);
  color: var(--bb-white);
  transform: rotate(180deg);
}

/* Answer panel */
.bb-accordion-panel {
  max-height: 0;
  overflow: hidden;
  transition: max-height 0.35s ease, padding 0.25s ease;
}
.bb-accordion-item.open .bb-accordion-panel {
  max-height: 1000px;
}

/* Answer content */
.bb-accordion-body {
  padding: 0 1.25rem 1.25rem;
  border-top: 1px solid var(--bb-border);
}
.bb-accordion-body p {
  color: var(--bb-text-secondary);
  font-size: 0.93rem;
  line-height: 1.85;
  margin: 0.85rem 0 0;
}
.bb-accordion-body p + p {
  margin-top: 0.75rem;
}
.bb-accordion-body a {
  color: var(--bb-green-accent);
  font-weight: 600;
  text-decoration: none;
}
.bb-accordion-body a:hover { text-decoration: underline; }
.bb-accordion-body strong {
  color: var(--bb-navy);
  font-weight: 600;
}

/* Desktop */
@media (min-width: 769px) {
  .bb-page-hero { padding: 3.5rem 3rem; border-radius: 12px; }
  .bb-page-hero h1 { font-size: 2.25rem; }
  .bb-page-hero p { font-size: 1.1rem; }
  .bb-accordion-btn { font-size: 1rem; padding: 1.2rem 1.5rem; }
  .bb-accordion-body { padding: 0 1.5rem 1.5rem; }
}
</style>

<div class="bb-page-hero">
  <h1>Frequently Asked Questions</h1>
  <p>Common questions from people just starting to explore biotechnology. Click any question to expand the answer.</p>
</div>

<div class="bb-accordion" id="bb-accordion">

  <div class="bb-accordion-item">
    <button class="bb-accordion-btn" aria-expanded="false">
      <span>I'm in high school. Where do I start?</span>
      <span class="bb-chevron">&#9660;</span>
    </button>
    <div class="bb-accordion-panel">
      <div class="bb-accordion-body">
        <p>Start by building a picture of what the field actually is — the <a href="/what-is-biotech/">What is Biotech?</a> page is a good first stop. From there, browse the <a href="/career-pathways/">Career Pathways</a> to see the kinds of roles that exist, because knowing where you might land helps you figure out what to pursue now.</p>
        <p>Beyond that: follow biotech news to stay curious (our <a href="/resources/">Learning Lab</a> has good podcast and newsletter picks for beginners), take AP Biology or chemistry if your school offers it, and look into summer programs or science competitions in your area. You have more time than you think, and the most useful thing you can do right now is stay engaged and explore widely.</p>
      </div>
    </div>
  </div>

  <div class="bb-accordion-item">
    <button class="bb-accordion-btn" aria-expanded="false">
      <span>I'm in college but not majoring in biology. Can I still get into biotech?</span>
      <span class="bb-chevron">&#9660;</span>
    </button>
    <div class="bb-accordion-panel">
      <div class="bb-accordion-body">
        <p>Absolutely — and this is one of the most important things to understand about biotech. The industry needs engineers for process development and manufacturing, computer scientists for bioinformatics and data analysis, business majors for operations and strategy, and communications people for science writing and marketing. A biology degree is one path in, not the only one.</p>
        <p>The key is connecting whatever you're studying to a real role. Check out the <a href="/career-pathways/">Career Pathways</a> page to see the non-research tracks — you'll likely find something that maps naturally to your current major.</p>
      </div>
    </div>
  </div>

  <div class="bb-accordion-item">
    <button class="bb-accordion-btn" aria-expanded="false">
      <span>I'm changing careers. Is it too late?</span>
      <span class="bb-chevron">&#9660;</span>
    </button>
    <div class="bb-accordion-panel">
      <div class="bb-accordion-body">
        <p>Not at all. People enter biotech in their 30s, 40s, and beyond — often in roles where their previous experience is exactly what's needed. Someone with a legal background is well-positioned for regulatory affairs. A project manager from any industry can move into clinical operations or manufacturing. Someone with sales experience can transition into biotech sales or business development without starting from scratch.</p>
        <p>The honest truth is that most biotech employers value problem-solving ability and relevant transferable skills more than a specific degree. What matters is being able to demonstrate that you understand the context and that you're committed to building the specific knowledge gaps. Online courses and industry certifications can help close those gaps faster than you'd expect.</p>
      </div>
    </div>
  </div>

  <div class="bb-accordion-item">
    <button class="bb-accordion-btn" aria-expanded="false">
      <span>I don't have a science background. Can I still learn?</span>
      <span class="bb-chevron">&#9660;</span>
    </button>
    <div class="bb-accordion-panel">
      <div class="bb-accordion-body">
        <p>Yes — and this entire website is built with you in mind. You don't need prior science knowledge to explore what biotech is or to understand the career landscape. The <a href="/what-is-biotech/">What is Biotech?</a> page starts from zero, and the <a href="/resources/">Learning Lab</a> has podcasts and YouTube channels designed for curious non-specialists.</p>
        <p>You also don't need to become a scientist to work in biotech. Many of the people keeping this industry running have backgrounds in law, business, communications, or engineering. The field is much broader than most people realize, and scientific literacy — not a science degree — is usually what's required for most of those roles.</p>
      </div>
    </div>
  </div>

  <div class="bb-accordion-item">
    <button class="bb-accordion-btn" aria-expanded="false">
      <span>What is the job market like?</span>
      <span class="bb-chevron">&#9660;</span>
    </button>
    <div class="bb-accordion-panel">
      <div class="bb-accordion-body">
        <p>Biotech is one of the faster-growing sectors in the economy, though like any industry it goes through cycles. Manufacturing and quality roles have remained consistently in demand. The growth of computational biology has created strong need for people with data and programming skills. Regulatory and compliance positions have grown alongside the increasing complexity of the approval process.</p>
        <p>Entry-level salaries generally range from $50k–$80k depending on role and location, with significant variation. Lab-based roles in lower cost-of-living areas often sit at the lower end; data and engineering roles in Boston or the Bay Area tend to sit higher. The important thing to know is that there are entry points at nearly every education level, and the field rewards people who stay curious and keep building expertise.</p>
      </div>
    </div>
  </div>

  <div class="bb-accordion-item">
    <button class="bb-accordion-btn" aria-expanded="false">
      <span>Do I need to live in a biotech hub?</span>
      <span class="bb-chevron">&#9660;</span>
    </button>
    <div class="bb-accordion-panel">
      <div class="bb-accordion-body">
        <p>It helps, especially early in your career when proximity to other people in the industry accelerates learning and networking. The major hubs — Boston/Cambridge, the San Francisco Bay Area, San Diego, Research Triangle in North Carolina, and Seattle — have the highest concentration of companies and therefore the most entry-level opportunities.</p>
        <p>That said, biotech companies exist in most mid-to-large cities, and remote work is increasingly common for non-lab roles like regulatory affairs, business development, and project management. If relocating isn't possible, it's worth identifying what's local and being strategic about which roles allow more flexibility.</p>
      </div>
    </div>
  </div>

  <div class="bb-accordion-item">
    <button class="bb-accordion-btn" aria-expanded="false">
      <span>How do I get my first internship or job?</span>
      <span class="bb-chevron">&#9660;</span>
    </button>
    <div class="bb-accordion-panel">
      <div class="bb-accordion-body">
        <p>For students, the most underused path is cold outreach — sending a short, specific email to a professor or researcher asking if there's an opportunity to get involved with their lab. Most people don't do this, which means the ones who do stand out. Summer research programs (REUs for undergrads, company internships for anyone) are also worth applying to broadly, since rejection rates are high but so are the payoffs. Joining biotech-focused student groups at your school helps too, mostly because it puts you in rooms with people who share the goal.</p>
        <p>For career changers, the path usually runs through LinkedIn networking and contract or temp positions. A contract role at a biotech company — even one that isn't your dream job — gives you the industry experience on your resume that opens the next door. Highlighting transferable skills clearly and honestly, and taking a free or low-cost online course to show genuine interest in the specific area, goes a long way.</p>
      </div>
    </div>
  </div>

  <div class="bb-accordion-item">
    <button class="bb-accordion-btn" aria-expanded="false">
      <span>What skills should I focus on building?</span>
      <span class="bb-chevron">&#9660;</span>
    </button>
    <div class="bb-accordion-panel">
      <div class="bb-accordion-body">
        <p>The skills that matter most depend on the path you're aiming for, but a few are broadly valuable across almost every biotech role. Data fluency — even at a basic level, with Excel or Python — is increasingly expected. Clear writing and communication are rare and consistently valued. Understanding the regulatory landscape (FDA, GMP, GLP basics) is relevant to far more roles than just regulatory affairs.</p>
        <p>Scientific literacy — the ability to read a paper, follow a technical argument, and understand what a study is actually claiming — is the underlying skill that compounds over time regardless of your specific role. The <a href="/resources/">Learning Lab</a> has resources to help build all of these, most of them free.</p>
      </div>
    </div>
  </div>

  <div class="bb-accordion-item">
    <button class="bb-accordion-btn" aria-expanded="false">
      <span>I have more questions. How can I get help?</span>
      <span class="bb-chevron">&#9660;</span>
    </button>
    <div class="bb-accordion-panel">
      <div class="bb-accordion-body">
        <p><a href="/get-involved/">Get in touch</a> — we're building a mentorship program and are happy to point you toward the right resources for your specific situation. You can also email us directly at <a href="mailto:contact@biobridge.org">contact@biobridge.org</a>.</p>
      </div>
    </div>
  </div>

</div>

<script>
(function() {
  var items = document.querySelectorAll('.bb-accordion-item');
  items.forEach(function(item) {
    var btn = item.querySelector('.bb-accordion-btn');
    btn.addEventListener('click', function() {
      var isOpen = item.classList.contains('open');
      // Toggle this item (allow multiple open simultaneously)
      item.classList.toggle('open');
      btn.setAttribute('aria-expanded', !isOpen);
    });
  });
})();
</script>
