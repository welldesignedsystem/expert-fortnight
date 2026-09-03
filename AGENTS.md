# AGENTS.md — AEO Intel 90-Day AEO/SEO/GEO Growth Operation

This file documents the whole system the way an `AGENTS.md` documents a coding project: who's doing what, in what order, using which files, checked against what definition of done. Treat this as the single source of truth for how the 90-day plan actually runs day to day. If anything in the other files conflicts with this one, this file wins — update it first when the plan changes.

---

## 1. Mission

Fix AEO Intel's AI/search visibility (currently near-zero, per the technical audit — see Section 2) and build a repeatable, ownable content system across blog + LinkedIn + Instagram + Facebook, run over a 90-day cycle, with results tracked well enough to become a public case study at the end.

**Two success conditions, not one:**
1. The site becomes crawlable and citable by AI engines (technical fix).
2. A sustained publishing cadence runs for 90 days without gaps (execution discipline) — most plans like this fail from inconsistency, not from a bad strategy.

---

## 2. Starting state (why this plan exists)

A direct fetch of `https://www.aeo-app.ai` returned almost no content — just a page title and meta description. That means the site is very likely a JavaScript-rendered SPA that doesn't serve finished HTML to crawlers. AI crawlers (GPTBot, ClaudeBot, PerplexityBot, Google-Extended) and search bots behave like that fetch — if they can't see it, none of the content strategy below matters until it's fixed. This is why **Phase 1 is entirely technical and gates everything else.**

Full detail: `aeo-app-ai_AEO-SEO-GEO_Growth_Report.md`

---

## 3. Roles ("agents") and their scope

Each person owns a lane. Work should not cross lanes without a handoff noted in the tracker (Section 8).

### Founder
- **Owns:** product strategy, personal LinkedIn voice, Phase 1 technical decisions (with a developer), final sign-off at Day 30/60/90 checkpoints, and the go/no-go decision to enter Phase 2.
- **Does not own:** carousel design, blog drafting — those are delegated so the founder's time stays on judgment calls, not production.
- **Recurring tasks:** personal LinkedIn POV/data/wrap-up posts (Mon/Tue/Thu/Fri per the calendar), weekly 15-minute review of the Progress Tracker.
- **Why personal, not company page:** LinkedIn's algorithm gives personal profiles 5-10x the organic reach of company pages. The Founder's personal voice (POV, data, lessons) is the high-reach channel; Shahana's polished carousels on the company page carry the branded presence. They are two distinct channels by design.

### Nivedya — Blog
- **Owns:** all 20 blog posts (10 tactical + 10 pillar), written directly from the prompts in the Content Library.
- **Definition of done for a blog post:**
  - Opens with a direct answer in the first sentence (not a windup)
  - Matches the word count and structure specified in its prompt
  - Includes FAQPage/Article schema before publishing (coordinate with Founder/Dev if schema isn't self-serve)
  - Internally links to 2-3 other blog posts and 2-3 product pages
  - No fabricated statistics — anywhere a prompt is marked **[NOTE TO WRITER]**, real data must be sourced before publishing
  - Published on the exact day assigned in the schedule, not batched late
- **Weekly output:** 2 posts (Tuesday tactical, Thursday pillar)
- **Logs into:** Progress Tracker → "Blog Posts Published (cumulative)" column, every Friday

### Shahana — Carousels & Visuals
- **Owns:** LinkedIn Company Page posts, Instagram feed/carousel/Stories, Facebook posts — everything visual/repurposed.
- **Definition of done for a carousel/poster:**
  - Uses the exact prompt from the Content Library (slide count, word limits, tone)
  - Follows brand visual system: indigo `#4F46E5` + white, bold typography, no stock photography, minimal geometric accents
  - Repurposes that week's blog post — do not create original topics outside the calendar without checking with Founder first
  - Caption includes the required engagement question + hashtag set where specified
  - Published on the exact day/channel assigned
- **Weekly output:** 3 LinkedIn Company posts, 3-4 Instagram feed posts, ~5 Instagram Stories, 2-3 Facebook posts
- **Logs into:** Progress Tracker → "Carousels/Posters Published (cumulative)" column, "LinkedIn Followers," "Instagram Followers," every Friday

---

## 4. File map (the "context" this operation runs on)

| File | Purpose | Owner reads it for |
|---|---|---|
| `aeo-app-ai_AEO-SEO-GEO_Growth_Report.md` | Full technical audit + strategy rationale | Founder (Phase 1 decisions), anyone who wants the "why" |
| `AEO-Intel_Content_Prompts_Library.md` | All 20 blog prompts + carousel/poster prompts, standalone | Nivedya (blog prompts), Shahana (carousel/poster prompts) |
| `AEO-Intel_Full_Schedule_and_Content_Library.md` | Everything above, merged into one self-contained file with working in-file links | Anyone who wants one file instead of three |
| `AEO-Intel_90-Day_Day-by-Day_Activity_Calendar.xlsx` | Same schedule as a filterable spreadsheet, plus the **Progress Tracker (Case Study)** sheet | Whoever is logging weekly metrics; best for the actual tracking (formulas/filtering) |

**Rule:** the spreadsheet is the working file for logging results (it's built for that). The markdown files are the working files for content production (prompts, links, portability). Don't try to log metrics into the markdown — it has no tracker table.

---

## 5. Operating cadence — how each phase actually runs

### Phase 1 — Days 1-14 — "Foundation" (no publishing yet)
One technical task per day, owned by Founder/Dev, e.g. robots.txt audit → SSR fix → schema → llms.txt → cornerstone page → tooling setup. Full task list is in the calendar/table.
**Exit condition:** Day 14's task is explicitly "go/no-go for Phase 2" — do not start Phase 2 on schedule if crawlability isn't actually fixed. A late Phase 1 is better than an invisible Phase 2.

### Phase 2 — Days 15-84 — "Full Cadence" (10 weeks)
Repeats the same weekly rhythm every week:
- **Tue/Thu:** Nivedya publishes a blog post (tactical/pillar alternating)
- **Mon/Wed/Fri:** Shahana publishes LinkedIn Company + Instagram + (partial) Facebook
- **Mon/Tue/Thu/Fri:** Founder publishes personal LinkedIn
- **Daily weekdays:** Shahana posts Instagram Stories
- **Every Friday:** whoever has data that week fills in the Progress Tracker row for that week

Each week's social content **repurposes** that week's blog post — Nivedya's output is upstream of Shahana's, so blog posts should go out on schedule to avoid blocking the carousel/poster work.

### Phase 3 — Days 85-90 — "Checkpoint & Case Study"
Joint task, all three roles: re-run the AI citation test, pull all analytics, identify top-performing content, refresh weak posts, and write up the Day 90 results — which becomes the basis for the "What 90 Days of Consistent AEO Content Actually Looks Like" blog post already scheduled in Week 9 of the Content Library.

---

## 6. Definition of done for the *system*, not just individual tasks

A week counts as "on track" only if all of the following are true by Sunday night:
- [ ] Both blog posts published on their assigned days (not late, not batched)
- [ ] All 3 LinkedIn Company posts published
- [ ] Founder's LinkedIn posts published per the weekly plan
- [ ] Instagram feed + Stories cadence held
- [ ] Facebook posts went out (repurposed, not skipped)
- [ ] Progress Tracker row for that week is filled in — even partially — by Friday

If more than one of these slips in a given week, flag it at the next weekly review rather than letting it compound silently. Two consecutive missed weeks is the threshold for reassessing the cadence itself (see Section 7) rather than just pushing through.

---

## 7. Review protocol

- **Weekly (every Friday):** 15-minute check — did the week hold cadence, what got logged in the tracker, anything to adjust for next week.
- **Day 30 checkpoint:** review indexing status, early follower growth, engagement rate trend. Do not expect traffic or AI citation gains yet — too early. This is a "did the system run" check, not a "did it work" check.
- **Day 60 checkpoint:** first real signal — keyword ranking movement, traffic trend, re-run the manual AI-citation test from Day 1 baseline.
- **Day 90 checkpoint:** full report. Decide whether to continue the same cadence, adjust it, or expand it (e.g. add a channel, add a person) for the next 90-day cycle.

---

## 8. Guardrails (do not violate these regardless of deadline pressure)

- **Never publish a fabricated statistic.** Every `[NOTE TO WRITER]` in the Content Library must be resolved with real data before that post goes live. AI engines penalize sources caught with inaccurate figures — this isn't just an ethics rule, it actively damages the goal.
- **Never skip Phase 1's exit check.** Publishing 90 days of content onto a site AI crawlers can't read wastes the entire quarter. Confirm crawlability before Phase 2 starts, not after.
- **Keep visual brand consistent** (indigo `#4F46E5` + white, no stock photography) across every asset Shahana produces — this is what makes AEO Intel recognizable across 4 channels without a logo doing all the work.
- **Don't invent new topics mid-cycle** without checking against the Content Library first — the 20-post arc is sequenced deliberately (technical → structuring → data/authority → APAC → measurement → case study → capstone). Random insertions break that narrative build.
- **Log the tracker even in a bad week.** A missing row is worse than a row that honestly shows a slow week — the whole point of the tracker is that it becomes the real case study at Day 90, and a case study with gaps is less credible, not more flattering.

---

## 9. What "Founder" means in this file specifically

Per your question earlier: "Founder" is a placeholder for whoever leads AEO Intel — it was never assigned a real name because only Nivedya and Shahana were specified. If a third person owns this role, replace every instance of "Founder" across this file, the schedule table, and the spreadsheet's "Assigned To" column with their actual name — say the word and I'll do the replacement everywhere consistently in one pass.
