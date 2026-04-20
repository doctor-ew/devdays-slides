---
layout: center
---

# Model Tiering — Cost Discipline at Scale

<div class="mt-6 max-w-2xl mx-auto">

<div class="grid grid-cols-3 gap-4 text-sm text-center">

<div class="p-4 bg-gray-800/80 rounded-xl border border-gray-600">
  <div class="text-gray-300 font-bold text-lg mb-1">Haiku</div>
  <div class="text-gray-500 text-xs mb-3">Mechanical work</div>
  <div class="space-y-1 text-left text-xs text-gray-400">
    <div>• run-all-tests</div>
    <div>• docs-updater</div>
    <div>• CLAUDE.md sync</div>
  </div>
</div>

<div class="p-4 bg-gray-800/80 rounded-xl border border-amber-400/40">
  <div class="text-amber-300 font-bold text-lg mb-1">Sonnet</div>
  <div class="text-gray-500 text-xs mb-3">Analysis · Default</div>
  <div class="space-y-1 text-left text-xs text-gray-400">
    <div>• spec-writer</div>
    <div>• engineer</div>
    <div>• qa · code-reviewer</div>
    <div>• security-auditor</div>
  </div>
</div>

<div class="p-4 bg-gray-800/80 rounded-xl border border-purple-400/40">
  <div class="text-purple-300 font-bold text-lg mb-1">Opus</div>
  <div class="text-gray-500 text-xs mb-3">Architecture · Complex</div>
  <div class="space-y-1 text-left text-xs text-gray-400">
    <div>• architect</div>
    <div>• 3+ files changed</div>
    <div>• cross-team impact</div>
    <div>• after 2 failed fixes</div>
  </div>
</div>

</div>

<div class="mt-5 p-3 bg-gray-800/80 rounded-lg text-sm text-center text-gray-300">
  <code class="text-amber-400">/drew-product</code> injects a <strong>## Model Router</strong> section into every spec — the decision is written down, not improvised at build time.
</div>

<div class="mt-2 text-center text-gray-500 text-xs">spec-guardrail hook blocks any spec write without a filled Model Router decision.</div>

</div>
