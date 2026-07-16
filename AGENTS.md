<!-- BEGIN:nextjs-agent-rules -->
# This is NOT the Next.js you know

This version has breaking changes — APIs, conventions, and file structure may all differ from your training data. Read the relevant guide in `node_modules/next/dist/docs/` before writing any code. Heed deprecation notices.
<!-- END:nextjs-agent-rules -->

# Depth Agent Instructions

## Before any task
Read PRODUCT.md, ARCHITECTURE.md, DESIGN.md, PLAN.md. PRODUCT.md's
"OUT OF SCOPE" list is absolute. Never build anything not in PLAN.md.

## Workflow
- For each task: propose your approach FIRST, wait for approval, then implement.
- If a task is ambiguous, ask — do not resolve ambiguity by inventing scope.
- Run typecheck and tests before declaring any task complete.
- Update PLAN.md checkboxes when items are verified.
- Append 2 lines to DEVLOG.md at the end of each work session:
  what was built, what decisions were made.

## Conventions
- TypeScript strict. Next.js App Router. Prisma for all DB access.
- Commit after each completed task; imperative, descriptive messages.
- Dev: docker compose up -d (Postgres+pgvector); npm run dev; npm test.
- Secrets in .env (never committed). OPENAI_API_KEY required.

## Quality bars
- Evaluator must distinguish fluent-but-wrong from correct, with line-level evidence.
- All generated questions/corrections must cite real file:line from the graph.
- The demo path (ingest → interview → bluff catch → heatmap → report) takes
  precedence over any other work when time is constrained.
