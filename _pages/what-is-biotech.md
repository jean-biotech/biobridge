---
layout: single
title: "What is Biotech?"
permalink: /what-is-biotech/
toc: true
toc_label: "On This Page"
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

/* Image Placeholder */
.bb-img-placeholder {
  background: linear-gradient(135deg, var(--bb-teal-bg), #e8f4f5);
  border: 2px dashed var(--bb-border);
  border-radius: 10px;
  padding: 2.5rem 1.5rem;
  text-align: center;
  color: var(--bb-gray);
  font-family: 'Inter', sans-serif;
  font-size: 0.85rem;
  font-weight: 500;
  line-height: 1.5;
  margin: 2rem 0;
}

/* Example Cards Grid — Mobile First */
.bb-example-grid {
  display: grid;
  grid-template-columns: 1fr;
  gap: 1.25rem;
  margin: 2rem 0;
}
.bb-example-card {
  background: var(--bb-white);
  border: 1px solid var(--bb-border);
  border-radius: 8px;
  padding: 1.75rem 1.5rem;
  transition: all 0.25s ease;
}
.bb-example-card:hover {
  box-shadow: 0 4px 16px rgba(0,0,0,0.08);
  transform: translateY(-1px);
}
.bb-example-card h3 {
  font-family: 'Inter', sans-serif;
  color: var(--bb-navy);
  margin-top: 0;
  font-size: 1.05rem;
  font-weight: 600;
  padding-bottom: 0.75rem;
  border-bottom: 2px solid var(--bb-teal-bg);
  margin-bottom: 0.75rem;
}
.bb-example-card p {
  color: var(--bb-text-secondary);
  font-size: 0.92rem;
  line-height: 1.75;
}

/* Misconception Blocks */
.bb-misconception {
  background: var(--bb-off-white);
  border: 1px solid var(--bb-border);
  border-left: 3px solid var(--bb-teal);
  border-radius: 8px;
  padding: 1.5rem;
  margin-bottom: 1rem;
}
.bb-misconception strong {
  color: var(--bb-navy);
  font-family: 'Inter', sans-serif;
  font-size: 0.95rem;
}
.bb-misconception p {
  color: var(--bb-text-secondary);
  margin: 0.5rem 0 0;
  font-size: 0.92rem;
  line-height: 1.75;
}

/* Section Text */
.bb-section-text p {
  color: #334155;
  font-size: 0.95rem;
  line-height: 1.85;
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
  .bb-example-grid {
    grid-template-columns: repeat(2, 1fr);
    gap: 1.5rem;
  }
  .bb-img-placeholder {
    padding: 3.5rem 2.5rem;
  }
}
</style>

<div class="bb-page-hero">
  <h1>What is Biotechnology, Really?</h1>
  <p>Understanding the science that is shaping our future, in plain language.</p>
</div>

<div class="bb-img-placeholder">
  [PLACEHOLDER: Hero Image - A striking visual of biotechnology in action, such as a modern lab with researchers, microscopy imagery, or a DNA double helix visualization]
</div>

Biotechnology is using living systems -- cells, bacteria, proteins, DNA -- to create useful products or solve problems.

If that sounds vague, it is because biotech is **incredibly broad**. It touches medicine, agriculture, environmental science, manufacturing, and more.

---

## Real-World Examples

Instead of abstract definitions, here are examples of how biotech is applied in practice.

<div class="bb-example-grid">

  <div class="bb-example-card">
    <h3>Medicine</h3>
    <p><strong>Did you know</strong> the insulin keeping millions of diabetics alive is made by bacteria? Scientists insert the human insulin gene into E. coli to create tiny living factories churning out life-saving medicine.</p>
    <p>Or consider <strong>CAR-T therapy</strong>, a treatment for cancer. Doctors extract your immune cells, genetically reprogram them to recognize cancer, and inject them back into you. Your own cells become trained to fight tumors.</p>
  </div>

  <div class="bb-example-card">
    <h3>Agriculture</h3>
    <p><strong>Drought-resistant crops</strong> can survive on 30% less water. In regions facing water scarcity, this is not just innovation -- it is survival.</p>
    <p><strong>The plant-based meat revolution</strong> relies on heme, a protein made by engineered yeast. It is what makes Impossible meat taste remarkably similar to beef.</p>
  </div>

  <div class="bb-example-card">
    <h3>Environment</h3>
    <p><strong>Bacteria that eat oil spills.</strong> Bioremediation uses microbes that break down petroleum into harmless compounds, turning environmental disasters into manageable cleanups.</p>
    <p><strong>Bioplastics decompose in months, not centuries.</strong> Made from plants instead of petroleum, they could replace traditional plastics in packaging, utensils, and more.</p>
  </div>

  <div class="bb-example-card">
    <h3>Cutting Edge</h3>
    <p><strong>Bioprinting organs is happening now.</strong> Researchers use 3D printers loaded with living cells to build skin grafts, cartilage, and blood vessels.</p>
    <p><strong>Brain organoids</strong> -- mini-brains grown from stem cells in a lab -- are helping scientists study Alzheimer's, test new drugs, and understand brain development without human trials.</p>
  </div>

</div>

---

## Beyond the Science

<div class="bb-section-text" markdown="1">

A breakthrough in the lab is just the beginning. Getting it from concept to the real world takes an entire team of people who are not scientists.

Take mRNA vaccines. The science behind them existed for decades, but turning that research into something that reached billions of people took work beyond the lab.

You need business strategists to decide what is worth pursuing and who will pay for it. You need regulatory experts to design safe trials and navigate the FDA. You need engineers to figure out how to manufacture at scale without losing quality.

Someone has to ask the hard questions: Should we edit human genes? Who gets access? What could go wrong? That is policy and ethics. You also need communicators who can explain a new technology to a skeptical public.

Every major biotech breakthrough follows this pattern. Science is step one, and everything else is steps two through twenty. That is why biotech needs business strategists, engineers, lawyers, writers, ethicists, and project managers just as much as it needs scientists.

</div>

---

## Common Misconceptions

<div class="bb-misconception">
  <strong>"You need to be good at biology to work in the industry."</strong>
  <p>Not necessarily. If you can explain complex ideas simply, you could do science communication. If you are good with numbers and logistics, there is operations. Biotech employs humanities majors, business students, and engineers just as much as biology PhDs.</p>
</div>

<div class="bb-misconception">
  <strong>"It is all lab work."</strong>
  <p>Lab work is one part. There is also manufacturing, regulatory affairs, sales, policy, data analysis, and more. Check out <a href="/career-pathways/" style="color: #0d7377; font-weight: 600;">Career Pathways</a> for additional information.</p>
</div>

<div class="bb-misconception">
  <strong>"You need a PhD."</strong>
  <p>Only if you want to lead research. Most biotech jobs in regulatory, manufacturing, business, and operations require a bachelor's degree or less. Some roles require only a high school diploma and training. Certificate programs take months, not years. There are entry points at every level, and you can build a rewarding career without ever going back to school.</p>
</div>
