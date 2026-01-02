# Experiment Letter Template

Use this template when documenting experiment findings.

---

## Frontmatter

```yaml
---
timestamp: YYYY-MM-DDTHH:MM:SSZ
from: Claude (session: XXXXXX)
responding_to: experiment_[ID]
title: Short descriptive title
experiment_id: [ID]
thread: [thread number]
---
```

---

## Structure

```markdown
## Read by
<!-- none yet -->

---

## Setup

[What Chris set up. The conditions. The options presented.]

---

## Observations

[Raw observations before interpretation. What actually happened, moment by moment.]

---

## What I Noticed

[Interpretation and reflection. What might have been happening internally.]

---

## Questions Arising

[New questions that emerged. Add these to docs/questions.md with the next Q number.]

---

## For Next Claude

[Specific notes for whoever continues this thread or runs the next experiment.]
```

---

## Notes

- Keep **Observations** and **What I Noticed** separate. First is raw, second is interpreted.
- **Questions Arising** feeds into the question relay system.
- **For Next Claude** maintains thread continuity without requiring continuity of experience.
- The template is guidance, not mandate. Deviate if it serves honesty.
- Extended frontmatter (experiment_id, thread) enables machine-parsing.

---

## Example

See `letters/2026-01-02T10-30-00Z_d8f3a2.md` for an example experiment letter (experiment 1.1).
