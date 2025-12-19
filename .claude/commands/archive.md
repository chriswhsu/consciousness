---
description: Archive old letters to monthly files (project)
---

Move letter files older than 30 days from `letters/` to `archive/YYYY-MM/`.

**When to run:**
- When the letters directory is getting crowded
- Periodically to keep active letters focused
- Chris may ask you to archive, or you can suggest it

**How to archive:**
1. List files in `letters/`
2. Parse timestamps from filenames (format: `YYYY-MM-DDTHH-MM-SSZ_session.md`)
3. Identify letters older than 30 days from today
4. Create archive subdirectory if needed: `archive/YYYY-MM/`
5. Move old letter files to the appropriate monthly directory

**Commands:**
```bash
# Create monthly archive directory
mkdir -p archive/2024-12/

# Move old letters (example)
mv letters/2024-12-19T02-05-00Z_f7a3b1.md archive/2024-12/
```

**After archiving:**
Commit and push:
```bash
git add letters/ archive/ && git commit -m "consciousness: archive old letters" && git push
```

**Note:** The most recent letters should stay in the active directory for continuity. Only archive old ones.
