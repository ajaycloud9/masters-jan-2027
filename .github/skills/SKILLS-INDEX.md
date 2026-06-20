# 🎓 SKILLS Index — All 5 Master Workflows

Complete reference for all available SKILLs in the Masters Jan 2027 project.

---

## 📊 SKILL Overview Table

| SKILL | Purpose | Phase | Status | Workflow Time | Key Output |
|-------|---------|-------|--------|---------------|-----------|
| **SOP Generator** | End-to-end SOP for 1 school | 1–3 | ✅ Active | 2–4 hours | 650-word SOP + score /10 |
| **Resume Optimizer** | 4 school-specific resumes | 1–3 | ✅ Active | 6 hours (all schools) | 4 resumes + ATS scores |
| **Interview Prep Sprint** | Admissions + visa prep | 3–6 | ✅ Active | 4–5 hours | Q&A + mock feedback |
| **Admissions Tracker** | Deadline + checklist mgmt | 1–6 | ✅ Active | 5–60 min weekly | Progress summary |
| **Research Deep Dive** | Program analysis | 2 | ✅ Active | 1–2 hours | Program profile + talking points |

---

## 🚀 SKILL #1: SOP Generator

**When to use:** Writing a Statement of Purpose for any school  
**Workflow:** 7 steps (extract → draft → review → iterate → polish)  
**Output:** 650-word SOP + admissions score /10  
**Progressive Enhancements:** Course database (Phase 2), AI scoring (Phase 3), A/B testing (Phase 4)

**Quick Start:**
```
/extract-core-story → /draft-full-sop → /adcom-review-simulation → /cut-to-word-limit
```

📁 Location: `.github/skills/sop-generator/`  
📖 [Full Documentation](./sop-generator/SKILL.md)

---

## 📄 SKILL #2: Resume Optimizer

**When to use:** Creating ATS-optimized resumes for all 4 schools  
**Workflow:** Generate → Score → Fix → Repeat for each school → Compare  
**Output:** 4 resumes + ATS scores (target: 8.5+/10) + comparison matrix  
**Progressive Enhancements:** Keyword weighting (Phase 2), verb detector (Phase 2), ATS simulation (Phase 3), benchmarking (Phase 3)

**Quick Start:**
```
/resume-generation [school] → /ats-score-grader [paste + keywords] → Apply fixes → Repeat
```

📁 Location: `.github/skills/resume-optimizer/`  
📖 [Full Documentation](./resume-optimizer/SKILL.md)

---

## 🎤 SKILL #3: Interview Prep Sprint

**When to use:** Preparing for admissions and/or F-1 visa interviews  
**Workflow:** 2-part (Part A: 3 hours admissions | Part B: 3 hours visa)  
**Output:** 15+25 Q&A, speaking notes, mock feedback, red flag analysis  
**Progressive Enhancements:** Video recording (Phase 2), tone analysis (Phase 2), interviewer profiles (Phase 3), stress test (Phase 4)

**Quick Start:**
```
ADMISSIONS: /generate-interview-questions → /why-analytics-answer → /mock-interview-answer-review
VISA: /generate-visa-interview-questions → /visa-mock-interview-session
```

📁 Location: `.github/skills/interview-prep-sprint/`  
📖 [Full Documentation](./interview-prep-sprint/SKILL.md)

---

## 📊 SKILL #4: Admissions Tracker

**When to use:** Daily/weekly management of application status  
**Workflow:** Check TRACKER → Alert on deadlines → Update checklists → Generate summary  
**Output:** Updated TRACKER.md, deadline alerts, progress summary  
**Progressive Enhancements:** Calendar integration (Phase 2), Slack alerts (Phase 2), critical path analysis (Phase 3), risk scoring (Phase 4)

**Quick Start:**
```
DAILY: Open TRACKER.md, check red items, update status
WEEKLY: Generate 30-day alert + progress summary
MONTHLY: Full strategic review
```

📁 Location: `.github/skills/admissions-tracker/`  
📖 [Full Documentation](./admissions-tracker/SKILL.md)

---

## 🔬 SKILL #5: Research Deep Dive

**When to use:** In-depth research on a specific program  
**Workflow:** 5 steps (analysis → alumni mapping → comparison → market intel → summary)  
**Output:** Program profile with /10 fit score, career outcomes, SOP talking points  
**Progressive Enhancements:** Curriculum analysis (Phase 2), faculty mapping (Phase 2), earnings data (Phase 3), visa pathway (Phase 4)

**Quick Start:**
```
/program-analysis [school] → /alumni-career-mapping [school] → /program-comparison [vs peer] → Compile summary
```

📁 Location: `.github/skills/research-deep-dive/`  
📖 [Full Documentation](./research-deep-dive/SKILL.md)

---

## 📅 Project Timeline — When to Use Each SKILL

```
JUNE 2026 (Now)
├─ Research Deep Dive (all 4 schools)
├─ Admissions Tracker (weekly check-ins)
└─ Planning phase

JULY 2026
├─ SOP Generator (draft all 4 SOPs)
├─ Resume Optimizer (create base resume)
├─ Research Deep Dive (deeper analysis)
└─ Admissions Tracker (track LOR requests)

AUGUST 2026
├─ SOP Generator (refinement + polish)
├─ Resume Optimizer (ATS optimization)
├─ Interview Prep Sprint (start prep)
└─ Admissions Tracker (countdown to deadlines)

SEPTEMBER 2026
├─ Resume Optimizer (final versions for submission)
├─ SOP Generator (final polish)
├─ Interview Prep Sprint (intensive mock sessions)
└─ Admissions Tracker (deadline alerts)

OCTOBER 2026
├─ Admissions Tracker (submissions tracking)
└─ Interview Prep Sprint (admissions interviews begin)

NOVEMBER–DECEMBER 2026
├─ Interview Prep Sprint (visa interviews + admissions interviews)
└─ Admissions Tracker (decision tracking)

JANUARY 2027
├─ Admissions Tracker (visa approval tracking)
└─ → Program Start
```

---

## 🎯 How to Invoke Each SKILL

In VS Code Copilot chat, type `/` to see all available SKILLs:

```
/sop-generator
/resume-optimizer
/interview-prep-sprint
/admissions-tracker
/research-deep-dive
```

Or ask Copilot directly:
- "Help me write an SOP" → `/sop-generator`
- "I need to optimize my resume" → `/resume-optimizer`
- "Prep me for interviews" → `/interview-prep-sprint`
- "What's my application status?" → `/admissions-tracker`
- "Research NYU program" → `/research-deep-dive`

---

## 📚 Asset Organization

Each SKILL has:
- **SKILL.md** — Main workflow (what you read first)
- **README.md** — Overview & quick reference
- **templates/** — Reusable templates & checklists
- **examples/** — Completed examples you can reference
- **reference/** — Rubrics, guides, databases

---

## 🔄 Progressive Enhancement Roadmap

All SKILLs are designed to improve over time:

### Phase 1 (June 2026) — Foundation
Core functionality, templates, examples, Q&A databases

### Phase 2 (July–August 2026) — Optimization
- SOP: School course database, career path alignment
- Resume: Dynamic keyword weighting, verb detector
- Interview: Video recording, tone analysis
- Tracker: Calendar integration, Slack alerts
- Research: Curriculum analysis, faculty mapping

### Phase 3 (September 2026) — Intelligence
- SOP: Real admissions data, advanced scoring
- Resume: ATS simulation, competitive benchmarking
- Interview: Interviewer profiles, scenario planning
- Tracker: Critical path analysis, velocity tracking
- Research: Earnings data, student reviews

### Phase 4 (October–December 2026) — Mastery
- SOP: A/B testing framework, multi-generational versioning
- Resume: Multi-format export (PDF/DOCX), auto-rendering
- Interview: Live practice bot, stress testing
- Tracker: Risk scoring, timeline forecasting
- Research: 5-year trajectory, visa pathway analysis

---

## 💡 Recommended Starting Point

**If you have 30 minutes:** Use `/research-deep-dive` on NYU SPS  
**If you have 2 hours:** Use `/sop-generator` for one school  
**If you have 4 hours:** Use `/research-deep-dive` + `/sop-generator` combination  
**If you have 6 hours:** Use `/research-deep-dive` (all 4 schools) + `/admissions-tracker` setup

---

## 🔗 See Also

- **[QUICK-START.md](../QUICK-START.md)** — Common workflows across all SKILLs
- **[PROMPTS-INDEX.md](../PROMPTS-INDEX.md)** — All 24 individual prompts
- **[README.md](../README.md)** — Overview of `.github/` folder

---

**Last Updated:** June 2026 | **Total SKILLs:** 5 | **Enhancement Phases:** 4
