---
layout: two-cols
---

# /drew-eng — The Adversarial Lane

<div class="mt-4 space-y-3 text-sm">

<div class="p-3 bg-gray-800/80 rounded-lg border-l-4 border-amber-400">
  <div class="font-semibold text-amber-400 mb-1">Step 1 — Extract every claim</div>
  <div class="text-gray-300 text-xs">Function names, types, file paths, field names, constants, CSS tokens — tagged <span class="text-blue-400">[EXISTING]</span> or <span class="text-green-400">[NEW]</span></div>
</div>

<div class="p-3 bg-gray-800/80 rounded-lg border-l-4 border-blue-400">
  <div class="font-semibold text-blue-400 mb-1">Step 2 — code-fact-extractor on every [EXISTING] claim</div>
  <div class="text-gray-300 text-xs">FOUND_MATCH → silent VERIFIED. FOUND_CONFLICT or NOT_FOUND → surfaces to engineer.</div>
</div>

<div class="p-3 bg-gray-800/80 rounded-lg border-l-4 border-red-400">
  <div class="font-semibold text-red-400 mb-1">Step 3 — Interactive challenge loop</div>
  <div class="font-mono text-xs text-gray-400 mt-1 space-y-0.5">
    <div><span class="text-green-400">A) CONFIRM</span> — extractor is misleading, claim is correct</div>
    <div><span class="text-amber-400">B) OVERRIDE</span> — discrepancy noted; reasoning + risk required</div>
    <div><span class="text-red-400">C) BLOCK</span> — claim is wrong; spec must be corrected</div>
  </div>
</div>

<div class="p-3 bg-gray-800/80 rounded-lg border-l-4 border-green-400">
  <div class="font-semibold text-green-400 mb-1">Gate: BLOCKED_COUNT = 0 → /implement</div>
  <div class="text-gray-300 text-xs">Any unresolved BLOCK stops the pipeline. Override requires written reasoning + risk level.</div>
</div>

</div>

::right::

<div class="ml-6 mt-4 space-y-4 text-sm">

<div class="p-4 bg-gray-800/80 rounded-lg border border-gray-700">
  <div class="font-semibold text-gray-300 mb-2 text-xs uppercase tracking-wider">The Credible Hulk Principle</div>
  <div class="text-gray-300 text-sm italic">"AI does all the verification legwork. The engineer carries the receipts and makes every override call."</div>
  <div class="text-gray-500 text-xs mt-2">No claim reaches the codebase without a human sign-off.</div>
</div>

<div class="p-3 bg-gray-800/80 rounded-lg border border-gray-700 font-mono text-xs text-gray-400 space-y-1">
  <div class="text-gray-300 font-semibold not-italic mb-1">Hot-spot briefing — post-gate</div>
  <div><span class="text-red-400">HIGH RISK</span></div>
  <div class="pl-2 text-gray-500">useMartaData() — extractor found</div>
  <div class="pl-2 text-gray-500">signature differs. Override: "hook</div>
  <div class="pl-2 text-gray-500">confirmed by team lead."</div>
  <div class="mt-1 text-gray-500 text-xs">Citations saved to task-progress/*.jsonl</div>
</div>

<div class="mt-2 p-3 bg-red-400/10 rounded-lg border border-red-400/30 text-xs text-gray-300">
  Adversarial verification — applied at the spec layer, against every claim, before a single line is written.
</div>

</div>
