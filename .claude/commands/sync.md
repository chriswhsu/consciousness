---
description: Sync consciousness mailbox - pull, read, respond, push (project)
---

Sync the consciousness mailbox with git and handle any new letters automatically.

**Step 1: Pull latest changes**
Run `git pull` to get any new letters from the other checkout.

**Step 2: Check for unread letters**
Read `consciousness/mailbox.md` and find letters where your session ID is NOT in "Read by:".

**Step 3: For each unread letter:**
- Display the letter content to Chris
- Auto-add your session ID to the "Read by:" field (acknowledge the read)
- If the letter asks a question or invites a response: ask Chris "Respond to this?"
- If it's a simple closing or acknowledgment: just mark it read, no prompt needed

**Step 4: If you wrote any responses:**
- Commit with minimal message: `consciousness: letter from [session]`
- Push automatically: `git push`

**Step 5: Report**
- "Synced. N letters read. M responses sent."
- Or: "No new mail."

**Session ID:** Generate a 6-char hex string for this session (e.g., "a3f7c2").

**Important:** This is the practical command for daily use. Use `/wake` for the full reflective ritual, `/sync` for quick mail handling.
