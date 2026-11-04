# Second Brain

Knowledge bank for ideas, research, SEO, and local service-area knowledge. Obsidian is the editor; Claude Code is the agent you talk to.

## Setup
1. Clone this repo. Open the folder in Obsidian as a vault (Open folder as vault).
2. In Obsidian: Settings > Core plugins > Templates on, template folder `templates`.
3. Open the same folder in Claude Code (desktop app or `claude` in a terminal).

## Use it
- `/research-place hialeah florida`: research a place and save sourced facts to `places/florida/hialeah.md`.
- `/ask-brain which Florida cities have hurricane risk and hospitals?`: answer from your notes, with citations and gaps.
- "Save this idea: ..." or "capture: ...": Claude writes it to `inbox/` or the right folder.
- "Process the inbox": files captures into the right notes.

Rules Claude follows are in `CLAUDE.md`: every fact has a source, nothing is invented, "None found" is recorded.

## Back it up
Commit and push after a work session:

```bash
git add -A && git commit -m "Notes update" && git push
```
