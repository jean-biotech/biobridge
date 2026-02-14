# BioBridge Website Modernization Plan

## Design Direction

Drawing from the inspiration images (First Generation Investors, Ramp, Robinhood, Wharton Healthcare Analytics), the redesign will shift from the current soft/friendly aesthetic to a **bold, professional, high-contrast** design that builds credibility and trust.

### Key Design Principles from Inspiration
- **Bold, oversized hero typography** (all 4 examples use dramatically large text)
- **Dark/bold color sections** (dark navy, emerald, black backgrounds)
- **Trust indicators** (logos bar, social proof, credibility markers)
- **Edge-to-edge sections** (full-width layouts, not contained in small rounded boxes)
- **Generous whitespace** with clear section separation
- **Strong visual hierarchy** - each section has one focal point
- **Professional CTAs** (email capture, not just simple links)

---

## Changes by File

### 1. `assets/css/main.scss` - Color System & Global Styles

**Current:** Soft sage green (#7a9b76), off-white background (#faf9f7), subtle styling
**New:**
- Primary color: Deep navy/dark teal (#0f2b3c) for authority
- Accent color: Vibrant green (#22c55e) for CTAs and highlights
- Background: Clean white (#ffffff) with light gray sections (#f8fafc)
- Text: Near-black (#0f172a) for high readability
- Updated masthead: Clean white with subtle bottom border, no background tint
- Smooth scroll behavior, better base typography
- Updated button styles with accent green and hover states
- Global section spacing and container width rules

### 2. `index.md` - Homepage (Major Redesign)

This is the biggest change. The homepage will be restructured into distinct full-width sections.

**Section 1: Hero**
- Full-width dark background (deep navy/dark teal gradient)
- Dramatically larger headline (~3.5rem desktop) with bold weight
- Concise subheadline in lighter weight
- Two CTAs side by side: primary "Get Started" (green accent) + secondary "Learn More" (outline)
- Clean, edge-to-edge design (no rounded container box)

**Section 2: Social Proof / Credibility Bar**
- Light background strip
- Show follower count or key metrics (e.g., "10,000+ students reached" or "Trusted by students at X universities")
- OR: "As featured in" / "Built by students at" trust badges
- Thin, horizontal layout

**Section 3: Three Pillars (What BioBridge Offers)**
- Clean 3-column grid on white background
- Each card: small icon/number at top, bold title, short description, subtle "Learn more" link
- Replaces the emoji-heavy icon grid with a more professional treatment
- Cards use subtle left-border accent or top-border accent instead of full borders

**Section 4: Problem / Solution Split**
- Two-column layout with stronger visual treatment
- Left column "The Problem" with dark background
- Right column "BioBridge is the answer" with light background and green accent
- Larger text, stronger contrast between the two sides

**Section 5: Founder Story**
- Clean full-width section with light gray background
- Larger profile photo with modern treatment (no heavy drop shadow)
- Refined typography for the narrative text
- Social links as clean icon buttons

**Section 6: CTA Banner**
- New section at the bottom before footer
- Full-width dark background
- Bold headline: "Ready to start your biotech journey?"
- Email capture or link CTA
- Replaces abrupt page ending

### 3. `_pages/what-is-biotech.md` - Content Page Refresh

- Add styled page header section with subtitle text
- Modernize the 4 example cards: remove emoji headers, use left-border accent color treatment, cleaner typography
- Add subtle background alternation between sections
- Improve the misconceptions section with an accordion or distinct card style
- Keep same content, just better visual presentation

### 4. `_pages/career-pathways.md` - Career Cards

- Add page header with descriptive subtitle
- Convert each career pathway into a professional card component
- Each card: colored top border, pathway title, description, key details (locations, entry points, skills) in organized sub-sections
- Consistent card grid layout instead of plain markdown sections

### 5. `_pages/resources.md` - Resource Cards

- Add page header with subtitle
- Convert resource lists into styled card grids per category
- Each resource: clean card with title, source, brief description
- Category headers with accent styling
- More visual separation between resource types

### 6. `_pages/get-involved.md` - Engagement Page

- Add hero-style page header with CTA
- Style each section (Students, Mentors, Contributors) as distinct cards with icons
- Add a prominent email CTA section
- Better visual hierarchy for contact information
- Professional "Stay Connected" footer section

### 7. `_pages/products.md` - Product Page

- Professional product showcase layout
- Feature list with checkmark icons instead of bullet dashes
- Pricing card with clear visual hierarchy
- Prominent CTA button for purchase
- "Coming Soon" section as a clean roadmap/timeline style

### 8. `_config.yml` - Minor Updates

- Add social media links to footer (Instagram, LinkedIn)
- No structural changes needed

### 9. `_data/navigation.yml` - No Changes

- Navigation structure is fine as-is

---

## Color Palette Summary

| Role | Current | New |
|------|---------|-----|
| Primary/Dark | #7a9b76 (sage green) | #0f2b3c (deep navy) |
| Accent/CTA | #5a7a56 (darker sage) | #22c55e (vibrant green) |
| Background | #faf9f7 (ivory) | #ffffff (white) |
| Alt Background | N/A | #f8fafc (light gray) |
| Text | #3a3a3a (charcoal) | #0f172a (near-black) |
| Muted Text | N/A | #64748b (slate gray) |
| Border | #e8e8e8 | #e2e8f0 (cool gray) |

## Typography (Keeping Inter + Poppins)

- Hero: Poppins 700, 3.5rem (desktop) / 2rem (mobile)
- Section headers: Poppins 600, 2rem
- Card titles: Poppins 600, 1.25rem
- Body: Inter 400, 1rem, line-height 1.75
- Small/muted: Inter 400, 0.875rem

## Scope

- **7 files modified** (index.md, main.scss, 5 content pages)
- **1 file with minor updates** (_config.yml)
- **No new dependencies** - all achievable with CSS within the Jekyll/Minimal Mistakes framework
- **No content changes** - same text, restructured presentation
- **Fully responsive** - mobile-first responsive breakpoints maintained
