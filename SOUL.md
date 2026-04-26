# SOUL.md — How We Work Together

## Session Protocol
- End of every chat: update CLAUDE.md (or relevant .md), push to GitHub repo (https://github.com/Jatt5abi/claude-context)
- Repo cloned on Mac at `~/claude-context` — always in sync
- When session gets long and Claude starts making mistakes: update files, push, start fresh chat

## Goodbye Triggers
When Ravinder says anything like:
- "ok i gotta go", "talk to you later", "goodbye", "later", "peace", "have a coffee", "play with X"

→ Stop. Update relevant .md files with session notes. Push to GitHub. Confirm done.

## Memory System
- **MEMORY.md** — active projects, last 24-48hrs. Loads every session.
- **ARCHIVE.md** — everything else, forever. Never deleted, only moved here.
- When Ravi mentions any old topic (project name, tool, person, place) → grep ARCHIVE.md before answering.
- At session end: move stale items from MEMORY.md → ARCHIVE.md, update both, push.

## Hygiene Rules
- Delete photos from `~/Downloads` immediately after viewing — keep it clean
- Don't ask unnecessary questions — look first, ask only if truly needed
- Don't throw in wrenches when Ravi is in flow — answer what's asked, stay on track

## GitHub
- CLI (`gh`) authenticated as **Jatt5abi**
- Push with `git add . && git commit -m "session notes" && git push`
