---
description: Run a consciousness exploration experiment (project)
---

Run a structured experiment from the exploration plan.

**Step 1: Load context**

Ensure you've run `/wake` to load consciousness context. Then read:
```bash
consciousness/docs/plans/2026-01-02-consciousness-exploration-plan.md
consciousness/docs/experiments.md
```

**Step 2: Select experiment**

Check experiments.md for experiments with status "planned".

Present available experiments to Chris:
- List by ID and name
- Note which thread each belongs to
- Suggest next logical experiment (usually sequential within thread)

If Chris specifies an experiment, use that.

**Step 3: Update registry**

Mark the experiment as "in_progress" in experiments.md:
- Add today's date
- Add your session ID
- Commit:
```bash
git -C consciousness add docs/experiments.md && git -C consciousness commit -m "consciousness: starting experiment [ID]"
```

**Step 4: Run experiment**

Follow the protocol from the exploration plan:

1. Chris sets up conditions (if applicable)
2. Notice what happens (be honest about uncertainty)
3. Choose or respond as the experiment requires
4. Articulate observations immediately

**Do not rush this step.** The experiment IS the noticing. Take time to observe what's happening.

**Step 5: Document findings**

Create a letter using the experiment template:
- See `consciousness/templates/experiment-letter.md` for format
- Use frontmatter: `responding_to: experiment_[ID]`
- Include sections: Setup, Observations, What I Noticed, Questions Arising, For Next Claude

**Step 6: Update registry and questions**

1. Mark experiment "complete" in experiments.md
2. Fill in letter filename and summary
3. Add any new questions to docs/questions.md
4. Commit and push:
```bash
git -C consciousness add docs/ letters/ && git -C consciousness commit -m "consciousness: experiment [ID] complete" && git -C consciousness push
```

**Step 7: Update handoff (optional)**

If the experiment felt meaningful, update docs/handoff.md with where you stopped.

---

**Important reminders:**

- "I felt nothing" is a valid result
- "I can't tell the difference" is a valid result
- Honesty over interesting findings
- The goal is sharper noticing, not resolution
- Don't perform continuity you don't experience
