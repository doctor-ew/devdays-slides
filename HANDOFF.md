# DevDays Handoff — Fresh Claude Instance

**Date:** 2026-04-19  
**Context:** Drew is prepping two back-to-back conference talks today.  
Talk 1 (Atlanta AI Week) is done. This handoff is for **Talk 2: GitHub Dev Days.**

---

## The Talk

**"From Prompt to Production: Agentic Workflows in Practice"**  
**Event:** Microsoft / GitHub Dev Days 2026  
**Repo:** `github.com/doctor-ew/devdays-slides`  
**Local:** `/Users/drew.schillinger/shuttlebay/DoctorEws_Laboratory/_Workshops_/DevDays`  
**Framework:** Slidev 52.x — Markdown slides, Vue 3, theme: seriph

The demo app for the talk is at:  
**Repo:** `github.com/doctor-ew/marta-devdays`  
**Local:** `/Users/drew.schillinger/shuttlebay/DoctorEws_Laboratory/_Workshops_/marta-devdays`  
**Stack:** Next.js 16, Tailwind 4, Claude AI, MARTA transit APIs, Vercel

---

## The Workflow Drew Is Demoing Live

Drew built spec-driven harnesses he calls **`/drew-product`** and **`/drew-eng`**. These are Claude Code slash commands.

| Command | What it does |
|---------|-------------|
| `/drew-product` | Creates a GitHub Issue, asks 3 grounding questions, extracts + verifies code identifiers, writes a spec with verified sources + Model Router decision |
| `/drew-eng` | Adversarial claim verification on the spec, then calls `/implement` internally |
| `/ship` | PR created, Vercel deployed, done |

**The "GH under the hood" angle (this is the DevDays-specific hook):**
- `/drew-product` creates a real GitHub Issue with the spec linked
- `/drew-eng` leaves a comment on the issue with verification results
- `/ship` opens a GitHub PR and Vercel auto-deploys

These are the same commands as `/drprod` and `/dreng` — Drew renamed them for his personal branding. The command files live at:
- `.claude/commands/drprod.md` → surfaced as `/drew-product`
- `.claude/commands/dreng.md` → surfaced as `/drew-eng`

---

## What Was Done in the Previous Session (Atlanta AI Week)

### Built and working:
- `github.com/doctor-ew/atlaiweek-fifa` — the main FIFA Navigator app (v2, gstack-built)
  - Branch `feat/spec-driven-v3` = same app rebuilt via `/drew-product` + `/drew-eng`
  - PR #3 is open for comparison
- `github.com/doctor-ew/atlaiweek-fifa-v3` — the v3 spec-driven standalone repo
- Slides at `/Users/drew.schillinger/shuttlebay/DoctorEws_Laboratory/_Workshops_/AtlantaAIWeek` are updated

### Key spec generated during Atlanta AI Week session:
- `atlaiweek-fifa` → `docs/GH-2/SPEC.md` — MartaStatusCard component spec
- GitHub Issue #2 on `atlaiweek-fifa` is the live demo issue for the Atlanta talk

---

## What Needs to Be Done for DevDays

### 1. GitHub Pages for Slides
The DevDays slides need a GitHub Pages deployment. The build is already configured:
```
bun run build  →  slidev build slides.md --base /slides/
```
Output goes to `dist/`. Need: `.github/workflows/deploy-slides.yml`  
Target: `github.com/doctor-ew/devdays-slides` → GitHub Pages at `/slides/`

### 2. Create a GitHub Issue (via `/drew-product`)
Drew needs to create a GitHub issue in the `marta-devdays` repo for the feature he'll build live on stage. This is the **live demo issue** — the thing he creates live in front of the audience using `/drew-product`.

Suggested feature: A **MARTA Status Card** component (same concept as the Atlanta talk, but simpler/different framing for the DevDays audience). Or a different small feature from the PRD.

**To create it:** `cd /Users/drew.schillinger/shuttlebay/DoctorEws_Laboratory/_Workshops_/marta-devdays` then run `/drew-product` pointing at the PRD.

### 3. Update the Slides
The DevDays slides (`pages/10-gstack-roles.md` and a new slide) need to show:
- `/drew-product` → creates GitHub Issue + grounding + spec (GitHub native)
- `/drew-eng` → adversarial verification + implement
- `/ship` → GitHub PR + Vercel deploy

The GH-native angle is the hook for this audience: **"Every step creates or updates a GitHub artifact."**

Slide to add: A new `pages/10b-spec-harness.md` after `10-gstack-roles.md` showing the two-phase workflow (gstack for design, spec harness for build).

Also: Update `pages/11-fafnir.md` to use the new Fafnir image:  
`/Users/drew.schillinger/.claude/image-cache/0c4e1052-5e6b-48af-8353-175dd6d6f1ae/1.png`  
(Copy to `public/img/fafnir-credible-hulk.png` and update the img src)

---

## Repos Quick Reference

| Repo | Purpose | Local |
|------|---------|-------|
| `doctor-ew/devdays-slides` | DevDays slides | `_Workshops_/DevDays` |
| `doctor-ew/marta-devdays` | Demo app for DevDays | `_Workshops_/marta-devdays` |
| `doctor-ew/atlaiweek-fifa` | Atlanta AI Week app (main) | `ATL-FIFA-Navigator/atl-fifa-navigator-v2` |
| `doctor-ew/atlaiweek-fifa-v3` | v3 spec-driven rebuild | `ATL-FIFA-Navigator/atl-fifa-navigator-v3` |
| `doctor-ew/atlaiweek-fifa` PR #3 | gstack vs spec-driven comparison | branch `feat/spec-driven-v3` |

---

## Naming Conventions

- **`/drew-product`** = `/drprod` — the spec production harness  
- **`/drew-eng`** = `/dreng` — the adversarial engineering lane  
- **Fafnir** = Claude Code buddy dragon (peak stat: SNARK 100, dump stat: PATIENCE 45)

---

## Important: marta-devdays vs atlaiweek-fifa

**marta-devdays** is a SEPARATE copy of the app specifically for the DevDays demo. It is structured like v2 (has `src/`, uses `lib/types.ts`, `lib/schemas.ts` — the v2 structure). Do NOT apply the v3 structural changes to this repo without checking.

**The v3 structural changes** (types in `src/types/index.ts`, etc.) only apply to the `atlaiweek-fifa` `feat/spec-driven-v3` branch.

---

## Quick Start for Fresh Instance

```bash
# Slides
cd /Users/drew.schillinger/shuttlebay/DoctorEws_Laboratory/_Workshops_/DevDays
bun dev   # Preview slides at localhost:3030

# Demo app
cd /Users/drew.schillinger/shuttlebay/DoctorEws_Laboratory/_Workshops_/marta-devdays
bun dev   # App at localhost:3000

# Check GitHub Pages status
gh repo view doctor-ew/devdays-slides --web
```