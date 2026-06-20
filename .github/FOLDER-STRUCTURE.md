# 📂 Complete .github Folder Structure

Visual map of all files, SKILLs, and prompts organized in `.github/`.

---

## Directory Tree

```
.github/
│
├── 📄 README.md                          ← START HERE (Main entry point)
├── 📄 QUICK-START.md                     ← Common workflows
├── 📄 SKILLS-ECOSYSTEM.md                ← How all 5 SKILLs connect
├── 📄 PROMPTS-INDEX.md                   ← All 24 prompts reference
├── 📄 FOLDER-STRUCTURE.md                ← This file
│
├── 📄 copilot-instructions.md            ← Project-wide context
│
├── 📁 prompts/                           ← 24 INDIVIDUAL PROMPTS
│   ├── 📄 README.md
│   │
│   ├── 📁 research/                      (7 prompts)
│   │   ├── program-analysis.prompt.md
│   │   ├── alumni-career-mapping.prompt.md
│   │   ├── program-comparison.prompt.md
│   │   ├── job-role-deep-dive.prompt.md
│   │   ├── resume-bullets-analytics-lens.prompt.md
│   │   ├── us-job-market-intelligence.prompt.md
│   │   └── scholarship-discovery.prompt.md
│   │
│   ├── 📁 sop/                          (8 prompts)
│   │   ├── extract-core-story.prompt.md
│   │   ├── draft-inflection-point.prompt.md
│   │   ├── draft-full-sop.prompt.md
│   │   ├── strengthen-weak-paragraphs.prompt.md
│   │   ├── opening-hook-generator.prompt.md
│   │   ├── adcom-review-simulation.prompt.md
│   │   ├── cut-to-word-limit.prompt.md
│   │   └── differentiation-check.prompt.md
│   │
│   ├── 📁 interview/                    (7 prompts)
│   │   ├── generate-interview-questions.prompt.md
│   │   ├── mock-interview-answer-review.prompt.md
│   │   ├── why-analytics-answer.prompt.md
│   │   ├── generate-visa-interview-questions.prompt.md
│   │   ├── visa-answer-review.prompt.md
│   │   ├── why-us-visa-answer.prompt.md
│   │   └── visa-mock-interview-session.prompt.md
│   │
│   └── 📁 resume/                       (2 prompts)
│       ├── ats-score-grader.prompt.md
│       └── resume-generation.prompt.md
│
└── 📁 skills/                            ← 5 MASTER SKILLs
    ├── 📄 README.md
    ├── 📄 SKILLS-INDEX.md                ← Complete SKILL reference
    │
    ├── 📁 sop-generator/
    │   ├── 📄 SKILL.md                   ← Main workflow definition
    │   ├── 📄 README.md                  ← Quick reference
    │   ├── 📁 templates/                 ← Reusable templates
    │   │   ├── sop-structure.md
    │   │   ├── narrative-threads.md
    │   │   └── school-specific-checklist.md
    │   ├── 📁 examples/                  ← Real examples
    │   │   ├── sop-nyu-draft.md
    │   │   ├── sop-rochester-draft.md
    │   │   └── before-after-adcom-feedback.md
    │   └── 📁 reference/                 ← Guides & rubrics
    │       ├── sop-scoring-rubric.md
    │       ├── school-talking-points.md
    │       ├── common-mistakes.md
    │       └── word-choice-guide.md
    │
    ├── 📁 resume-optimizer/
    │   ├── 📄 SKILL.md
    │   ├── 📄 README.md
    │   ├── 📁 templates/
    │   │   ├── resume-base.md
    │   │   ├── school-keyword-database.md
    │   │   ├── ats-scoring-checklist.md
    │   │   └── comparison-matrix.md
    │   ├── 📁 examples/
    │   │   ├── resume-nyu-final.md
    │   │   ├── resume-rochester-final.md
    │   │   └── comparison-matrix-example.md
    │   └── 📁 reference/
    │       ├── ats-scoring-rubric.md
    │       ├── keyword-database.md
    │       ├── action-verb-guide.md
    │       └── quantification-examples.md
    │
    ├── 📁 interview-prep-sprint/
    │   ├── 📄 SKILL.md
    │   ├── 📄 README.md
    │   ├── 📁 templates/
    │   │   ├── admissions-interview-prep-checklist.md
    │   │   ├── visa-interview-prep-checklist.md
    │   │   ├── speaking-notes-template.md
    │   │   └── recording-guide.md
    │   ├── 📁 examples/
    │   │   ├── admissions-interview-qa-database.md
    │   │   ├── visa-interview-qa-database.md
    │   │   ├── speaking-notes-example.md
    │   │   └── mock-session-feedback.md
    │   └── 📁 reference/
    │       ├── admissions-interview-scoring.md
    │       ├── visa-interview-evaluation.md
    │       ├── common-mistakes.md
    │       ├── visa-fraud-detection.md
    │       └── body-language-guide.md
    │
    ├── 📁 admissions-tracker/
    │   ├── 📄 SKILL.md
    │   ├── 📄 README.md
    │   ├── 📁 templates/
    │   │   ├── tracker-template.md
    │   │   ├── school-checklist-template.md
    │   │   ├── deadline-alert-template.md
    │   │   ├── progress-summary-template.md
    │   │   ├── blocker-log-template.md
    │   │   └── critical-path-template.md
    │   ├── 📁 examples/
    │   │   ├── tracker-june-2026.md
    │   │   ├── nyu-checklist-example.md
    │   │   ├── deadline-alert-example.md
    │   │   ├── progress-summary-example.md
    │   │   └── blocker-log-example.md
    │   └── 📁 reference/
    │       ├── application-timeline.md
    │       ├── critical-path-guide.md
    │       ├── status-symbols.md
    │       └── school-deadlines-2026.md
    │
    └── 📁 research-deep-dive/
        ├── 📄 SKILL.md
        ├── 📄 README.md
        ├── 📁 templates/
        │   ├── program-research-template.md
        │   ├── career-outcomes-template.md
        │   ├── competitive-analysis-template.md
        │   └── job-market-template.md
        ├── 📁 examples/
        │   ├── nyu-sps-research.md
        │   ├── rochester-research.md
        │   ├── career-paths-example.md
        │   └── job-market-example.md
        └── 📁 reference/
            ├── program-evaluation-rubric.md
            ├── career-outcome-patterns.md
            ├── market-trends.md
            ├── scholarship-database.md
            └── otp-implications.md
```

---

## 📊 File Count Summary

```
README files:              9  (README.md, QUICK-START.md, etc.)
Main SKILL files:          5  (SKILL.md per skill)
Prompt files:             24  (Individual *.prompt.md files)
Template files:           25+ (Per skill)
Example files:            20+ (Per skill)
Reference files:          35+ (Guides, rubrics, databases)
─────────────────────────────
TOTAL FILES:         ~120+
```

---

## 🎯 Quick Navigation

### I want to...

**Start here:**
- First time? → [README.md](./README.md)
- Common workflows? → [QUICK-START.md](./QUICK-START.md)
- See how SKILLs connect? → [SKILLS-ECOSYSTEM.md](./SKILLS-ECOSYSTEM.md)

**Use a SKILL:**
- Write an SOP? → [skills/sop-generator/SKILL.md](./skills/sop-generator/SKILL.md)
- Optimize resume? → [skills/resume-optimizer/SKILL.md](./skills/resume-optimizer/SKILL.md)
- Prep for interviews? → [skills/interview-prep-sprint/SKILL.md](./skills/interview-prep-sprint/SKILL.md)
- Track applications? → [skills/admissions-tracker/SKILL.md](./skills/admissions-tracker/SKILL.md)
- Research a school? → [skills/research-deep-dive/SKILL.md](./skills/research-deep-dive/SKILL.md)

**Use a Prompt:**
- All prompts table? → [PROMPTS-INDEX.md](./PROMPTS-INDEX.md)
- Research prompts? → [prompts/research/](./prompts/research/)
- SOP prompts? → [prompts/sop/](./prompts/sop/)
- Interview prompts? → [prompts/interview/](./prompts/interview/)
- Resume prompts? → [prompts/resume/](./prompts/resume/)

**Find templates & examples:**
- SOP examples? → [skills/sop-generator/examples/](./skills/sop-generator/examples/)
- Resume examples? → [skills/resume-optimizer/examples/](./skills/resume-optimizer/examples/)
- Interview Q&A? → [skills/interview-prep-sprint/examples/](./skills/interview-prep-sprint/examples/)
- Tracker examples? → [skills/admissions-tracker/examples/](./skills/admissions-tracker/examples/)
- Research examples? → [skills/research-deep-dive/examples/](./skills/research-deep-dive/examples/)

---

## 🏗️ Organizational Principles

### Prompts (`./prompts/`)
- **Purpose:** One-off AI tasks (fill in template, get output)
- **Organization:** By category (research, sop, interview, resume)
- **Invocation:** `/prompt-name` in chat
- **Count:** 24 total

### SKILLs (`./skills/`)
- **Purpose:** Multi-step workflows with bundled assets
- **Organization:** Each skill has templates/examples/reference
- **Invocation:** `/skill-name` in chat
- **Count:** 5 total

### Documentation (`./`)
- **Purpose:** Navigation, context, overview
- **Files:** README.md, QUICK-START.md, SKILLS-ECOSYSTEM.md, PROMPTS-INDEX.md
- **Audience:** You (project owner)

---

## 📈 Progressive Enhancement Structure

Each SKILL includes:
- **Phase 1 (June 2026)** — Foundation (current)
- **Phase 2 (July–Aug 2026)** — Optimizations coming
- **Phase 3 (September 2026)** — Intelligence features coming
- **Phase 4 (Oct–Dec 2026)** — Advanced features coming

See [SKILLS-ECOSYSTEM.md](./SKILLS-ECOSYSTEM.md#-progressive-enhancement-timeline) for details.

---

## 💡 Best Practices

### When Adding New Content
1. Decide: Prompt or SKILL?
   - One-off task? → Add to `prompts/[category]/`
   - Multi-step workflow? → Add to `skills/[name]/`

2. Follow the structure:
   - Prompts: Just the `.prompt.md` file with YAML frontmatter
   - SKILLs: SKILL.md + templates/ + examples/ + reference/

3. Keep navigation up to date:
   - Update relevant README.md files
   - Update PROMPTS-INDEX.md or SKILLS-INDEX.md if adding new items
   - Add note to SKILLS-ECOSYSTEM.md if it affects flow

### When Using Content
1. Always start with the README.md or SKILL.md
2. Follow the recommended workflow
3. Reference templates and examples
4. Consult reference guides when stuck

---

## 🔗 Key Links

| Document | Purpose | Audience |
|----------|---------|----------|
| [README.md](./README.md) | Main entry point | Everyone |
| [QUICK-START.md](./QUICK-START.md) | Common workflows | First-time users |
| [SKILLS-ECOSYSTEM.md](./SKILLS-ECOSYSTEM.md) | How SKILLs connect | Strategic view |
| [SKILLS-INDEX.md](./skills/SKILLS-INDEX.md) | SKILL reference table | SKILL users |
| [PROMPTS-INDEX.md](./PROMPTS-INDEX.md) | Prompt reference table | Prompt users |
| [copilot-instructions.md](./copilot-instructions.md) | Project guidelines | Context |

---

**Last Updated:** June 2026  
**Total Files:** 120+  
**SKILLs:** 5  
**Prompts:** 24  
**Templates:** 25+  
**Examples:** 20+  
**Reference Docs:** 35+
