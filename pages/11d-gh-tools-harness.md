---
layout: center
---

# The Harness — What GitHub Is Doing

<div class="mt-4 max-w-2xl mx-auto space-y-2 text-sm">

<div class="flex items-start gap-3 p-3 bg-gray-800/80 rounded-lg">
  <div class="font-mono text-amber-400 w-36 shrink-0">/drew-product</div>
  <div class="flex-1 text-gray-300">
    <div class="space-y-0.5">
      <div><span class="text-gray-500 font-mono text-xs">gh issue create</span> — creates the ticket, assigns it</div>
      <div><span class="text-gray-500 font-mono text-xs">Copilot Chat</span> — answers 3 grounding questions inline</div>
      <div><span class="text-gray-500 font-mono text-xs">gh issue comment</span> — posts the spec link when done</div>
    </div>
  </div>
  <div class="text-amber-400 text-xs border border-amber-400/40 rounded px-2 py-0.5 shrink-0 self-start">SPEC WRITTEN</div>
</div>

<div class="text-center text-gray-600 text-xs">↓ engineer reviews · approves or pushes back</div>

<div class="flex items-start gap-3 p-3 bg-gray-800/80 rounded-lg border border-red-400/20">
  <div class="font-mono text-red-400 w-36 shrink-0">/drew-eng</div>
  <div class="flex-1 text-gray-300">
    <div class="space-y-0.5">
      <div><span class="text-gray-500 font-mono text-xs">Copilot Code Review</span> — adversarially verifies every claim against the codebase</div>
      <div><span class="text-gray-500 font-mono text-xs">gh issue comment</span> — logs CONFIRM / OVERRIDE / BLOCK verdicts</div>
    </div>
  </div>
  <div class="text-red-400 text-xs border border-red-400/40 rounded px-2 py-0.5 shrink-0 self-start">CLAIMS RESOLVED</div>
</div>

<div class="text-center text-gray-600 text-xs">↓ no BLOCKs outstanding</div>

<div class="flex items-start gap-3 p-3 bg-gray-800/80 rounded-lg">
  <div class="font-mono text-blue-400 w-36 shrink-0">/implement</div>
  <div class="flex-1 text-gray-300">
    <div class="space-y-0.5">
      <div><span class="text-gray-500 font-mono text-xs">Copilot Coding Agent</span> — builds against spec + citation file</div>
      <div><span class="text-gray-500 font-mono text-xs">gh pr create</span> — opens PR, links to the issue, assigns reviewers</div>
    </div>
  </div>
  <div class="text-green-400 text-xs border border-green-400/40 rounded px-2 py-0.5 shrink-0 self-start">PR OPEN</div>
</div>

<div class="text-center text-gray-600 text-xs">↓ CI green</div>

<div class="flex items-start gap-3 p-3 bg-gray-800/80 rounded-lg">
  <div class="font-mono text-green-400 w-36 shrink-0">/ship</div>
  <div class="flex-1 text-gray-300">
    <div class="space-y-0.5">
      <div><span class="text-gray-500 font-mono text-xs">gh pr merge</span> — merges, closes the issue</div>
      <div><span class="text-gray-500 font-mono text-xs">GitHub Actions</span> — runs build pipeline, deploys artifact</div>
      <div><span class="text-gray-500 font-mono text-xs">GitHub Pages</span> — live in seconds</div>
    </div>
  </div>
  <div class="text-green-400 text-xs border border-green-400/40 rounded px-2 py-0.5 shrink-0 self-start">LIVE</div>
</div>

</div>

<div class="mt-4 text-center text-gray-500 text-xs">Every artifact — issue · spec · claims log · PR · deploy — lives in GitHub. The trail is the audit.</div>
