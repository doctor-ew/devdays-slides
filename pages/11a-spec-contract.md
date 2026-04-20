---
layout: statement
---

# The Spec Is the Contract

<div class="mt-10 grid grid-cols-2 gap-12 max-w-2xl mx-auto text-left">

<div class="space-y-3">
  <div class="text-amber-400 font-semibold text-sm uppercase tracking-wider">The problem</div>
  <div class="text-lg">AI makes building fast. It doesn't make building the <em>right thing</em> easier.</div>
  <div class="text-gray-300 text-sm">Without a spec, the engineer and the AI are both guessing about intent.</div>
</div>

<div class="space-y-3">
  <div class="text-amber-400 font-semibold text-sm uppercase tracking-wider">The rule</div>
  <div class="text-lg font-semibold">No code without a spec.</div>
  <div class="text-gray-300 text-sm">The spec is not a planning doc. It's the contract between the ticket and the implementation.</div>
</div>

</div>

<div class="mt-12 text-center text-gray-400 italic text-lg max-w-xl mx-auto">
  "If you can't write it down, you're not ready to build it."
</div>

---
layout: center
---

# The Pipeline — Handoff Gates

<div class="mt-4 max-w-2xl mx-auto space-y-2 text-sm">

<div class="flex items-center gap-3 p-3 bg-gray-800/80 rounded-lg">
  <div class="font-mono text-amber-400 w-36 shrink-0">/drew-product</div>
  <div class="flex-1 text-gray-300">GH Issue → 3 grounding Qs → code-fact-extractor → spec with cited sources</div>
  <div class="text-amber-400 text-xs border border-amber-400/40 rounded px-2 py-0.5 shrink-0">ENGINEER APPROVES</div>
</div>

<div class="text-center text-gray-600">↓</div>

<div class="flex items-center gap-3 p-3 bg-gray-800/80 rounded-lg border border-red-400/20">
  <div class="font-mono text-red-400 w-36 shrink-0">/drew-eng</div>
  <div class="flex-1 text-gray-300">Extract all claims → adversarial verify each → CONFIRM / OVERRIDE / BLOCK</div>
  <div class="text-red-400 text-xs border border-red-400/40 rounded px-2 py-0.5 shrink-0">ALL CLAIMS RESOLVED</div>
</div>

<div class="text-center text-gray-600">↓</div>

<div class="flex items-center gap-3 p-3 bg-gray-800/80 rounded-lg">
  <div class="font-mono text-blue-400 w-36 shrink-0">/implement</div>
  <div class="flex-1 text-gray-300">Engineer or Architect agent — builds against spec + citation file</div>
  <div class="text-green-400 text-xs border border-green-400/40 rounded px-2 py-0.5 shrink-0">TESTS GREEN</div>
</div>

<div class="text-center text-gray-600">↓</div>

<div class="flex items-center gap-3 p-3 bg-gray-800/80 rounded-lg">
  <div class="font-mono text-purple-400 w-36 shrink-0">/review-spec</div>
  <div class="flex-1 text-gray-300">QA agent — 3-doc check: issue ↔ spec ↔ code. Flags drift before PR opens.</div>
  <div class="text-purple-400 text-xs border border-purple-400/40 rounded px-2 py-0.5 shrink-0">ALIGNED</div>
</div>

<div class="text-center text-gray-600">↓</div>

<div class="flex items-center gap-3 p-3 bg-gray-800/80 rounded-lg">
  <div class="font-mono text-green-400 w-36 shrink-0">/ship</div>
  <div class="flex-1 text-gray-300">PR → Vercel preview → production promote — deployment manifest generated</div>
  <div class="text-green-400 text-xs border border-green-400/40 rounded px-2 py-0.5 shrink-0">DEPLOY SAFE</div>
</div>

</div>

<div class="mt-4 text-center text-gray-500 text-xs">Agents propose. Engineers decide. Every gate is a human handoff.</div>
