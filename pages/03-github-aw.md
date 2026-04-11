---
layout: two-cols
---

# What GitHub Agentic Workflows Is

<div class="mt-4 space-y-4 text-sm">

<div class="p-4 bg-gray-800/80 rounded-lg border-l-4 border-amber-400">
  <div class="font-semibold text-amber-400 mb-2">Write it in Markdown</div>
  <div class="text-gray-300">Plain <code>.md</code> files with frontmatter. Triggers, AI engine, permissions, tools, env.</div>
</div>

<div class="p-4 bg-gray-800/80 rounded-lg border-l-4 border-blue-400">
  <div class="font-semibold text-blue-400 mb-2">Compile to a lockfile</div>
  <div class="font-mono text-xs text-gray-300 mt-1">gh extension install github/gh-aw<br>gh aw compile</div>
</div>

<div class="p-4 bg-gray-800/80 rounded-lg border-l-4 border-green-400">
  <div class="font-semibold text-green-400 mb-2">Run in isolation</div>
  <div class="text-gray-300">Read-only permissions. Agent proposes actions. Threat detection scans output before execution.</div>
</div>

</div>

::right::

<div class="ml-6 mt-4">

```markdown
---
on: issues
  types: [labeled]
model: gpt-4o
permissions:
  issues: write
  pull-requests: write
tools:
  - github
---

When an issue is labeled "needs-repro",
investigate and open a draft PR with
a minimal reproduction case.
```

<div class="mt-4 text-xs text-gray-400 italic">*.md → gh aw compile → *.lock.yml → runs in CI</div>

</div>
