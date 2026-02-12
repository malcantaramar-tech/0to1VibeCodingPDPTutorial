# Technical Requirements Document

| Field       | Value                                          |
|-------------|------------------------------------------------|
| **Project** | [Learner's website name]                       |
| **Author**  | [Learner name]                                 |
| **Date**    | [Auto-generated]                               |
| **Version** | 1.0                                            |
| **Status**  | Draft — Pending learner approval               |

---

## 1. Site Overview

### 1.1 Summary
<!-- Sourced from: Discovery §1 (Intro) -->

[One paragraph describing what this website is and why it exists.]

### 1.2 Target Audience
<!-- Sourced from: Discovery §2 (Customer Needs) -->

**Primary audience:** [Who will visit the site — role, context, intent]

**What they need:**
- **Functionally:** [What they're trying to do — e.g., learn about the person, find contact info, see their work]
- **Emotionally:** [How they want to feel — e.g., confident this person is credible, impressed, curious to connect]

### 1.3 Core Value Proposition
<!-- Sourced from: Discovery §2–3 (Customer Needs + Problem Statement) -->

[One sentence: what is the single most important thing a visitor should take away?]

### 1.4 Problem Statement
<!-- Sourced from: Discovery §3 (Problem Statement) -->

**Long form:**
[2–3 sentences describing the gap that exists without this website.]

**Short form:**
[One sentence distillation.]

---

## 2. Site Map

<!-- Sourced from: Design §2A (Feature Definition) -->

The site is structured as a [single-page scroll / multi-page site] with the following sections:

| Order | Section              | Description                                        | Complexity |
|-------|----------------------|----------------------------------------------------|------------|
| 1     | Hero                 | [First impression — name, tagline, CTA, image]     | Light      |
| 2     | About                | [Bio, background, personal story]                  | Light      |
| 3     | [Section name]       | [Description]                                      | [L/M/C]    |
| 4     | [Section name]       | [Description]                                      | [L/M/C]    |
| 5     | [Section name]       | [Description]                                      | [L/M/C]    |
| 6     | Contact              | [Contact info and/or form]                         | Light      |
| 7     | Footer               | [Links, copyright, social]                         | Light      |

*Complexity: Light = static content, Medium = interactive elements, Complex = dynamic/data-driven*

---

## 3. Design System

<!-- Sourced from: Design §2B (Visual Identity) -->

**Baseline:** `tutorial-web-design-system.json` (v1.0)

The following design tokens have been customized by the learner. All other tokens remain at baseline defaults.

### 3.1 Color Palette

| Token                | Baseline     | Override     | Usage                              |
|----------------------|-------------|-------------|-------------------------------------|
| primaryBackground    | `#EFECE9`   | [value]     | Section backgrounds                 |
| heroPanel            | `#FFFFFF`   | [value]     | Cards, hero inner panel             |
| darkTeal             | `#3C5759`   | [value]     | Headings, buttons, footer           |
| deepBlue             | `#143852`   | [value]     | Hero subtitle, accents              |
| bodyText             | `#4b5563`   | [value]     | Paragraphs, descriptions            |
| footerText           | `#D0D5CE`   | [value]     | Footer text on dark background      |

*If "Override" is blank or `—`, the baseline value is used.*

### 3.2 Typography

| Token             | Baseline                      | Override          |
|-------------------|------------------------------|-------------------|
| Primary (display) | Cormorant Garamond, serif    | [font or `—`]     |
| Secondary (body)  | Outfit, sans-serif           | [font or `—`]     |

### 3.3 Layout

| Decision        | Choice                                              |
|-----------------|------------------------------------------------------|
| Layout style    | [Single-page scroll / Multi-page / Card-based]       |
| Max width       | 1440px (baseline)                                    |
| Responsive      | Yes — mobile-first (baseline)                        |

### 3.4 Logo / Monogram

| Element       | Value                                                 |
|---------------|-------------------------------------------------------|
| Type          | [Text-based monogram / Generated image / None]        |
| Content       | [Initials or text used]                               |
| Placement     | [Header nav / Hero section / Both]                    |

### 3.5 Language

| Element       | Value                                                 |
|---------------|-------------------------------------------------------|
| UI copy       | [English / Spanish / Other]                           |
| Content       | [English / Spanish / Other]                           |

---

## 4. Technical Stack

<!-- These are default decisions made by the tutorial. Documented here for transparency. -->

| Layer          | Choice           | Rationale                                         |
|----------------|-----------------|---------------------------------------------------|
| Framework      | React + Vite    | Fast builds, component-based, modern standard     |
| Styling        | Tailwind CSS    | Utility-first, matches the design system JSON     |
| Hosting        | [Vercel / TBD]  | Free tier, instant deploys, custom domain support |
| Version control| Git (local)     | Track changes throughout development              |
| Design tokens  | `tutorial-web-design-system.json` | Single source of truth for all visual styles |

---

## 5. Content Map

<!-- Sourced from: Discovery conversation (Content Inventory) + Design §2A -->

What content goes where. Marks whether the learner has the content ready or needs to create/source it.

| Section          | Content needed                        | Status            |
|------------------|---------------------------------------|-------------------|
| Hero             | Full name, role/tagline, headshot     | [Ready / Needed]  |
| Hero             | Primary CTA label and target          | [Ready / Needed]  |
| About            | Bio (2–3 paragraphs)                  | [Ready / Needed]  |
| About            | Skills / expertise list               | [Ready / Needed]  |
| [Section name]   | [Content description]                 | [Ready / Needed]  |
| [Section name]   | [Content description]                 | [Ready / Needed]  |
| Contact          | Email, social links, form fields      | [Ready / Needed]  |
| Footer           | Copyright text, navigation links      | [Ready / Needed]  |

*For content marked "Needed": the AI will generate placeholder content during development. The learner replaces it with real content before or after launch.*

---

## 6. Requirements Table

<!-- This is the core of the document. Every row traces back to a decision. Every build step references these IDs. -->

### Legend

- **Source:** Links to the Discovery (D§) or Design (DS§) section where the decision was made.
- **Priority:** Must (non-negotiable for v1) / Should (important, include if possible) / Could (nice-to-have, defer if needed) / Won't (explicitly out of scope for v1).
- **Status:** Pending → In Progress → Done / Changed / Removed.

### 6.1 Structure & Navigation

| ID     | Requirement                                              | Source  | Priority | Status  |
|--------|----------------------------------------------------------|---------|----------|---------|
| REQ-01 | Site uses [single-page / multi-page] layout              | DS§2B   | Must     | Pending |
| REQ-02 | Navigation includes links to all sections                | DS§2A   | Must     | Pending |
| REQ-03 | Navigation is sticky/fixed on scroll                     | Default | Should   | Pending |
| REQ-04 | Mobile hamburger menu for small screens                  | Default | Must     | Pending |

### 6.2 Hero Section

| ID     | Requirement                                              | Source  | Priority | Status  |
|--------|----------------------------------------------------------|---------|----------|---------|
| REQ-05 | Display full name prominently                            | D§1     | Must     | Pending |
| REQ-06 | Role or tagline below name                               | D§2     | Must     | Pending |
| REQ-07 | Professional headshot or image                           | D§5     | Must     | Pending |
| REQ-08 | Primary CTA button (e.g., "Contact me", "See my work")  | DS§2A   | Must     | Pending |
| REQ-09 | Secondary CTA button (optional)                          | DS§2A   | Could    | Pending |

### 6.3 About Section

| ID     | Requirement                                              | Source  | Priority | Status  |
|--------|----------------------------------------------------------|---------|----------|---------|
| REQ-10 | Bio text (2–3 paragraphs)                                | D§5     | Must     | Pending |
| REQ-11 | Key skills or expertise list                             | DS§2A   | Should   | Pending |
| REQ-12 | Supporting image or visual element                       | DS§2A   | Could    | Pending |

### 6.4 [Section Name] — *Repeat for each section the learner chose*

| ID     | Requirement                                              | Source  | Priority | Status  |
|--------|----------------------------------------------------------|---------|----------|---------|
| REQ-XX | [Requirement description]                                | [Ref]   | [M/S/C]  | Pending |
| REQ-XX | [Requirement description]                                | [Ref]   | [M/S/C]  | Pending |

### 6.5 Contact Section

| ID     | Requirement                                              | Source  | Priority | Status  |
|--------|----------------------------------------------------------|---------|----------|---------|
| REQ-XX | Display email address                                    | D§5     | Must     | Pending |
| REQ-XX | Social media links (LinkedIn, etc.)                      | D§5     | Should   | Pending |
| REQ-XX | Contact form (name, email, message)                      | DS§2A   | Could    | Pending |

### 6.6 Design & Global

| ID     | Requirement                                              | Source  | Priority | Status  |
|--------|----------------------------------------------------------|---------|----------|---------|
| REQ-XX | Apply learner's chosen color palette                     | DS§2B   | Must     | Pending |
| REQ-XX | Apply learner's chosen font pairing                      | DS§2B   | Must     | Pending |
| REQ-XX | Display logo/monogram in header                          | DS§2B   | Should   | Pending |
| REQ-XX | All UI copy in learner's chosen language                  | DS§2B   | Must     | Pending |
| REQ-XX | Responsive — fully functional on mobile and desktop      | Default | Must     | Pending |
| REQ-XX | Accessible — sufficient contrast, focus states, alt text | Default | Must     | Pending |
| REQ-XX | Meta tags (title, description, Open Graph)               | Default | Should   | Pending |
| REQ-XX | Favicon                                                  | Default | Could    | Pending |

### 6.7 Deployment & Rollout

| ID     | Requirement                                              | Source  | Priority | Status  |
|--------|----------------------------------------------------------|---------|----------|---------|
| REQ-XX | Deployed to [Vercel / TBD] on a public URL               | §4      | Must     | Pending |
| REQ-XX | Custom domain connected (if learner has one)              | §4      | Could    | Pending |
| REQ-XX | Basic performance check (loads in < 3s)                   | Default | Should   | Pending |

---

## 7. Change Log

<!-- Updated during development. Tracks any requirement that changes after initial approval. -->

| Date | ID(s) affected | Change description                        | Reason              |
|------|----------------|-------------------------------------------|---------------------|
| —    | —              | *No changes yet — document just created.* | —                   |

---

## 8. Sign-Off

| Role            | Name        | Date       | Approved |
|-----------------|-------------|------------|----------|
| Product Owner   | [Learner]   | [Date]     | [ ]      |
| Builder (AI)    | Cursor Agent| [Date]     | [ ]      |

---

*This document is the single source of truth for development. All build steps reference requirement IDs from section 6. Any changes during development are logged in section 7 and reflected in the requirements table status column.*
