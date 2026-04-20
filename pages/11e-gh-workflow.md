---
layout: center
background: '#0d1117'
---

# Issue → Spec → Verify → Ship

<div class="mt-4 max-w-2xl mx-auto font-mono text-xs space-y-2">

<div class="p-3 bg-gray-900 rounded-lg border border-gray-700">
  <div class="text-green-400 mb-1"># 1. Create the GitHub Issue</div>
  <div class="text-gray-300">gh issue create --title <span class="text-amber-400">"feat: Add MARTA Status Card"</span> \</div>
  <div class="text-gray-300 pl-4">--body <span class="text-amber-400">"Real-time sidebar showing bus/train status per zone"</span> \</div>
  <div class="text-gray-300 pl-4">--label <span class="text-amber-400">"enhancement"</span></div>
  <div class="text-gray-500 mt-1">→ Issue <span class="text-amber-400">#2</span> created · Copilot Chat asks 3 grounding questions inline</div>
</div>

<div class="p-3 bg-gray-900 rounded-lg border border-gray-700">
  <div class="text-red-400 mb-1"># 2. Adversarial verification</div>
  <div class="text-gray-300">/drew-eng GH-2</div>
  <div class="text-gray-500 mt-1">→ Copilot Code Review verifies every spec claim · <span class="text-green-400">CONFIRM</span> / <span class="text-amber-400">OVERRIDE</span> / <span class="text-red-400">BLOCK</span></div>
  <div class="text-gray-500">→ gh issue comment #2 <span class="text-amber-400">"Verification complete — 0 BLOCKs"</span></div>
</div>

<div class="p-3 bg-gray-900 rounded-lg border border-gray-700">
  <div class="text-blue-400 mb-1"># 3. Build + open the PR</div>
  <div class="text-gray-300">/implement GH-2  <span class="text-gray-600"># Copilot Coding Agent builds against spec</span></div>
  <div class="text-gray-300">bun test  <span class="text-gray-600">→ green</span></div>
  <div class="text-gray-300">gh pr create --title <span class="text-amber-400">"feat: MartaStatusCard"</span> --body <span class="text-amber-400">"Closes #2"</span></div>
  <div class="text-gray-500 mt-1">→ Vercel preview deployed · reviewers assigned</div>
</div>

<div class="p-3 bg-gray-900 rounded-lg border border-green-400/30">
  <div class="text-green-400 mb-1"># 4. Merge → Actions → Pages</div>
  <div class="text-gray-300">gh pr merge --squash  <span class="text-gray-600"># closes Issue #2</span></div>
  <div class="text-gray-500 mt-1">→ GitHub Actions: build · test · upload artifact</div>
  <div class="text-gray-500">→ GitHub Pages: <span class="text-amber-400">doctor-ew.github.io/marta-devdays/</span> · live in ~34s</div>
</div>

</div>

<div class="mt-3 text-center text-gray-500 text-xs">One issue. One spec. One PR. Every step a GitHub artifact — traceable, auditable, reproducible.</div>
