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
  --bb-gray: #757575;
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

/* Image Placeholder */
.bb-img-placeholder {
  background: linear-gradient(135deg, var(--bb-green-bg), #e8f4f5);
  border: 2px dashed var(--bb-border);
  border-radius: 10px;
  padding: 2rem 1.5rem;
  text-align: center;
  color: var(--bb-gray);
  font-family: 'Inter', sans-serif;
  font-size: 0.82rem;
  font-weight: 500;
  line-height: 1.5;
}

/* Pull quote / callout box */
.bb-callout {
  background: var(--bb-navy);
  border-radius: 10px;
  padding: 1.5rem 1.75rem;
  margin: 2rem 0;
  position: relative;
  overflow: hidden;
}
.bb-callout::before {
  content: '';
  position: absolute;
  top: 0; left: 0;
  width: 4px; height: 100%;
  background: linear-gradient(180deg, var(--bb-green-bright), var(--bb-green-accent));
}
.bb-callout p {
  font-family: 'Playfair Display', Georgia, serif;
  font-size: 1.1rem;
  font-weight: 600;
  color: var(--bb-white);
  margin: 0;
  line-height: 1.55;
  letter-spacing: -0.01em;
}
.bb-callout span {
  display: block;
  font-family: 'Inter', sans-serif;
  font-size: 0.8rem;
  font-weight: 400;
  color: rgba(255,255,255,0.55);
  margin-top: 0.6rem;
  letter-spacing: 0.04em;
  text-transform: uppercase;
}

/* Section intro text */
.bb-intro-text {
  font-family: 'Inter', sans-serif;
  font-size: 0.95rem;
  color: #334155;
  line-height: 1.85;
  margin-bottom: 1.5rem;
}

/* Visual divider with label */
.bb-divider {
  display: flex;
  align-items: center;
  gap: 1rem;
  margin: 2.25rem 0;
}
.bb-divider-line {
  flex: 1;
  height: 1px;
  background: var(--bb-border);
}
.bb-divider-label {
  font-family: 'Inter', sans-serif;
  font-size: 0.72rem;
  font-weight: 700;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  color: var(--bb-green-accent);
  white-space: nowrap;
}

/* Example Cards Grid */
.bb-example-grid {
  display: grid;
  grid-template-columns: 1fr;
  gap: 1.25rem;
  margin: 1.5rem 0;
}
.bb-example-card {
  background: var(--bb-white);
  border: 1px solid var(--bb-border);
  border-radius: 8px;
  padding: 1.5rem;
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
  font-size: 1rem;
  font-weight: 700;
  padding-bottom: 0.65rem;
  border-bottom: 2px solid var(--bb-green-bg);
  margin-bottom: 0.75rem;
}
.bb-example-card p {
  color: var(--bb-text-secondary);
  font-size: 0.9rem;
  line-height: 1.75;
  margin: 0 0 0.6rem;
}
.bb-example-card p:last-child { margin-bottom: 0; }

/* Two-column split for Beyond the Science */
.bb-two-col {
  display: grid;
  grid-template-columns: 1fr;
  gap: 1.75rem;
  margin: 1.5rem 0;
  align-items: start;
}
.bb-two-col-text p {
  font-family: 'Inter', sans-serif;
  color: #334155;
  font-size: 0.93rem;
  line-height: 1.85;
  margin: 0 0 0.9rem;
}
.bb-two-col-text p:last-child { margin-bottom: 0; }

/* Misconception Blocks */
.bb-misconception {
  background: var(--bb-off-white);
  border: 1px solid var(--bb-border);
  border-left: 3px solid var(--bb-green-accent);
  border-radius: 8px;
  padding: 1.25rem 1.5rem;
  margin-bottom: 0.85rem;
}
.bb-misconception strong {
  color: var(--bb-navy);
  font-family: 'Inter', sans-serif;
  font-size: 0.93rem;
  font-weight: 600;
}
.bb-misconception p {
  color: var(--bb-text-secondary);
  margin: 0.45rem 0 0;
  font-size: 0.9rem;
  line-height: 1.75;
}

/* Desktop */
@media (min-width: 769px) {
  .bb-page-hero { padding: 3.5rem 3rem; border-radius: 12px; }
  .bb-page-hero h1 { font-size: 2.25rem; }
  .bb-page-hero p { font-size: 1.1rem; }
  .bb-example-grid { grid-template-columns: repeat(2, 1fr); gap: 1.5rem; }
  .bb-two-col { grid-template-columns: 3fr 2fr; gap: 2.5rem; }
  .bb-callout p { font-size: 1.2rem; }
  .bb-img-placeholder { padding: 3rem 2rem; font-size: 0.88rem; }
}
</style>

<div class="bb-page-hero">
  <h1>What is Biotechnology, Really?</h1>
  <p>Understanding the science shaping our future — in plain language, no prerequisites required.</p>
</div>

<p class="bb-intro-text">Biotechnology is using living systems — cells, bacteria, proteins, DNA — to create useful products or solve real problems.</p>

<div class="bb-callout">
  <p>"Biotech = biology + technology to solve real problems."</p>
  <span>The simplest definition that actually holds up</span>
</div>

<p class="bb-intro-text">It sounds vague because biotech is <strong>incredibly broad</strong>. It touches medicine, agriculture, environmental science, manufacturing, and more. The best way to understand it is through examples.</p>

<div class="bb-divider">
  <div class="bb-divider-line"></div>
  <div class="bb-divider-label">Real-World Examples</div>
  <div class="bb-divider-line"></div>
</div>

## Real-World Examples

<div class="bb-example-grid">

  <div class="bb-example-card">
    <h3>Medicine</h3>
    <p>The insulin keeping millions of diabetics alive is made by bacteria. Scientists insert the human insulin gene into E. coli, turning microbes into living medicine factories.</p>
    <p>CAR-T therapy goes further: doctors extract your immune cells, genetically reprogram them to recognize cancer, and inject them back. Your own cells become trained to fight tumors.</p>
  </div>

  <div class="bb-example-card">
    <h3>Agriculture</h3>
    <p>Drought-resistant crops can survive on 30% less water. In regions facing water scarcity, that's not just innovation — it's survival.</p>
    <p>The plant-based meat revolution relies on heme, a protein made by engineered yeast. It's what makes Impossible meat taste remarkably close to beef.</p>
  </div>

  <div class="bb-example-card">
    <h3>Environment</h3>
    <p>Bioremediation uses bacteria that break down petroleum into harmless compounds — turning oil spill disasters into manageable cleanups.</p>
    <p>Bioplastics made from plants instead of petroleum decompose in months, not centuries — and are already being used in packaging and utensils.</p>
  </div>

  <div class="bb-example-card">
    <h3>The Cutting Edge</h3>
    <p>Bioprinting is happening now — researchers use 3D printers loaded with living cells to build skin grafts, cartilage, and blood vessels.</p>
    <p>Brain organoids (mini-brains grown from stem cells) are helping scientists study Alzheimer's, test drugs, and understand brain development without human trials.</p>
  </div>

</div>

<div class="bb-divider">
  <div class="bb-divider-line"></div>
  <div class="bb-divider-label">Beyond the Lab</div>
  <div class="bb-divider-line"></div>
</div>

## Beyond the Science

<div class="bb-two-col">
  <div class="bb-two-col-text">
    <p>A breakthrough in the lab is just the beginning. Getting from concept to the real world takes an entire team — and most of them aren't scientists.</p>
    <p>Take mRNA vaccines. The underlying science existed for decades. Turning it into something that reached billions of people took business strategists, regulatory experts, manufacturing engineers, ethicists, and communicators working in parallel.</p>
    <p>Someone had to decide what was worth pursuing and who would pay for it. Someone had to design safe trials and navigate the FDA. Someone had to figure out how to manufacture at scale without losing efficacy. Someone had to explain a brand-new technology to a skeptical public.</p>
    <p>That's why biotech needs business people, engineers, lawyers, writers, and project managers just as much as it needs scientists. The science is step one — everything else is steps two through twenty.</p>
  </div>
  <div>
    <div class="bb-img-placeholder">
      [PLACEHOLDER: Illustration — showing the cross-functional team behind a biotech breakthrough: researcher, engineer, regulatory specialist, communicator]
    </div>
  </div>
</div>

<div class="bb-divider">
  <div class="bb-divider-line"></div>
  <div class="bb-divider-label">Common Misconceptions</div>
  <div class="bb-divider-line"></div>
</div>

## Common Misconceptions

<div class="bb-misconception">
  <strong>"You need to be good at biology to work in the industry."</strong>
  <p>Not necessarily. If you can explain complex ideas simply, science communication is an option. If you're organized and analytical, there's operations. Biotech employs humanities majors, business students, and engineers just as readily as biology PhDs.</p>
</div>

<div class="bb-misconception">
  <strong>"It's all lab work."</strong>
  <p>Lab work is one slice of a much bigger picture. There's also manufacturing, regulatory affairs, sales, policy, data analysis, and more. The <a href="/career-pathways/" style="color: #3A7D5C; font-weight: 600;">Career Pathways</a> page shows the full range.</p>
</div>

<div class="bb-misconception">
  <strong>"You need a PhD."</strong>
  <p>Only if you want to lead independent research. Most biotech jobs in regulatory, manufacturing, business, and operations require a bachelor's degree or less — and some only require a high school diploma and on-the-job training. Certificate programs can get you there in months. There are entry points at every level.</p>
</div>
