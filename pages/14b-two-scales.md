---
layout: statement
---

# Two Scales, One Pattern

<div class="mt-10 grid grid-cols-2 gap-12 max-w-2xl mx-auto text-left">

<div class="space-y-3 p-5 bg-gray-800/80 rounded-xl border border-amber-400/30">
  <div class="text-amber-400 font-semibold text-sm uppercase tracking-wider">Scale 1 — Scrappy</div>
  <div class="text-3xl font-bold">~2h</div>
  <div class="text-gray-300 text-sm">1 developer · new API · zero prior domain knowledge · live on Vercel</div>
</div>

<div class="space-y-3 p-5 bg-gray-800/80 rounded-xl border border-blue-400/30">
  <div class="text-blue-400 font-semibold text-sm uppercase tracking-wider">Scale 2 — Production</div>
  <div class="text-3xl font-bold">spec → ship</div>
  <div class="text-gray-300 text-sm">Adversarial verification · 3-doc QA · nothing merges without a preflight</div>
</div>

</div>

<div class="mt-10 text-center text-gray-400 text-lg">Same underlying pattern. Different stakes.</div>

---

# What This Maps To — Scale 1

<div class="mt-2 text-gray-300 text-sm mb-4">The scrappy build. Claude Code + gstack, zero prior domain knowledge, ~2 hours.</div>

<div class="space-y-3 text-sm">

<div class="flex items-start gap-4 p-3 bg-gray-800/80 rounded-lg">
  <div class="text-amber-400 font-mono w-44 shrink-0">/office-hours</div>
  <div class="text-gray-300 flex-1">Validates approach, surfaces API questions, pushes back before code is written</div>
  <div class="text-amber-400 font-semibold text-xs w-36 shrink-0 text-right">Reactive Intelligence</div>
</div>

<div class="flex items-start gap-4 p-3 bg-gray-800/80 rounded-lg">
  <div class="text-blue-400 font-mono w-44 shrink-0">/plan-eng-review</div>
  <div class="text-gray-300 flex-1">Architecture feedback, 13 critical gaps surfaced before merge</div>
  <div class="text-blue-400 font-semibold text-xs w-36 shrink-0 text-right">Insight & Governance</div>
</div>

<div class="flex items-start gap-4 p-3 bg-gray-800/80 rounded-lg">
  <div class="text-purple-400 font-mono w-44 shrink-0">/plan-design-review</div>
  <div class="text-gray-300 flex-1">7 passes · 4/10 → 8.5/10 · full color palette written</div>
  <div class="text-purple-400 font-semibold text-xs w-36 shrink-0 text-right">Continuous Improvement</div>
</div>

<div class="flex items-start gap-4 p-3 bg-gray-800/80 rounded-lg">
  <div class="text-green-400 font-mono w-44 shrink-0">/ship</div>
  <div class="text-gray-300 flex-1">PR → Vercel → live in 34 seconds — the whole loop automated</div>
  <div class="text-green-400 font-semibold text-xs w-36 shrink-0 text-right">Orchestration</div>
</div>

<div class="flex items-start gap-4 p-3 bg-gray-800/80 rounded-lg">
  <div class="text-gray-300 font-mono w-44 shrink-0">Human pivot</div>
  <div class="text-gray-300 flex-1">"The map IS the point" — user context the AI didn't have. Engineer decides.</div>
  <div class="text-gray-400 font-semibold text-xs w-36 shrink-0 text-right">The irreducible human</div>
</div>

</div>

<div class="mt-4 text-center text-amber-400 text-sm font-semibold">The practitioner proves the platform vision.</div>

---

# What This Maps To — Scale 2

<div class="mt-2 text-gray-300 text-sm mb-4">The production pipeline. Same 5 patterns, enterprise stakes.</div>

<div class="space-y-3 text-sm">

<div class="flex items-start gap-4 p-3 bg-gray-800/80 rounded-lg">
  <div class="text-amber-400 font-mono w-44 shrink-0">/drew-product</div>
  <div class="text-gray-300 flex-1">GH Issue → 3 grounding Qs → code-fact-extractor → spec with ## Sources + ## Model Router</div>
  <div class="text-blue-400 font-semibold text-xs w-36 shrink-0 text-right">Insight & Governance</div>
</div>

<div class="flex items-start gap-4 p-3 bg-gray-800/80 rounded-lg border border-red-400/20">
  <div class="text-red-400 font-mono w-44 shrink-0">/drew-eng</div>
  <div class="text-gray-300 flex-1">Every claim verified adversarially — CONFIRM / OVERRIDE (w/ reasoning) / BLOCK gate</div>
  <div class="text-red-400 font-semibold text-xs w-36 shrink-0 text-right">Insight & Governance</div>
</div>

<div class="flex items-start gap-4 p-3 bg-gray-800/80 rounded-lg">
  <div class="text-amber-400 font-mono w-44 shrink-0">/review</div>
  <div class="text-gray-300 flex-1">Code reviewer reacts to every change; security auditor fires automatically on auth</div>
  <div class="text-amber-400 font-semibold text-xs w-36 shrink-0 text-right">Reactive Intelligence</div>
</div>

<div class="flex items-start gap-4 p-3 bg-gray-800/80 rounded-lg">
  <div class="text-green-400 font-mono w-44 shrink-0">/ship</div>
  <div class="text-gray-300 flex-1">PR → Vercel preview → production promote — deployment manifest generated</div>
  <div class="text-green-400 font-semibold text-xs w-36 shrink-0 text-right">Orchestration</div>
</div>

<div class="flex items-start gap-4 p-3 bg-gray-800/80 rounded-lg">
  <div class="text-purple-400 font-mono w-44 shrink-0">spec-guardrail hook</div>
  <div class="text-gray-300 flex-1">Blocks any spec write missing ## Sources (path:line + commit) or unfilled ## Model Router</div>
  <div class="text-purple-400 font-semibold text-xs w-36 shrink-0 text-right">Continuous Improvement</div>
</div>

</div>

<div class="mt-4 text-center text-amber-400 text-sm font-semibold">Two scales. Same pattern. The practitioner proves both.</div>
