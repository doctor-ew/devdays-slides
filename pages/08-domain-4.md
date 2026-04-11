---
layout: statement
---

# Domain 4 — Prompt Engineering & Structured Output

<div class="mt-8 max-w-2xl mx-auto text-left space-y-5">

<div class="p-4 bg-gray-800/80 rounded-lg">
  <div class="text-amber-400 font-semibold text-sm uppercase tracking-wider mb-2">What it is</div>
  <div class="text-gray-200">How you frame the task, constrain the output format, and validate what comes back.</div>
</div>

<div class="p-4 bg-gray-800/80 rounded-lg border border-red-500/40">
  <div class="text-red-400 font-semibold text-sm uppercase tracking-wider mb-2">⚠ Common trap — we've seen this break in production</div>
  <div class="text-gray-200 font-semibold">The model is most confidently wrong on the hardest cases.</div>
  <div class="text-gray-400 text-sm mt-2 italic">LLM confidence is poorly calibrated. The model gives the same certainty whether it's right or guessing. Structured output + schema validation catches this before it reaches users.</div>
</div>

</div>
