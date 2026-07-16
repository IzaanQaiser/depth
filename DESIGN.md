# Depth — Design

## Aesthetic: "Calm Academic"
Off-white background (#FAF9F6-ish), single accent (deep ink blue), serif display
headers (e.g. Source Serif / Lora), sans body, generous whitespace, exam-paper
calm. No gradients, no glassmorphism, no dashboard slop. Feels like a well-typeset
examination — serious, quiet, confident. shadcn/ui components, restrained.

## Screens (6)
1. **Home / Repos** — list of ingested repos + "Add repo" (URL input). Each card:
   name, Depth Score, last session.
2. **Repo Overview (Understand)** — architecture map (Mermaid from graph),
   "files that matter" ranked list, data-flow diagrams, entry to all modes.
3. **Interview Session** — one question at a time, centered, cited code snippet
   inline (file:line visible), answer box, timer subtle in Assess Mode. Verdict
   appears as a calm inline correction, not a red buzzer.
4. **Knowledge Heatmap** — file/concept grid colored by confidence; hovering
   shows evidence (which exchanges). The screenshot-hero screen.
5. **Depth Report** — shareable page: score, heatmap, blind-trust zones,
   session deltas ("3 days ago you couldn't explain X").
6. **Assessment Link Flow** — create link (educator) / take assessment (student);
   completion routes report to creator.

## Tone in copy
Interviewer voice: precise, warm, unimpressed by fluency. Corrections cite lines.
Never mocking. "Not quite — look at line 47" not "Wrong!"