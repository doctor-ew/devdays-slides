---
layout: statement
---

# Domain 1 — Architecture & Orchestration

<div class="mt-8 max-w-2xl mx-auto text-left space-y-5">

<div class="p-4 bg-gray-800/80 rounded-lg">
  <div class="text-amber-400 font-semibold text-sm uppercase tracking-wider mb-2">What it is</div>
  <div class="text-gray-200">How subagents are structured, what they own, and how they hand off work.</div>
</div>

<div class="p-4 bg-gray-800/80 rounded-lg border border-red-500/40">
  <div class="text-red-400 font-semibold text-sm uppercase tracking-wider mb-2">⚠ Common trap — we've seen this break in production</div>
  <div class="text-gray-200 font-semibold">Context leakage between subagents creates compounding failures.</div>
  <div class="text-gray-400 text-sm mt-2 italic">Agent A passes a bloated context to Agent B. Agent B's output drifts. Agent C doesn't know which half is real. Each step amplifies the error.</div>
</div>

</div>
