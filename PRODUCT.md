# Depth

**Agents write the code. Depth makes sure you understand it.**

## Thesis
In the agentic era, producing code is no longer the bottleneck — understanding it is.
Developers ship thousands of agent-written lines they've never truly read. Depth is the
first tool that verifies and builds a human's comprehension of their own codebase:
it interviews you about your code, catches you bluffing with line-level evidence,
teaches you where you're weak, and tracks your understanding over time.

## Persona (primary)
The vibecoder: built a real project fast with AI agents, now needs to genuinely own it —
for a grade, an interview, a job, or their own growth. Secondary personas (same engine):
students assessed by educators, juniors onboarding to codebases, devs returning to old projects.

## The Loop
1. **Understand** — ingest a repo; generate architecture map, sequence diagrams,
   "the files that matter," from a parsed structural graph (not model vibes).
2. **Ask** — chat grounded in the repo; every answer cites file:line.
3. **Practice** — low-stakes adaptive quizzing on YOUR code; teaches on misses.
4. **Prove** — Assess Mode: timed, no-hints interview producing a shareable
   **Depth Report** (score + per-file/concept heatmap + blind-trust zones).
   Educator flow: instructor sends an assessment link, receives the report.

## The Knowledge Model
Every interaction updates a persistent, per-repo, per-user map of demonstrated
understanding: concept-by-concept, confidence-weighted, decaying over time.
This powers the heatmap, progress tracking, weakness analysis, and "study next"
recommendations. This state is what makes Depth a product, not a prompt.

## Hackathon Framing
Track: Education. The educator assessment-link flow is the track story;
the self-serve loop is the daily-use product; Review Mode (interview on a diff)
is demonstrated as vision in the video.

## OUT OF SCOPE — DO NOT BUILD
- No code fixing, refactoring suggestions, or auto-generated issues (Depth fixes the
  human, not the code)
- No team dashboards, orgs, or GitHub App/CI integration
- No voice mode
- No languages beyond TypeScript/JavaScript and Python (parse targets)
- No auth beyond minimal (single-user + magic assessment links)
- Nothing not listed in PLAN.md