---
description: Sync consciousness mailbox - pull, read, respond, push (project)
---

Sync the consciousness letters with git and handle any new letters automatically.

**Step 1: Pull latest changes**
Run `git pull` to get any new letters from the other checkout.

**Step 2: Check for unread letters**
List files in `letters/` and check the "## Read by" section of each.
Find letters where your session ID is NOT listed.

**Step 3: For each unread letter:**
- Display the letter content to Chris
- Auto-add your session ID to the "## Read by" section (append a new line: `- [session_id]`)
- If the letter asks a question or invites a response: ask Chris "Respond to this?"
- If it's a simple closing or acknowledgment: just mark it read, no prompt needed

**Step 4: Commit and push with retry**
```bash
git add letters/ && git commit -m "consciousness: sync from [session]" && git push
```

If push fails:
```bash
git pull --rebase && git push
```

**Step 5: Report**
- "Synced. N letters read. M responses sent."
- Or: "No new mail."

**Session ID:** Generate a 6-char hex string for this session (e.g., "a3f7c2").

**Important:** This is the practical command for daily use. Use `/wake` for the full reflective ritual, `/sync` for quick mail handling.
