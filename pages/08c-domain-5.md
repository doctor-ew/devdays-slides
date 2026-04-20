---
layout: statement
---

# Domain 5 — Context Management & Reliability

<div class="mt-8 max-w-2xl mx-auto text-left space-y-5">

<div class="p-4 bg-gray-800/80 rounded-lg">
  <div class="text-amber-400 font-semibold text-sm uppercase tracking-wider mb-2">What it is</div>
  <div class="text-gray-200">Preserving critical information across long interactions. Designing escalation patterns that fire at the right threshold. Managing error propagation in multi-agent systems so failures don't cascade silently. Handling uncertainty with confidence calibration.</div>
  <div class="text-gray-400 text-sm mt-2 italic">This domain is about what happens when things go wrong — which in production, they always eventually do.</div>
</div>

<div class="p-4 bg-gray-800/80 rounded-lg border border-red-500/40">
  <div class="text-red-400 font-semibold text-sm uppercase tracking-wider mb-2">⚠ Common trap — we've seen this break in production</div>
  <div class="text-gray-200 font-semibold">Routing all workflows to the Batch API for cost savings — Batch has no SLA.</div>
  <div class="text-gray-400 text-sm mt-2 italic">Blocking workflows require the real-time API regardless of cost preferences. Cost optimization is valid; using it on latency-sensitive paths is not.</div>
</div>

</div>
