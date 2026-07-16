# Portugal Buyer-Side Knowledge Base — Usage Instructions

An LLM-maintained Obsidian wiki (Karpathy "LLM wiki" pattern) for a venture monetizing the buyer's side of the Portuguese real estate market through two platforms (buyer's agency and home inspection). You curate sources and ask questions; the LLM writes and maintains everything.

## Setup (5 minutes)

1. **Unzip** this folder anywhere (ideally inside a git repo: `git init` for free version history).
2. **Open as an Obsidian vault:** Obsidian → Open folder as vault → select `pt-buyers-kb`. Start at `Home.md`. Use graph view to see the shape.
3. **Connect your LLM agent** (Claude Code, Codex, etc.) with the vault folder as its working directory. `CLAUDE.md` is the schema — Claude Code reads it automatically; for other agents, point them at it explicitly ("Read CLAUDE.md and follow it").
4. Recommended Obsidian settings: Files & links → attachment folder = `raw/assets/`. Optional plugins: Dataview (frontmatter queries), Obsidian Web Clipper (browser → markdown sources).

## Daily workflows

**Add a source:** drop the file into `raw/`, then tell the agent: *"Ingest raw/<filename> per CLAUDE.md."* It will summarize, discuss takeaways, update every touched page, update index.md, and append to log.md. Ingest one at a time and stay involved — read the summary, correct emphasis.

**Ask a question:** just ask. The agent reads Home/index, drills into pages, answers with links. If the answer is valuable, tell it to file the answer in `06-syntheses/` — that's how explorations compound.

**Monthly health check:** *"Run a lint pass per CLAUDE.md."* Finds contradictions, orphans, stale claims, stubs, and suggests next sources.

## Rules that keep the system healthy

- **One concept per page (atomicity).** If a page starts covering two things, the agent splits it. Don't fight this by pasting long dumps into single notes — drop dumps into `07-inbox/` or `raw/` and let the agent file them.
- **`07-inbox/` is temporary parking**, not storage — monthly lint empties it.
- **Never edit `raw/`** — it's the immutable source of truth. The LLM writes everything else; you rarely edit wiki pages by hand.
- **The buyer journey is the root taxonomy.** Platforms are views, not folders of duplicated knowledge. If you're tempted to reorganize around one platform, read `06-syntheses/inspection-in-the-buyer-journey.md` first.
- **Symptom-first for defects, numbers are sacred, every page links to a hub** — full conventions in `CLAUDE.md`.

## Immediate next steps (highest-leverage)

1. **Run and ingest the missing prompt-chain modules** (1–6, 9, 11–12) — the biggest expansion of the inspection engine. Drop each output into `raw/` and ingest.
2. **Ingest playbook Ch. 10 property types and Appendices B/C** into dedicated pages (already flagged in the source page).
3. Decide agency fee model and launch region — open questions logged on the strategy pages.
