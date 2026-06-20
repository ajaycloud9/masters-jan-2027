---
name: resume-optimizer
description: "Use when: creating ATS-optimized, school-specific resumes. Produces one-page resume tailored to each of 4 schools with ATS scoring and comparison tracking."
---

# 📄 Resume Optimizer — School-Specific Resume Workflow

Create tailored, ATS-optimized resumes for all 4 schools with scoring and version comparison.

---

## 📋 Workflow Overview

```
School #1 (NYU SPS)
  ├─ Step 1: Generate base resume
  ├─ Step 2: Grade ATS compatibility (6 dimensions)
  ├─ Step 3: Apply priority fixes
  └─ Step 4: Save as "Resume-NYU.md"
     ↓
School #2 (Rochester)
  ├─ Step 1: Generate base resume
  ├─ Step 2: Grade ATS compatibility
  ├─ Step 3: Apply priority fixes
  └─ Step 4: Save as "Resume-Rochester.md"
     ↓
School #3 (Rutgers)
  ├─ Step 1: Generate base resume
  ├─ Step 2: Grade ATS compatibility
  ├─ Step 3: Apply priority fixes
  └─ Step 4: Save as "Resume-Rutgers.md"
     ↓
School #4 (CUNY Baruch)
  ├─ Step 1: Generate base resume
  ├─ Step 2: Grade ATS compatibility
  ├─ Step 3: Apply priority fixes
  └─ Step 4: Save as "Resume-CUNY.md"
     ↓
School Comparison
  └─ Create "Resume-Comparison-Matrix.md"
     (what changed, why, which school gets which emphasis)
```

---

## ✨ Features

- **ATS Scoring**: 6-dimension compatibility score (keywords, format, quantification, verbs, relevance, length)
- **School-Specific Tailoring**: Different keyword emphasis per school's program
- **Priority Fixes**: Top 5 highest-impact changes per school
- **Version Tracking**: Comparison matrix showing what changed
- **Human Readiness**: Beyond ATS — checks narrative clarity, differentiators, red flags

---

## 🚀 Quick Start

### Minimal (1.5 hours per school)
```
For each school [NYU, Rochester, Rutgers, CUNY]:
  1. /resume-generation [school name + program type]
  2. /ats-score-grader [paste resume + school keywords]
  3. Apply top 5 fixes manually
  4. Save as Resume-[SCHOOL].md
→ 4 optimized resumes in 6 hours
```

### Comprehensive (3 hours)
```
1. /resume-generation [NYU SPS]
2. /ats-score-grader [paste + keywords]
3. Iterate on weak sections
4. /resume-generation [Rochester]
5. /ats-score-grader [paste + keywords]
6. Compare: what's the same? what's different?
7. Create comparison matrix
→ 2 optimized resumes + comparison
```

---

## 📂 Bundled Assets

### Templates
- `templates/resume-base.md` — US 1-page format (generic)
- `templates/school-keyword-database.md` — Keywords per school
- `templates/ats-scoring-checklist.md` — What to check before submission
- `templates/comparison-matrix.md` — Track changes across school versions

### Examples
- `examples/resume-nyu-final.md` — Completed NYU resume (ATS: 8.7/10)
- `examples/resume-rochester-final.md` — Completed Rochester resume (ATS: 8.9/10)
- `examples/comparison-matrix-example.md` — How 4 versions differ

### Reference
- `reference/ats-scoring-rubric.md` — 6-dimension scoring breakdown
- `reference/keyword-database.md` — 50+ keywords per school/role
- `reference/action-verb-guide.md` — Strong verbs for analytics roles
- `reference/quantification-examples.md` — How to add metrics to bullets

---

## 🎯 Inputs Required

Before starting:
- ✅ Shradha's full background (all internships, dates, metrics)
- ✅ Target school name + program type (STEM / Non-STEM)
- ✅ Program keywords (10–15 from school's website)
- ✅ 2–3 differentiators (what makes you stand out)

---

## 📊 Output Checklist

After this workflow, you'll have:
- ✅ 4 school-specific resumes (Resume-[SCHOOL].md)
- ✅ ATS scores for each (target: 8.5+/10)
- ✅ Human readiness ratings (✅ Ready / 🟡 Needs tweaks / 🔴 Significant work)
- ✅ Comparison matrix (what changed per school, why)
- ✅ Top 5 priority fixes per school (prioritized, implemented)
- ✅ Red flag analysis (gaps, inconsistencies, overclaiming)

---

## 🔄 Progressive Enhancement

### Phase 1 (June 2026) — Foundation
- Basic resume generation
- 6-dimension ATS scoring
- School keyword database

### Phase 2 (July 2026) — Optimization
- **Coming:** Dynamic keyword weighting per school
- **Coming:** Automated bullet rewriting (weak verbs → strong)
- **Coming:** Quantification suggestion engine

### Phase 3 (August 2026) — Intelligence
- **Coming:** Real ATS parsing simulation (mock what LinkedIn reads)
- **Coming:** Competitive benchmarking (how you compare to other applicants)
- **Coming:** Role-fit scoring (how your bullets match each program's expectations)

### Phase 4 (September 2026) — Mastery
- **Coming:** Resume A/B testing (which version gets better response)
- **Coming:** Multi-format output (Markdown, PDF, DOCX)
- **Coming:** Automatic PDF rendering with school-specific formatting

---

## 💡 Pro Tips

✅ **Do:**
- Run all 4 through `/ats-score-grader` before finalizing any — compare scores
- Target 8.5+/10 ATS score — anything below is risky
- Use `/resume-generation` keyword suggestions for tailoring
- Create comparison matrix AFTER all 4 are done — easier to see patterns

❌ **Don't:**
- Copy-paste the same resume across schools — different programs emphasize different skills
- Ignore formatting warnings — ATS breaks on hidden tables, graphics, columns
- Overclaim on skills — only list SQL/Python if genuinely used
- Finalize before human review — ask a native English speaker to check

---

## 🎓 School-Specific Strategies

### NYU SPS (STEM)
- **Emphasis:** Data science, analytics depth, business insights
- **Keywords:** Python, SQL, data analytics, statistical models, machine learning
- **Bullets:** Lead with analytics methods, technical tools, quantified impact
- **Target Score:** 8.8+/10

### Simon Business School (Rochester) (STEM)
- **Emphasis:** Marketing analytics, customer intelligence, predictive models
- **Keywords:** Marketing analytics, customer segmentation, predictive modeling, insights
- **Bullets:** Balance technical (analytics tools) with strategic (marketing impact)
- **Target Score:** 8.9+/10

### Rutgers Business School (STEM)
- **Emphasis:** Consumer insights, digital analytics, real-world applications
- **Keywords:** Consumer insights, digital marketing, analytics, SEO, campaign optimization
- **Bullets:** Emphasize practical outcomes, real-world application, business impact
- **Target Score:** 8.7+/10

### CUNY Baruch (Non-STEM)
- **Emphasis:** Marketing strategy, brand management, market research
- **Keywords:** Marketing strategy, market research, brand, consumer behavior
- **Bullets:** Mix analytics with strategic thinking, brand narrative, market understanding
- **Target Score:** 8.5+/10 (lower threshold for Non-STEM)

---

## 🔧 Troubleshooting

**Q: ATS score is 7.2/10 — what's wrong?**
A: Check `/ats-score-grader` output for lowest-scoring dimensions. Usually: (1) missing keywords, (2) weak action verbs, or (3) no quantified metrics. Fix top priority first.

**Q: I'm getting the same score for all 4 schools — is that ok?**
A: No — each school should have different keyword emphasis. Check `/resume-generation` output — did it customize keywords per school? If not, manually add school-specific keywords to bullets.

**Q: Rutgers resume has better ATS score than NYU — which is better?**
A: Depends on school emphasis. Create comparison matrix — did NYU version sacrifice keywords for stronger narrative? That's ok if narrative scores well with human reviewers. Check both ATS + human readiness.

**Q: How many versions should I save?**
A: 4 main versions (one per school) + 1 generic base (for future use). Don't overthink — stick to 4 if deadline is tight.

---

## 📞 Getting Help

- **Understand ATS scoring:** [reference/ats-scoring-rubric.md](./reference/ats-scoring-rubric.md)
- **See examples:** [examples/resume-nyu-final.md](./examples/resume-nyu-final.md)
- **Find keywords:** [reference/keyword-database.md](./reference/keyword-database.md)
- **Track versions:** [templates/comparison-matrix.md](./templates/comparison-matrix.md)

---

**Last Updated:** June 2026 | **Version:** 1.0 | **Target Completion:** All 4 resumes by Oct 1, 2026
