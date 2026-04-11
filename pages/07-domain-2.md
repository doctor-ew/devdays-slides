---
layout: statement
---

# Domain 2 — Tool Design & MCP Integration

<div class="mt-8 max-w-2xl mx-auto text-left space-y-5">

<div class="p-4 bg-gray-800/80 rounded-lg">
  <div class="text-amber-400 font-semibold text-sm uppercase tracking-wider mb-2">What it is</div>
  <div class="text-gray-200">What tools you give agents, how they're scoped, and how agents select them.</div>
</div>

<div class="p-4 bg-gray-800/80 rounded-lg border border-red-500/40">
  <div class="text-red-400 font-semibold text-sm uppercase tracking-wider mb-2">⚠ Common trap — we've seen this break in production</div>
  <div class="text-gray-200 font-semibold">Giving 18 tools to an agent that needs 4 reliably degrades its tool selection quality.</div>
  <div class="text-gray-400 text-sm mt-2 italic">More tools = more surface area for the model to get confused. The agent starts using the wrong tool with confidence. Curate ruthlessly.</div>
</div>

</div>
