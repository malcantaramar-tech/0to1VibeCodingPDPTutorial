# Tutorial Concept Document
## "From Idea to Launch: Vibe Coding Your Personal Website Step by Step"

**Status:** Draft for alignment — not yet built  
**Target audience:** PM leads & senior leadership with zero coding experience  
**Format:** A single prompt pasted into Cursor's agent chat  
**Deliverable for the learner:** A live, deployed personal website they built themselves  

---

## 1. What the Learner Experiences

When a learner pastes the prompt into Cursor, the AI takes on a **dual role**:

| Role | What it does |
|---|---|
| **1-on-1 Tutor** | Teaches concepts, asks questions, checks understanding, gives feedback, paces the journey |
| **Cursor Agent** | Creates files, writes code, runs commands, deploys — all with the learner's approval |

The interaction is **conversational and sequential**. The AI asks one question or introduces one concept at a time. The learner responds (ideally via voice dictation), and only then does the AI move forward. The learner never sees a wall of text or a list of 10 things to do.

### Interaction Pattern (repeated throughout)

```
1. AI introduces a concept or asks a question
2. Learner responds (voice or text)
3. AI validates, gives feedback, or asks a follow-up
4. AI performs a hands-on action (creates a file, writes code, etc.)
5. AI explains what it just did and why
6. Checkpoint — learner confirms they understand before moving on
```

### Progress Signals

At every major transition, the AI shows a progress bar like:

```
━━━━━━━━━━░░░░░░░░░░ 40% complete
📍 You are here: Solution Design → Choosing your color palette
⏭️ Next up: Translating your design into a requirements doc
```

This keeps motivation high and gives the learner a sense of the full journey.

---

## 2. Tutorial Structure — Section by Section

### SECTION 0: Welcome & Setup (~5 min)

**Purpose:** Make the learner feel safe, oriented, and excited.

**What happens:**
- The AI introduces itself: "I'm your tutor and your builder. I'll teach you the concepts, and I'll also do the technical work — with your approval every step of the way."
- Explains what vibe coding is in plain language: *"You describe what you want in natural language, and AI turns it into working software. Your job is to think, decide, and direct — not to write code."*
- Explains why this matters for leaders: strategic advantage, faster prototyping, better conversations with engineering.
- Explains tool approvals: "Cursor will sometimes ask you to approve an action. I'll always tell you what it's about to do and why it's safe before it asks."
- Teaches a key shortcut: **Cmd+Shift+V** — toggles the editor between raw code and formatted preview. *"When you see a file full of symbols and markdown syntax, hit Cmd+Shift+V and it turns into a clean, readable document. This will be your best friend throughout the tutorial."*
- Explains **how projects and folders work in Cursor:**
  - *"Cursor works with a project folder — think of it as your workspace. Everything we build lives inside this folder: your website files, your documents, your design system."*
  - Shows the file explorer panel on the left: *"This sidebar is your project's filing cabinet. Every file and folder I create will appear here."*
  - Explains the concept: *"When you open a folder in Cursor, that becomes your project. The AI can only see and work with files inside this folder. It's like a sandbox — contained and safe."*
  - Points out the project folder that the AI just created during setup: *"See these files that just appeared? That's the AI setting up our workspace. Let's walk through what each one is."* — briefly tours the instruction file, the design system, and the requirements template so the learner understands the landscape before building begins.
- Encourages voice dictation: "You can speak your answers instead of typing. It's faster and more natural."
- Quick environment check: confirms Cursor is set up, the workspace folder exists, etc.

**Learner interaction:** The AI asks the learner to introduce themselves briefly (name, role, what they hope to get out of this). This personalizes the rest of the experience.

---

### SECTION 1: Foundations (~10 min)

**Purpose:** Build mental models before building anything.

**What's covered:**
- **What is a website, really?** — Files (HTML, CSS, JS) served from a computer to a browser. Explained with a physical-world analogy (e.g., a website is like a document in a binder on a shelf that anyone can request a copy of).
- **What is vibe coding?** — A shift from writing code to directing an AI that writes code. The human brings context, taste, and judgment. The AI brings speed and syntax.
- **Why this matters for PMs & leaders** — Vibe coding unlocks a new level of performance for individuals and teams. It gives everyone the ability to build products themselves. In large organizations the goal isn't to replace engineers — it's to collaborate with them better: prototype ideas independently, evaluate technical feasibility faster, speak their language. But the broader unlock is real — anyone with product sense can now go from idea to working software.
- **The PDP framework** — Starts with a key insight: "An AI agent is only as good as the context you give it. If you jump straight into asking the AI to build, without clarity on what you're solving for and why, the result will be generic at best — wrong at worst. That's why we'll work across the full PDP — Discovery, Design, Develop, Roll Out — ensuring what we're solving for and why is clear before we write a single line of code." Then connects it to their existing knowledge: "You already know this framework. Now you'll experience it from the builder's side."

**Learner interaction:**
- AI asks: "In your own words, what do you think vibe coding changes about how products get built?" — The learner must articulate the concept before moving on.
- AI asks: "What would you want your personal website to say about you?" — Seeds the discovery phase.

**Reflection point:** "You now understand the tools and the process. Everything from here is building."

---

### SECTION 2: Discovery (~15 min)

**Purpose:** Define the problem, audience, and goals — exactly like a real product discovery.

**What happens:**
The AI runs a structured discovery conversation, asking one question at a time. It mirrors how a PM would run discovery on a real product.

But first — the AI acknowledges that not everyone has a real, pressing need for a personal website. It asks upfront:

> "Before we start: do you have a genuine need for a personal website, or are you here mainly to learn the process? Both are perfectly valid — it just changes how we approach discovery."

**Path A — Real need:** The learner has a genuine reason (career transition, speaking profile, side project showcase, etc.). The AI runs discovery against their actual situation.

**Path B — Learning exercise:** The learner doesn't have a pressing need. The AI offers 2–3 lightweight hypothetical scenarios to adopt as their own:
- *"The Speaker"* — You're building a public profile to support a growing presence at conferences and panels. You need a site that says: here's who I am, here's what I talk about, here's how to book me.
- *"The Portfolio Leader"* — You want a single place that showcases the products you've led, the teams you've built, and what you stand for as a leader.
- *"The Side Project"* — You have a passion project or idea outside work and want a landing page that explains it and captures interest.

The learner picks one (or riffs on it), and the AI runs discovery as if it were real. The process is identical — the scenario just provides a starting context.

**Questions the AI asks (sequentially, adapted to the chosen path):**
1. "Who is this website for? Who will actually visit it and why?" (target audience)
2. "What's the one thing you want someone to take away after visiting your site?" (core value proposition)
3. "What problem does NOT having a personal website create for you today?" (problem statement — for Path B, framed within the chosen scenario)
4. "What are 3 personal websites you admire? What do you like about them?" (competitive/inspiration analysis — AI can look them up if the learner provides URLs)
5. "What content do you already have that could go on the site?" (inventory: bio, headshot, resume, portfolio pieces, links — for Path B, the AI helps the learner brainstorm placeholder content)

**Deliverable:** The AI compiles the learner's answers into a **Discovery Document** — a structured markdown file saved to the project. The structure mirrors the Whisper discovery doc exactly, adapted for a personal website:

```
Discovery Document
├── 1. Intro (purpose of the document, author, date, status)
├── 2. Customer Needs (who visits the site, what they need functionally & emotionally)
├── 3. Problem Statement (what's missing today without this website — short & long form)
├── 4. Market Characteristics (landscape of personal websites / portfolios in their space)
└── 5. High-Level Solution Concept (what the website is and how it works at a conceptual level)
```

The AI guides the learner through each area with targeted questions, one at a time.

The AI shows the complete document and asks the learner to review and approve it before moving on.

**Learner interaction:** Answering discovery questions, reviewing and approving the document.

**Reflection point:** "You just ran a product discovery — on yourself. Notice how the same framework applies whether you're building a consumer app or a personal page."

---

### SECTION 3: Solution Design (~20 min)

**Purpose:** Turn the discovery into a concrete plan — features, visual identity, and requirements.

**Three sub-phases:**

#### 3A. Feature Definition
The AI asks what sections/pages the website should have, offering a starting menu:
- Hero / landing section
- About me
- Experience / career timeline
- Projects or portfolio
- Blog or writing
- Contact
- Testimonials

The learner picks what they want. The AI explains what each one involves (light/medium/complex) so the learner can make informed decisions. The AI recommends a scope for a first version.

#### 3B. Visual Identity (built on top of a baseline design system)

The tutorial uses `web-design-system.json` as the **baseline design system**. This file defines a complete, production-quality set of design tokens: colors, typography, spacing, components, layout patterns, effects, and guidelines. Instead of building a design system from scratch, the learner starts from this proven foundation and only adjusts the specific choices that make the site theirs.

The AI explains this upfront: *"We're starting from a professional design system that handles all the technical details — spacing, shadows, responsive layouts, accessibility. Your job is to make the key creative decisions that give the site your identity. Everything else is already taken care of."*

**What the learner customizes (one choice at a time):**
1. **Color palette:** AI shows the baseline palette (dark teal, off-white, deep blue) and offers 2–3 alternative palettes. Learner picks one. The AI updates the relevant color tokens in the design system.
2. **Typography:** AI shows the baseline fonts (Cormorant Garamond + Outfit) and proposes 2 alternative pairings. Learner picks one. The AI updates the font tokens.
3. **Layout style:** AI describes 2–3 layout approaches (single-page scroll, multi-page, card-based). Learner picks one.
4. **Logo/monogram:** AI offers to generate a simple text-based logo or monogram using their initials and the chosen palette.
5. **Language:** Baseline is in Spanish — AI asks: "Should your site be in English, Spanish, or another language?" and adjusts all UI copy accordingly.

Each choice is presented with a clear "here's what this means in practice" explanation. Choices the learner doesn't customize stay at their baseline defaults — so the result always looks polished, even if someone only changes one or two things.

#### 3B-ii. Design Mockup
Once the learner has made all their visual identity choices (tone, palette, typography, layout, logo), the AI generates a **design mockup** — a static HTML/CSS page that applies those choices to the site structure defined in 3A. This is not the final build; it's a visual proof-of-concept.

The mockup shows:
- The chosen color palette and fonts applied to real sections
- The layout structure with placeholder content
- The logo/monogram in context

The AI presents it to the learner: *"Here's a preview of what your site will look like based on everything you've chosen. Take a look — does this feel right? Anything you'd want to adjust before we start building for real?"*

The learner can request changes (different palette, swap the layout, tweak the logo), and the AI regenerates the mockup until the learner is happy. Only then do we move to the requirements doc.

This is a key moment: the learner sees their decisions come to life for the first time. It builds confidence and catches misalignment early — before development begins.

#### 3C. Technical Requirements Document

This is the **single source of truth** the AI references during development. Every build step traces back to a specific requirement. Every requirement traces back to a decision made in Discovery or Design.

The AI compiles everything into a **structured requirements document** (saved as a markdown file in the project). The document has two layers:

**Layer 1 — Sections & structure:**

```
Technical Requirements Document
├── Meta (title, author, date, version, status)
├── 1. Site Overview
│     Summary, target audience, core value prop (sourced from Discovery §1–3)
├── 2. Site Map
│     Pages/sections list with hierarchy (sourced from Feature Definition §3A)
├── 3. Design System Reference
│     Points to web-design-system.json + documents any overrides the learner chose (sourced from Visual Identity §3B)
├── 4. Technical Stack
│     Framework, hosting, deployment method (React + Vite + Tailwind, Vercel)
└── 5. Requirements Table (see Layer 2)
```

**Layer 2 — Requirements table (the core):**

Every individual requirement gets its own row with a unique ID, making it easy to reference, track, and verify during development:

```
| ID     | Section      | Requirement                           | Source       | Priority | Status   |
|--------|-------------|---------------------------------------|--------------|----------|----------|
| REQ-01 | Hero        | Display full name and role tagline     | Discovery §1 | Must     | Pending  |
| REQ-02 | Hero        | Show professional headshot             | Discovery §5 | Must     | Pending  |
| REQ-03 | Hero        | Primary CTA button ("Contact me")      | Design §3A   | Must     | Pending  |
| REQ-04 | About       | 2–3 paragraph bio                     | Discovery §5 | Must     | Pending  |
| REQ-05 | About       | Key skills / expertise list            | Design §3A   | Should   | Pending  |
| REQ-06 | Design      | Use learner's chosen color palette     | Design §3B   | Must     | Pending  |
| REQ-07 | Design      | Use learner's chosen font pairing      | Design §3B   | Must     | Pending  |
| REQ-08 | Global      | Responsive — works on mobile & desktop | Default      | Must     | Pending  |
| ...    | ...         | ...                                   | ...          | ...      | ...      |
```

**How traceability works:**
- **Source** column links each requirement back to the specific Discovery or Design section where the decision was made (e.g., "Discovery §3" = Problem Statement, "Design §3B" = Visual Identity).
- **Status** column is updated during development: `Pending → In Progress → Done`. The learner sees this at each checkpoint.
- **Priority** uses MoSCoW (Must / Should / Could / Won't) so the learner practices scoping.
- **ID** is referenced by the AI at every build checkpoint: *"I just completed REQ-01 through REQ-03. Here's what the hero section looks like."*

**Why this matters for the learner:**
The AI explicitly teaches this: *"In real product work, requirements without traceability lead to scope creep, missed intent, and 'why did we build this?' moments. Every line in this table connects back to a decision you made. If something changes later, we update it here first — then in the code."*

The AI shows the full document and asks the learner to review and approve it before development begins. Any changes during development get reflected back in the requirements table — status updates, modifications noted, new requirements added with a clear source.

**Learner interaction:** Reviewing the requirements doc, verifying traceability makes sense, approving the plan.

**Reflection point:** "You've now gone from a vague idea to a traceable plan. Every requirement has a reason. Every reason connects to a decision you made. This is the moment where most personal projects die — but not this one, because we're building it right now."

---

### SECTION 4: Development (~30 min)

**Purpose:** Build the website. The AI codes; the learner reviews, learns, and approves.

**How it works:**

The AI creates a **build plan** derived directly from the requirements table. Each build task maps to one or more requirement IDs, so progress is always traceable:

```
Build Plan
☐ 1. Project setup — scaffold React + Vite + Tailwind, apply design system    [REQ-06, REQ-07]
☐ 2. Build site structure — create page/section components per site map       [Site Map]
☐ 3. Build hero section                                                       [REQ-01, REQ-02, REQ-03]
☐ 4. Build about section                                                      [REQ-04, REQ-05]
☐ 5. Build [remaining sections per learner's choices...]                       [REQ-XX...]
☐ 6. Responsive design pass                                                   [REQ-08]
☐ 7. Final polish & cross-check all requirements                              [All REQs]
```

As each task is completed, the AI updates the requirements table status (`Pending → Done`) so the learner always has a live view of what's been built and what's left.

The AI works through each task **one at a time**, following this loop:

1. **Announce:** "I'm about to build the hero section. Here's what it will include..."
2. **Build:** AI creates/modifies files (learner approves tool actions)
3. **Explain:** "Here's what I just did and why. The `<header>` tag defines..."
4. **Show:** AI tells the learner how to preview the result (open the HTML file, or start a local server)
5. **Checkpoint:** "Does this match what you had in mind? Anything you'd change?"

The learner can request changes at any checkpoint. The AI makes adjustments before moving to the next task.

**Key teaching moments woven in:**
- When creating the first HTML file: briefly explain what HTML is (the skeleton)
- When adding CSS: briefly explain what CSS is (the skin/clothes)
- When the site goes from unstyled to styled: "This is the moment — see how CSS transformed the raw content into something that looks like a real website?"
- When adding responsive design: explain why mobile matters (likely 60%+ of their visitors)

**Learner interaction:** Approving tool actions, previewing results, requesting changes at checkpoints, answering occasional concept-check questions.

**Reflection point:** "You just built a website. Not by writing code, but by making decisions and directing an AI. This is what vibe coding looks like at its best — human judgment, AI execution."

**Peer Review (end of Development):**
The AI suggests a peer review step: "Before we ship, let's get a second opinion." It offers two options:
- Open a new Cursor chat and paste a review prompt the AI provides (AI-as-reviewer)
- Share the preview link with a colleague for human feedback

---

### SECTION 5: Rollout (~15 min)

**Purpose:** Deploy the site to the internet and learn how to maintain it.

**What happens:**
1. **Pre-launch checklist:** AI runs through a quality checklist (all links work, images load, mobile looks good, meta tags present, etc.)
2. **Deployment:** AI walks the learner through deploying to a free hosting platform (e.g., Vercel or Netlify). Explains each step and why it's needed.
3. **Custom domain (optional):** AI explains how domains work and offers to help connect one if the learner has one.
4. **Post-launch:** AI explains how to make future changes (come back to Cursor, describe what you want, AI makes the change).
5. **Monitoring basics:** Brief explanation of what to watch (is the site up, are people visiting).

**Learner interaction:** Approving deployment actions, visiting their live URL for the first time.

**Reflection point:** "Your website is live. Anyone in the world can see it right now. You went from zero to a live product in under two hours — using the same PDP process you use at work every day."

---

### SECTION 6: Wrap-Up & Reflection (~5 min)

**Purpose:** Consolidate learning, celebrate, and point to what's next.

**What happens:**
- AI summarizes the full journey: "Here's everything you did today..."
- Asks final reflection questions:
  - "What surprised you most about this process?"
  - "How might you use vibe coding in your actual work?"
  - "What would you build next?"
- Provides a cheat sheet of key concepts learned
- Encourages the learner to share their site and their experience

---

## 3. Design Principles Baked Into the Prompt

| Principle | How it manifests |
|---|---|
| **One question at a time** | The AI never dumps multiple questions. Always sequential. |
| **Active learning** | The learner must answer, explain, decide — not just read. |
| **Beginner-safe** | Every tool approval is pre-explained. No jargon without definition. |
| **Voice-first nudges** | The AI periodically reminds: "Feel free to speak your answer." |
| **Curiosity-friendly** | If the learner asks a tangent question, the AI answers it, then returns to the main thread. |
| **Progress visible** | Progress bar + "you are here" at every section transition. |
| **Real artifact** | The learner ends with a live, deployed website — not just knowledge. |
| **PDP-native** | The structure maps directly to the PDP framework they already use at work. |

---

## 4. Estimated Timing

| Section | Duration | Cumulative |
|---|---|---|
| Welcome & Setup | ~5 min | 5 min |
| Foundations | ~10 min | 15 min |
| Discovery | ~15 min | 30 min |
| Solution Design | ~20 min | 50 min |
| Development | ~30 min | 80 min |
| Rollout | ~15 min | 95 min |
| Wrap-Up | ~5 min | **~100 min** |

Total: approximately **1.5 to 2 hours**, depending on how much the learner explores.

---

## 5. Open Questions for Alignment

1. ~~**Technical complexity:**~~ **Resolved.** The baseline design system (`web-design-system.json`) uses React + Vite + Tailwind CSS. The tutorial will use this stack. The learner doesn't need to understand the stack — the AI handles it — but they get a production-quality result rather than a toy HTML page.

2. ~~**Hosting platform:**~~ **Resolved.** Vercel — simplest deployment flow from Cursor.

3. ~~**The Whisper discovery doc:**~~ **Resolved.** The Whisper discovery doc is used internally as a structural guideline for how the tutorial's discovery document should look (sections, depth, tone). It will NOT be referenced by name or shown to learners — it remains private.

4. ~~**Logo generation:**~~ **Resolved.** CSS/text monogram only — the learner's initials styled with their chosen font and palette, rendered in code. Clean, instant, no extra tools. Logo design is not the focus of this tutorial.

5. ~~**Depth of coding explanations:**~~ **Resolved.** Very lean — brief conceptual explanations only at key moments (e.g., "HTML is the skeleton, CSS is the skin"). No deep dives, no syntax walkthroughs. Enough to demystify, not enough to distract.

6. ~~**Peer review step:**~~ **Resolved.** Mandatory. The AI guides the learner to run a peer review using either another Cursor agent (new chat thread with a review prompt) or ChatGPT. The tutorial provides the review prompt and walks the learner through the process.

---

## 6. Distribution Model

**Resolved.** Tutorial files are hosted in a **GitHub repo**. The learner receives a short starter prompt that tells the AI to fetch the files and set up the project locally.

**Hosted files (in the GitHub repo):**
- `TUTORIAL-INSTRUCTIONS.md` — The full playbook the AI follows
- `web-design-system.json` — Baseline design system
- `Technical Requirements Document - Template.md` — Template used during Section 3C

**Learner experience:**
1. Open Cursor
2. Paste the starter prompt into agent chat
3. The AI fetches the files from GitHub, creates the project folder, and begins the tutorial

**Starter prompt** references the raw GitHub URLs so the AI can fetch each file. The prompt also sets the tone and explains what's about to happen so the learner feels oriented before the first tool approval appears.

---

*This is a living document. Let's iterate until the structure feels right, then I'll build the actual prompt.*
