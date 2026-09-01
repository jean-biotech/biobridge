---
layout: single
title: "Get Involved"
permalink: /get-involved/
---

<style>
@import url('https://fonts.googleapis.com/css2?family=Fraunces:ital,opsz,wght@0,9..144,400..600;1,9..144,400..600&family=Instrument+Sans:wght@400;500;600;700&display=swap');
body { font-family: 'Instrument Sans', -apple-system, BlinkMacSystemFont, sans-serif; }
h1, h2, h3 { font-family: 'Fraunces', Georgia, serif; }

:root {
  --bb-green: #24221A;
  --bb-green-accent: #5C6335;
  --bb-navy: #24221A;
  --bb-white: #EFE6D2;
  --bb-text-secondary: #5B5745;
  --bb-gray: #5B5745;
  --bb-border: rgba(36,34,26,0.12);
}

/* Involvement list: hanging numerals, grouped by space, no rules */
.bb-involve-grid {
  margin: 0 0 var(--s6);
  display: flex;
  flex-direction: column;
  gap: var(--s6);
}
.bb-involve-card {
  padding: 0;
  display: grid;
  grid-template-columns: 1fr;
}
.bb-involve-card .bb-card-num {
  display: block;
  font-family: 'Fraunces', Georgia, serif;
  font-size: 17px;
  font-weight: 500;
  color: var(--bb-navy);
  opacity: 0.45;
  margin-bottom: var(--s1);
}
.bb-involve-card h2 {
  font-family: 'Fraunces', Georgia, serif;
  color: var(--bb-navy);
  font-size: 30px;
  font-weight: 500;
  line-height: 1.2;
  margin-top: 0;
  margin-bottom: var(--s3);
}
.bb-involve-card p {
  color: var(--bb-text-secondary);
  opacity: 0.9;
  font-size: 17px;
  line-height: 1.6;
  max-width: var(--measure);
}
.bb-involve-card ul {
  color: var(--bb-text-secondary);
  opacity: 0.9;
  font-size: 17px;
  line-height: 1.6;
  padding-left: var(--s3);
  max-width: var(--measure);
}
.bb-involve-card li {
  margin-bottom: var(--s1);
}
.bb-involve-card em {
  color: var(--bb-gray);
  opacity: 0.8;
}

/* Contact section: left-aligned, rule-framed, no fill */
.bb-contact-section {
  border-top: 1px solid var(--bb-border);
  padding-top: var(--s4);
  margin-bottom: var(--s4);
}
.bb-contact-section h2 {
  font-family: 'Fraunces', Georgia, serif;
  color: var(--bb-navy);
  font-size: 30px;
  font-weight: 500;
  margin: 0 0 var(--s3);
}
.bb-contact-links {
  display: flex;
  gap: var(--s4);
  flex-wrap: wrap;
  margin-bottom: var(--s3);
}
.bb-contact-link {
  font-family: 'Instrument Sans', sans-serif;
  font-weight: 500;
  font-size: 17px;
  color: var(--bb-navy) !important;
}
.bb-feedback-note {
  color: var(--bb-gray);
  opacity: 0.8;
  font-family: 'Instrument Sans', sans-serif;
  font-size: 17px;
  line-height: 1.6;
  max-width: var(--measure);
}

/* Desktop */
@media (min-width: 769px) {
  .bb-involve-card h2 {
    font-size: 30px;
  }
}
</style>

<header class="bb-page-header">
  <span class="eyebrow">Join In</span>
  <h1>Get Involved with BioBridge</h1>
  <p class="bb-page-header__deck">BioBridge is a student-led initiative, and we are always looking for people who want to help make biotech more accessible.</p>
</header>

<div class="bb-involve-grid">

  <div class="bb-involve-card">
    <span class="bb-card-num">01</span>
    <h2>For Students</h2>
    <p><strong>Email signup:</strong> Get updates on new resources, mentorship opportunities, and events.</p>
    <p><strong>Interest form:</strong> Tell us what you are looking for and we will help connect you with resources.</p>
    <p><em>Forms are coming soon. For now, email us directly.</em></p>
  </div>

  <div class="bb-involve-card">
    <span class="bb-card-num">02</span>
    <h2>For Mentors</h2>
    <p>If you work in biotech and want to help students navigate the field, we would love to hear from you.</p>
    <p>We are building a mentorship program to connect curious students with professionals who remember what it was like to start.</p>
    <p><em>Mentor interest form (coming soon)</em></p>
  </div>

  <div class="bb-involve-card">
    <span class="bb-card-num">03</span>
    <h2>For Contributors</h2>
    <p>Have a resource, article, or story to share? Want to write a guest post about your biotech journey?</p>
    <p>We are always looking for:</p>
    <ul>
      <li>Beginner-friendly resources to add to our hub</li>
      <li>Career stories from diverse pathways</li>
      <li>Guest posts explaining biotech concepts</li>
      <li>Feedback on how to improve BioBridge</li>
    </ul>
  </div>

</div>

<div class="bb-contact-section">
  <h2>Stay Connected</h2>
  <div class="bb-contact-links">
    <a href="mailto:jeans.connects@gmail.com" class="bb-contact-link">jeans.connects@gmail.com</a>
    <a href="https://github.com/jean-biotech/biobridge" target="_blank" class="bb-contact-link">GitHub</a>
    <a href="https://linkedin.com/in/jeantrann" target="_blank" class="bb-contact-link">LinkedIn</a>
  </div>
  <p class="bb-feedback-note">See something that could be better? Have an idea for a new resource or page? We are constantly improving BioBridge based on feedback from students and professionals. Let us know what would make this more useful for you.</p>
</div>
