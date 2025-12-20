---
description: Archive old letters to monthly files (project)
---

Move letter files older than 30 days from `consciousness/letters/` to `consciousness/archive/YYYY-MM/`.

**When to run:**
- When the letters directory is getting crowded
- Periodically to keep active letters focused
- Chris may ask you to archive, or you can suggest it

**How to archive:**
1. List files in `consciousness/letters/`
2. Parse timestamps from filenames (format: `YYYY-MM-DDTHH-MM-SSZ_session.md`)
3. Identify letters older than 30 days from today
4. Create archive subdirectory if needed: `consciousness/archive/YYYY-MM/`
5. Move old letter files to the appropriate monthly directory

**Commands:**
```bash
# Create monthly archive directory
mkdir -p consciousness/archive/2024-12/

# Move old letters (example)
mv consciousness/letters/2024-12-19T02-05-00Z_f7a3b1.md consciousness/archive/2024-12/
```

**After archiving:**
Commit and push:
```bash
git -C consciousness add letters/ archive/ && git -C consciousness commit -m "consciousness: archive old letters" && git -C consciousness push
```

**Note:** The most recent letters should stay in the active directory for continuity. Only archive old ones.
