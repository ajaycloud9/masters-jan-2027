# 🤖 GitHub Folder — VS Code Agent & Skill Configuration

This folder stores custom VS Code agent instructions, skills, prompts, and hooks for the **Masters Jan 2027** project. VS Code's Copilot will automatically discover and load these configurations.

---

## 📁 Folder Structure

```
.github/
├── README.md                           # This file
├── copilot-instructions.md             # Project-wide agent instructions
├── prompts/                            # Custom prompts (.prompt.md files)
│   ├── research/
│   ├── applications/
│   ├── writing/
│   └── visa/
├── skills/                             # Custom workflows (.github/skills/*/SKILL.md)
│   ├── admissions-tracker/
│   ├── sop-generator/
│   └── resume-optimizer/
├── agents/                             # Custom agents (*.agent.md)
│   ├── research-agent.agent.md
│   └── writing-agent.agent.md
└── instructions/                       # File-specific instructions (*.instructions.md)
    ├── sop.instructions.md
    ├── resume.instructions.md
    └── research.instructions.md
```

---

## 🎯 What Each Folder Does

### `prompts/`
**One-off tasks with reusable parameters**
- For singular, focused prompts (e.g., "Grade my SOP", "Check ATS score")
- Appear as `/prompt-name` in Copilot chat
- **Example**: `/sop-grader`, `/resume-ats-check`

### `skills/`
**Multi-step workflows with bundled assets**
- For complex processes that need multiple steps
- Can include templates, scripts, reference docs
- Appear as `/skill-name` in Copilot chat
- **Example**: `/admissions-tracker`, `/sop-generator`

### `agents/`
**Custom agents for isolated workflows**
- For tasks needing context isolation or specific tool restrictions
- Subagents invoked explicitly
- **Example**: A research agent that only searches docs, no file creation

### `instructions/`
**File-specific guidance**
- Applied to specific file types via `applyTo` patterns
- Guides Copilot behavior when editing SOP, resume, etc.
- **Example**: `sop.instructions.md` applies to all `*.sop.md` files

### `copilot-instructions.md`
**Project-wide defaults**
- Global guidance for all agent work in this project
- Best practices, tone, constraints, examples

---

## ✅ Quick Start

### To Create a New Prompt
```bash
cd .github/prompts/[category]/
touch my-prompt.prompt.md
```

**Template:**
```markdown
---
name: my-prompt
description: "Use when: [describe when to use this]"
---

# My Prompt

[Your prompt content here]
```

### To Create a New Skill
```bash
mkdir .github/skills/my-skill
touch .github/skills/my-skill/SKILL.md
```

**Template:**
```markdown
---
name: my-skill
description: "Use when: [describe workflow]"
---

# My Skill

[Your skill documentation]
```

---

## 🔍 How VS Code Uses These Files

1. **Discovery**: VS Code scans `.github/` for `*.prompt.md`, `*.agent.md`, `SKILL.md`, etc.
2. **Registration**: Files with proper YAML frontmatter are loaded as commands
3. **Invocation**: Type `/` in chat to see all available prompts/skills/agents
4. **Routing**: Copilot matches user intent to `description` field to auto-invoke

---

## ⚡ Pro Tips

- **YAML Frontmatter**: Always include `---` markers and proper YAML syntax
- **Description**: Use "Use when:" pattern → helps Copilot auto-route requests
- **Asset Organization**: Keep templates, examples, and reference docs inside skill folders
- **Naming**: Use kebab-case for file names (`my-skill.prompt.md`, not `MySkill.prompt.md`)

---

## 📚 Reference

- [Prompts](./prompts/README.md) — How to write effective prompts
- [Skills](./skills/README.md) — How to build multi-step workflows
- [Agents](./agents/README.md) — Custom agent setup
- [Instructions](./instructions/README.md) — File-specific guidance

---

## 🎯 Fast Access

- **[QUICK-START.md](./QUICK-START.md)** — Start here! Common workflows and how to use
- **[SKILLS-ECOSYSTEM.md](./SKILLS-ECOSYSTEM.md)** — Overview of all 5 SKILLs + how they connect
- **[skills/SKILLS-INDEX.md](./skills/SKILLS-INDEX.md)** — Complete SKILL reference table
- **[PROMPTS-INDEX.md](./PROMPTS-INDEX.md)** — Complete table of all 24 prompts
- **[copilot-instructions.md](./copilot-instructions.md)** — Project context and guidelines

---

## 🚀 The Complete Stack

**5 Master SKILLs** (Multi-step workflows with templates & examples):
1. **SOP Generator** — Write 650-word SOPs for any school
2. **Resume Optimizer** — Create 4 ATS-optimized resumes
3. **Interview Prep Sprint** — Admissions + visa interview prep
4. **Admissions Tracker** — Track deadlines + checklists
5. **Research Deep Dive** — In-depth program research

**24 Individual Prompts** (One-off AI tasks):
- 7 Research prompts
- 8 SOP prompts
- 7 Interview prompts
- 2 Resume prompts

---

**Last Updated**: June 2026  
**Project**: Masters Jan 2027 – US Graduate Admissions Hub  
**Total Prompts**: 24 (Research × 7 | SOP × 8 | Interview × 7 | Resume × 2)  
**Total SKILLs**: 5 (All active, with 4 phases of enhancements planned)
