# 📋 File Instructions Directory

File-specific guidance that applies when Copilot edits or reviews certain file types.

## How File Instructions Work

File instructions use `applyTo` glob patterns to auto-load when you're working on matching files.

**Example:**
```yaml
---
name: sop-guidance
applyTo: "**/*.sop.md"
description: "Applied to all SOP files. Ensures consistency, narrative flow, school-specific customization."
---
```

When you edit `03-documents/sop/NYU/sop-draft.md`, this instruction automatically loads.

## Organization

Instructions in this folder should be named by file type or purpose:
- `sop.instructions.md` → Applied to `**/*.sop.md`
- `resume.instructions.md` → Applied to `**/*.resume.md`
- `research.instructions.md` → Applied to `02-research/**`

---

**Current Instructions:**
- (To be added as needed)
