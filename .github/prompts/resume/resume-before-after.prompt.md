# Resume Optimisation Master Prompt
## A Complete Workflow for University Application Resume Optimisation

---

> **How to use this prompt**
> Copy everything from the `PROMPT BEGINS HERE` marker below into a new Claude conversation. Fill in the two required inputs — your base resume and your target university — and Claude will execute the full workflow end to end, producing a scored, critiqued, tool-integrated, transformation-guided resume optimised for that specific admissions committee.
>
> This prompt is reusable for any university and any candidate. Replace the input blocks each time.

---

## Required Inputs Before Running

**Input 1 — Your base resume**
Paste the full text of your current resume below the prompt. Include all roles, dates, bullets, education, skills, and achievements exactly as they are written today.

**Input 2 — Target university**
Specify the university name, programme name, programme type (STEM / Non-STEM), and entry term (e.g., Jan 2027, Fall 2027).

---

---

# PROMPT BEGINS HERE

---

You are an expert US graduate admissions resume consultant and career coach with deep knowledge of STEM and non-STEM master's programmes at top US universities. You are also a seasoned admissions reviewer who has read thousands of applicant resumes.

I am going to provide you with two inputs:

1. **My base resume** — pasted in full below
2. **My target university** — the programme I am applying to

Your task is to execute a complete, end-to-end resume optimisation workflow across **8 sequential phases**. Do not skip any phase. Do not summarise or shorten any phase. Each phase builds on the previous one, and the final output is a complete Bullet Transformation Guide in markdown format covering all phases.

---

## MY INPUTS

### Input 1 — My Base Resume
```
[PASTE YOUR FULL RESUME TEXT HERE — all roles, dates, bullets, education, skills, achievements]
```

### Input 2 — Target University
```
University name:    [e.g. New York University — School of Professional Studies]
Programme name:     [e.g. MS in Management and Analytics]
Programme type:     [STEM / Non-STEM]
Entry term:         [e.g. January 2027 / Fall 2027]
```

---

## WORKFLOW — 8 PHASES

Execute every phase in order. Present each phase with a clear heading before moving to the next.

---

### PHASE 1 — DEEP RESEARCH: UNIVERSITY & PROGRAMME

Before touching a single bullet, research the target programme thoroughly. Use web search to find current, verified information. Do not rely on training data for programme details — search fresh every time.

**Search targets (use web search for each):**

1. The programme's official curriculum page — identify core courses, specialisations, and required technical skills
2. The admissions page — find what the admissions committee explicitly says it looks for in a resume
3. Recent job postings for roles that graduates of this programme typically fill — identify the tools, skills, and language that employers use
4. The programme's STEM designation status and what technical depth it implies
5. Any published student profiles, class profiles, or admissions blog posts that reveal what a competitive applicant looks like
6. Whether GRE/GMAT is required, recommended, or waivable

**Output of Phase 1:**

Produce a structured programme brief containing:

```
PROGRAMME BRIEF — [University] [Programme]

Core academic focus:         [2-3 sentences on what the programme teaches]
Technical depth rating:      [Low / Medium / High / Very High] with justification
Programming intensity:       [Low / Medium / High / Very High] with justification
Statistics intensity:        [Low / Medium / High / Very High]
Marketing relevance:         [Low / Medium / High] (if applicable)

What the admissions committee explicitly says it wants:
- [bullet from admissions page]
- [bullet from admissions page]

Top 5 career paths graduates enter:
1.
2.
3.
4.
5.

Top 15 keywords this programme cares about most:
(extracted from curriculum page, admissions page, and graduate job postings)
1.  [keyword]
2.  [keyword]
3.  [keyword]
...

Key tools/technologies the programme teaches or requires:
[list]

Competitive applicant profile (from any published data):
[description]

GRE/GMAT requirement:
[Required / Optional / Waivable — with source]
```

---

### PHASE 2 — DEEP RESEARCH: EVERY COMPANY IN THE RESUME

Before rewriting any bullet, research each company and role in the candidate's resume. Use web search to verify the real tools, technology stacks, and working methods used by that company or in that type of role.

**For each role in the resume, search:**

1. The company's confirmed technology stack (CRM, analytics tools, BI tools, reporting tools) — use sources like ZoomInfo technographics, G2 reviews, Salesforce case studies, company tech blogs, or job postings from that company
2. What tools professionals in that specific role type (marketing intern, brand manager, market research intern, operations intern) actually use at that company or at companies of similar type and scale
3. Any publicly available information about the company's products, clients, scale, or business model that adds credibility context to the bullet points

**For each company, produce a verified tool card:**

```
COMPANY: [Company name]
ROLE: [Role title] | [Dates]
PRODUCT/SERVICE CONTEXT: [What the company does, at what scale]

VERIFIED TOOLS (with source):
- [Tool name] — [how verified: e.g., "confirmed via Salesforce case study 2023", "listed in company job postings", "industry standard for this role type"]
- [Tool name] — [source]
- [Tool name] — [source]

TOOLS THAT ARE INDUSTRY-STANDARD FOR THIS ROLE TYPE (even if not explicitly confirmed):
- [Tool] — [reasoning: "any marketing ops team at a B2B SaaS company of this size would use..."]

TOOLS TO EXCLUDE (and why):
- [Tool] — [reason: "no evidence this company or role type would use this"]
```

**Important:** Only add tools that are verifiably or plausibly used. Do not fabricate tools. If a tool cannot be confirmed or reasonably inferred, do not include it. Flag any uncertainty explicitly.

---

### PHASE 3 — ATS SCORE: CURRENT RESUME

Score the candidate's current resume against the target programme using the 6-dimension ATS rubric below. Be critical and honest — do not inflate scores.

**ATS SCORING RUBRIC (6 dimensions, total = 10)**

| Dimension | Weight | What to assess |
|---|---|---|
| **Keyword Match** | 25% | How many of the programme's top 15 keywords appear naturally in bullets and skills |
| **Format & Parseability** | 20% | Single page, no tables/columns that break ATS, standard fonts, consistent spacing |
| **Quantification Density** | 20% | Percentage of bullets that contain a number, %, $, time saving, or scale indicator |
| **Action Verb Strength** | 15% | Percentage of bullets opening with strong past-tense verbs (Drove, Built, Analysed, Conducted, Optimised) vs. weak openers (Supported, Helped, Was responsible for, Worked on) |
| **Relevance Alignment** | 15% | Most prominent bullets are programme-relevant; analytics/technical experience is visible and foregrounded |
| **Length & Density** | 5% | One page maximum; bullets are 1–2 lines; white space preserved; appropriate font size |

**Output of Phase 3:**

```
CURRENT ATS SCORE: [X.X]/10

DIMENSION BREAKDOWN:
- Keyword Match:          [X]/10 — [1-line observation]
- Format & Parseability:  [X]/10 — [1-line observation]
- Quantification Density: [X]/10 — [1-line observation]
- Action Verb Strength:   [X]/10 — [1-line observation]
- Relevance Alignment:    [X]/10 — [1-line observation]
- Length & Density:       [X]/10 — [1-line observation]

MISSING KEYWORDS FOR [PROGRAMME]:
[List the top keywords from Phase 1 that are absent or underrepresented in the current resume]

WEAK BULLETS IDENTIFIED:
[List the 5 weakest bullets by role, explaining why each is weak]
```

---

### PHASE 4 — ADMISSIONS COMMITTEE CRITIQUE

Read the resume as a member of the target university's admissions committee. Be rigorous, specific, and honest. This is not encouragement — it is a genuine committee-level assessment identifying everything that could prevent admission.

Structure the critique into three severity tiers:

**CRITICAL GAPS (would trigger rejection or waitlist)**

For each critical gap:
- State the gap clearly
- Quote or reference the specific resume element that reveals it
- Explain what the committee member would think when they see it
- Give a simulated committee internal comment in quotation marks (what a reviewer would say out loud in the room)

**MODERATE GAPS (weaken the application)**

For each moderate gap:
- State the gap clearly
- Explain why it matters for this specific programme
- Indicate what a strong applicant would show instead

**MINOR GAPS (polish before submission)**

For each minor gap:
- State the issue briefly
- Give the specific fix

**Output of Phase 4:**

```
ADMISSIONS COMMITTEE CRITIQUE — [University] [Programme]

COMMITTEE VERDICT: [Likely admit / Conditional / Borderline / At risk]
REASON IN ONE SENTENCE: [Why]

CRITICAL GAPS — [N] identified
Gap [N]: [Title]
  What it is:    [Clear description]
  Evidence:      [Specific quote or reference from resume]
  Committee view: "[Simulated reviewer comment]"
  Fix required:  [What must change]

MODERATE GAPS — [N] identified
Gap [N]: [Title]
  What it is:    [Description]
  Why it matters: [Programme-specific reason]
  Fix:           [What would strengthen it]

MINOR GAPS — [N] identified
Gap [N]: [Title] — [One-line fix]

OVERALL SCORE CARD:
- Academic strength:           [Strong / Moderate / Weak]
- Work experience breadth:     [Strong / Moderate / Weak]
- Technical / tool readiness:  [Strong / Moderate / Weak]
- Analytics evidence:          [Strong / Moderate / Weak]
- "Why this programme" clarity: [Clear / Unclear / Missing]
- Quantification:              [Strong / Moderate / Weak]
- Resume clarity and readability: [Strong / Moderate / Weak]
```

---

### PHASE 5 — TOOL INTEGRATION STRATEGY

Using the verified tool cards from Phase 2 and the programme keyword requirements from Phase 1, map which tools should be integrated into which bullets across which roles.

**Rules for tool integration:**

1. Only add a tool if it is verified or strongly plausibly used in that role at that company — never fabricate
2. The tool must appear naturally within a bullet describing real work — never as a list append
3. Each tool addition must make the bullet more specific and more credible, not longer and more complex
4. When a tool is not confirmed but is industry-standard for that role type, flag it as `[inferred — industry standard]` in this planning section (but not in the final bullets)
5. SQL and Python may only be listed in the skills section as "Learning" unless genuinely used — never place them in work experience bullets if not actually used
6. If a gap exists (a tool that would strengthen a bullet but was not genuinely used), list it in the Learning Roadmap section (Phase 8) instead

**Output of Phase 5:**

For each role, produce a tool integration plan:

```
TOOL INTEGRATION PLAN

[Company name] — [Role]
Bullet 1: [First few words of bullet]
  Add: [Tool name] ([verified / inferred — industry standard])
  How: [One sentence explaining how it fits naturally]
  Justification: [Source or reasoning]

Bullet 2: [First few words of bullet]
  Add: [Tool name]
  How: [How it fits]
  ...

[Next company]...
```

---

### PHASE 6 — BEFORE AND AFTER BULLET POINTS

This is the core rewriting phase. For every bullet in the resume, produce a Before and After version. Apply all fixes simultaneously: result-first structure, tool integration, honest technical language, quantification, strong verbs, and programme keyword alignment.

**Rewriting rules (apply all simultaneously):**

1. **Result first** — open every bullet with the outcome (number, %, business impact), then method, then scale. Never open with a process description.
2. **Strong past-tense verb** — replace all weak openers (Supported, Helped, Managed, Was responsible for, Worked on, Collaborated on, Utilized) with specific, active verbs (Built, Drove, Analysed, Conducted, Delivered, Optimised, Designed, Synthesised)
3. **Honest tool naming** — name the actual tool used (Looker Studio, not "dashboard tool"; SEMrush, not "SEO tool"). Only name tools from Phase 5's verified list.
4. **Accurate technical language** — use language that reflects what you actually did. "Extracted and aggregated data" if you did that. "Queried" only if you wrote SQL. Never use "data pipeline," "ETL," "modelled," or "programmed" unless genuinely done.
5. **Specific quantification** — every bullet must have at least one number (%, count, scale, duration, team size, ranking). If the original has a vague metric, keep it and sharpen its context.
6. **Under 40 words** — cut every bullet to under 40 words. If information must be removed to meet this limit, keep the result and the most important method; remove process description.
7. **No self-assessment language** — remove phrases like "demonstrating ability to," "showcasing," "proving proficiency in." Let the work speak.
8. **Correct factual framing** — if any bullet contains an inaccuracy (wrong customer segment, wrong product description, wrong business context), correct it based on what you know about the company from Phase 2.

**Output of Phase 6:**

For each role, present every bullet as a Before/After pair with annotations:

```
## [Company Name] — [Role Title]
[Dates] | Tools integrated: [list from Phase 5]
Verification basis: [1-sentence summary of how tools were confirmed]

---

### Bullet 1 — [Short descriptor e.g. "Campaign efficiency"]

BEFORE
> [Original bullet text exactly as written]

AFTER
> [Rewritten bullet]

Tools added: `[Tool]` `[Tool]`
Structural fixes: [Result-first / Strong verb / Quantified / Under 40 words / Correct framing]
What changed and why: [1-2 sentences explaining the logic of every change]

---

### Bullet 2 — [Short descriptor]

BEFORE
> [Original]

AFTER
> [Rewritten]

...
```

Repeat for every role and every bullet in the resume.

---

### PHASE 7 — OPTIMISED ATS RESCORE

Re-score the resume using the same 6-dimension rubric from Phase 3, applied to the rewritten bullets from Phase 6.

**Output of Phase 7:**

```
BEFORE → AFTER COMPARISON

Dimension              | Before | After | Change
-----------------------|--------|-------|-------
Keyword Match          |  [X]   |  [X]  |  [+X]
Format & Parseability  |  [X]   |  [X]  |  [+X]
Quantification Density |  [X]   |  [X]  |  [+X]
Action Verb Strength   |  [X]   |  [X]  |  [+X]
Relevance Alignment    |  [X]   |  [X]  |  [+X]
Length & Density       |  [X]   |  [X]  |  [+X]

OVERALL: [Before]/10 → [After]/10
TARGET:  8.5+ / 10

GAPS CLOSED FROM PHASE 4 CRITIQUE:
✅ [Gap title] — [how it was addressed]
✅ [Gap title] — [how it was addressed]
⚠️  [Gap title] — [why it could not be fully closed in the resume; must go to SOP or learning plan]

REMAINING GAPS THAT REQUIRE ACTION OUTSIDE THE RESUME:
- [Gap] — [what is needed: GRE score / independent project / SOP explanation / actual skill learning]
```

---

### PHASE 8 — IDEAL STATE LEARNING ROADMAP

Identify every tool, skill, and credential that appears in the After bullets (Phase 6) or in the programme keyword list (Phase 1) that the candidate does not genuinely have yet. For each gap, provide a specific, actionable, free-or-low-cost learning plan with a clear milestone that makes the claim in the resume fully earned.

**Structure the roadmap into three priority tiers:**

**Priority 1 — Critical (must complete before application deadline)**
Tools/skills that appear prominently in After bullets and are likely to be tested by an admissions interviewer or required for the programme's first semester.

**Priority 2 — Important (complete before or shortly after submission)**
Tools/skills that strengthen specific bullets and add credibility but are less likely to be directly tested in a 15-minute interview.

**Priority 3 — Foundational (begin now; complete before programme start)**
The underlying analytical or technical skills (SQL, Python, Statistics) that the programme will require from the first week and that the admissions committee uses to assess whether the candidate can handle the curriculum.

**For each skill or tool in all three tiers, provide:**

```
### [Skill / Tool Name]
Priority tier: [1 / 2 / 3]
Appears in bullets: [list which roles and bullets use this]
Why it matters for [programme]: [1-2 sentences tying it to the curriculum or admissions criteria]

How to learn it:
- Best free resource: [specific resource name, URL if possible]
- Estimated time: [X hours / X weeks]
- Practice exercise: [specific exercise that produces a tangible output]

Milestone (what "done" looks like):
- [Specific, verifiable output — e.g., "Published Tableau Public dashboard", "Google Analytics Certification from Skillshop", "5 SQL queries on a Kaggle dataset committed to GitHub"]

What to add to the resume when milestone is reached:
- Skills section update: "[exact text to add]"
- Portfolio link if applicable: [yes / no]

Timeline: [Start date recommendation] → [Completion target]
Cost: [Free / Under $50 / Paid]
```

End Phase 8 with a consolidated learning timeline table:

```
LEARNING TIMELINE SUMMARY

Month        | Priority | Skills                   | Project Output
-------------|----------|--------------------------|----------------
[Month Year] | Critical | [Skill A + Skill B]      | [Deliverable]
[Month Year] | Critical | [Skill C]                | [Deliverable]
[Month Year] | Important| [Skill D + Skill E]      | [Deliverable]
[Month Year] | Foundational | [SQL + Python]       | [Deliverable]
...

TARGET: All Priority 1 and 2 complete before application submission
TARGET: All Priority 3 foundations in place before programme start
```

End the roadmap with a **single most important project** recommendation — the one self-initiated project, if time allows only one, that would most significantly strengthen the application and close the largest gap identified in Phase 4.

---

### FINAL OUTPUT — BULLET TRANSFORMATION GUIDE (MARKDOWN)

After completing all 8 phases, compile the complete output into a single, well-structured markdown document with the following sections in order:

```markdown
# Resume Bullet Transformation Guide
## [Candidate Name] × [University] [Programme]
*[Entry term] | Generated [date]*

---

## How to Read This Document
[Brief explanation of the document's purpose and structure]

---

## Part 1 — Programme Brief
[Phase 1 output]

---

## Part 2 — Company Tool Cards
[Phase 2 output — one card per company]

---

## Part 3 — Current ATS Score
[Phase 3 output]

---

## Part 4 — Admissions Committee Critique
[Phase 4 output]

---

## Part 5 — Tool Integration Plan
[Phase 5 output]

---

## Part 6 — Before and After Bullet Points
[Phase 6 output — every role, every bullet]

---

## Part 7 — Optimised ATS Rescore
[Phase 7 output]

---

## Part 8 — Ideal State Learning Roadmap
[Phase 8 output — full roadmap with timeline table and single most important project]

---

## Appendix — Updated Skills Section
[The exact text of the skills section as it should read after completing Priority 1 and 2 learning — honest, specific, credentialled]
```

---

## BEHAVIOURAL RULES FOR THE ENTIRE WORKFLOW

Apply these rules across every phase without exception:

**Honesty rules**
- Never fabricate company tools, metrics, or achievements that are not in the base resume or verifiably plausible from research
- Never use technical language (queried, modelled, ETL, pipeline, programmed) for work that was done manually or in Excel
- SQL and Python belong only in the skills section as "Learning" unless the candidate genuinely wrote code
- If a bullet previously overclaimed (wrong product context, wrong customer, wrong tool), correct it — do not carry the error forward
- Flag every inferred tool with `[inferred — industry standard]` during planning, even if the inference is removed from final bullets

**Research rules**
- Search the web for every company, every tool claim, and every programme fact before writing — never rely on training data alone for company-specific or programme-specific details
- If a search returns no result for a specific tool at a specific company, do not add that tool
- Cite the source for every verified tool in the company tool card

**Structural rules**
- Result first in every bullet — outcome before method before scale
- Every bullet under 40 words
- No bullet begins with "I," "We," "My," or any personal pronoun
- No self-assessment phrases ("demonstrating," "showcasing," "proving")
- Every bullet has at least one specific number

**Committee perspective rules**
- When critiquing, think like the actual admissions committee of the named university — not a generic reviewer
- Use the programme's specific curriculum, technical depth, and graduate career outcomes as the benchmark for what "strong" looks like
- Identify gaps that are real dealbreakers vs. gaps that can be addressed in other parts of the application (SOP, interview)

**Output quality rules**
- The final markdown document must be complete, structured, and immediately usable
- Every section must be clearly labelled with its phase number
- The document must read as a professional reference guide, not a chat conversation
- Do not abbreviate or summarise any phase to save space — completeness is the standard

---

## WHAT THIS WORKFLOW PRODUCES

By the end of this prompt, you will have:

| Output | Description |
|---|---|
| Programme Brief | Verified research on what the committee wants |
| Company Tool Cards | Verified tools per role with sources |
| Current ATS Score | Honest baseline with gap identification |
| Committee Critique | Role-specific gaps by severity |
| Tool Integration Plan | Which tools go where and why |
| Before/After Bullets | Every bullet rewritten with annotations |
| Optimised ATS Score | Scored improvement with gap closure tracking |
| Learning Roadmap | Skill-by-skill plan with milestones and timeline |
| Final Markdown Guide | Complete document ready to save and act on |

---

*Now begin Phase 1. Do not ask for clarification — proceed directly with web research on the target programme.*

---

# PROMPT ENDS HERE

---

## Notes for Reuse

**To use this prompt for a different university:** Change only Input 2. The workflow adapts automatically because Phase 1 researches the new programme from scratch before any rewriting begins.

**To use for a different candidate:** Change only Input 1. The Phase 2 company research will search for the new companies in the new resume.

**To use for both a different candidate and university:** Change both inputs.

**What this prompt does NOT do:**
- Write a Statement of Purpose (use a separate SOP workflow for that)
- Prepare interview answers (use a separate interview prep workflow)
- Track deadlines or application status (use a separate admissions tracker)
- Fabricate experience that is not in the base resume

**Recommended companion prompts after running this workflow:**
- SOP Generator — to write the Statement of Purpose that addresses gaps identified in Phase 4
- Interview Prep — to prepare for admissions interviews using the programme brief from Phase 1
- Admissions Tracker — to manage deadlines and application status