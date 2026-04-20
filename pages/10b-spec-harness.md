---
layout: center
background: '#0d1117'
---

# The Spec-Driven Harness

<div class="text-sm text-gray-400 mt-1 mb-5">Every step creates or updates a GitHub artifact.</div>

<div class="space-y-3 text-sm max-w-2xl mx-auto">

<div class="flex items-start gap-4 p-3 bg-gray-800/80 rounded-lg border-l-4 border-amber-400">
  <div class="font-mono text-amber-400 w-36 shrink-0">/drew-product</div>
  <div>
    <div class="text-gray-200">Creates GitHub Issue · asks 3 grounding questions</div>
    <div class="text-gray-500 text-xs mt-1">extracts + verifies every identifier in the codebase · writes spec with confirmed sources</div>
  </div>
</div>

<div class="flex items-start gap-4 p-3 bg-gray-800/80 rounded-lg border-l-4 border-blue-400">
  <div class="font-mono text-blue-400 w-36 shrink-0">approve</div>
  <div>
    <div class="text-gray-200">Human reviews the spec · pushes back if needed</div>
    <div class="text-gray-500 text-xs mt-1">nothing ships without sign-off — the guardrail is a git hook</div>
  </div>
</div>

<div class="flex items-start gap-4 p-3 bg-gray-800/80 rounded-lg border-l-4 border-orange-400">
  <div class="font-mono text-orange-400 w-36 shrink-0">/drew-eng</div>
  <div>
    <div class="text-gray-200">Adversarial verification → then builds</div>
    <div class="text-gray-500 text-xs mt-1">challenges every claim · catches hallucinated identifiers · comments on the GH issue</div>
  </div>
</div>

<div class="flex items-start gap-4 p-3 bg-gray-800/80 rounded-lg border-l-4 border-green-400">
  <div class="font-mono text-green-400 w-36 shrink-0">/ship</div>
  <div>
    <div class="text-gray-200">GitHub PR opened · Vercel deploys · done</div>
    <div class="text-gray-500 text-xs mt-1">issue linked · reviewers assigned · the whole trail is in GitHub</div>
  </div>
</div>

</div>

<div class="mt-5 text-center text-gray-500 text-xs">
  Issue → Spec → Verify → Build → PR — <span class="text-amber-400">every artifact lives in GitHub</span>
</div>
