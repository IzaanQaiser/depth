# Depth — Build Plan (living checklist; Codex updates checkboxes)

## Phase 1 — Spine (Thu, buffer Fri AM)
- [ ] Repo scaffold: Next.js + Prisma + Postgres/pgvector via docker-compose
- [ ] Ingestion: clone repo from URL, enumerate source files w/ ignores
- [ ] tree-sitter parsing (ts/tsx/js/py) → symbols with line ranges
- [ ] Graph builder: edges (calls/imports/contains), centrality ranking
- [ ] Embedding + pgvector storage per symbol chunk
- [ ] Retrieval: query → relevant symbols w/ file:line (vector + graph expansion)
- [ ] CLI gate: ingest Demo Repo A, print call graph, answer a "where does X
      happen" query with correct file:line
GATE: all above verified by human on Demo Repo A before Phase 2.

## Phase 2 — Interview Engine (Fri PM–Sat)
- [ ] Session state machine (covered topics, difficulty, mode)
- [ ] Grounded question generation citing real file:line
- [ ] Evaluator as separate pass; verdict taxonomy incl. fluent-but-wrong
- [ ] Adaptive strategy: advance / drill / teach (learn mode)
- [ ] Terminal interview gate on Demo Repo A
GATE: all 4 scripted bluffs caught with line-level corrections.

## Phase 3 — Knowledge Model + Report (Sun)
- [ ] Knowledge table + confidence updates from verdicts + decay
- [ ] Depth Score computation
- [ ] Heatmap data generation
- [ ] Report page + share token
GATE: two sessions → visibly evolved heatmap; report screenshot self-explanatory.

## Phase 4 — UI + Understand (Mon)
- [ ] Six screens per DESIGN.md
- [ ] Mermaid architecture/data-flow rendering from graph
- [ ] Assessment link create/take/deliver flow
GATE: full loop in browser on Repo A AND Repo B, zero broken demo-path states.

## Phase 5 — Ship (Mon night–Tue)
- [ ] 5+ demo rehearsals; record segments w/ fallbacks
- [ ] Video per skeleton (bluff catch lands by 1:45; close names Codex + GPT-5.6)
- [ ] README as pitch incl. "How we built it with Codex" from DEVLOG
- [ ] Fresh-clone test of setup instructions
- [ ] /feedback session ID captured
- [ ] Devpost form complete; SUBMIT EARLY AFTERNOON TUESDAY