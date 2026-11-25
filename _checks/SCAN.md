# SCAN: public work vs. what nathanlangley.dev shows (2026-11-24)

Evidence was read live on 2026-11-24 (~20:00 ET): GitHub API (`gh api users/ninjahawk/repos`, public, non-fork),
the iTunes lookup API for his developer account (artist id 6776376037), blog.nathanlangley.dev, Apart Research project pages.
Only public, shipped work is listed. Forks are excluded.

| Item | On site before? | Evidence | Decision + why |
|---|---|---|---|
| livenerf | yes (research #1, "1.5K stars") | github.com/ninjahawk/livenerf: 1,997 stars, last push 2026-11-24; README "Progress (2026-11-24): 62 days collected, none missed", "five full 10-day windows after launch week, no change detected"; Discord invite discord.gg/JRGCUg2pyX: approximate_member_count 290 from the public invite API discord.com/api/v9/invites/JRGCUg2pyX?with_counts=true (2026-11-24) | UPDATE: stars 1.5K -> 1,900+, 62 days none missed; home-page paragraph refreshed; "every deviation was published before the results" trimmed (deviations are logged as they happen) |
| Hold 'Em or Fold 'Em (Apart AI x Epistemics sprint, Nov 2026, solo, Track 1) | no | github.com/ninjahawk/hold-or-fold (public, created 2026-11-15, report/REPORT-final.pdf); README: Haiku 5.5 + Sonnet 5.5, 300 coding items each from MBPP+, HumanEval+ and trap variants, three escalating rebuttals, code run after every turn; hero figure: AUROC of initial confidence 0.78 (Haiku) / 0.81 (Sonnet) for holding when initially correct, 0.39 / 0.57 for fixing when initially wrong; Apart project page apartresearch.com/sprints/projects/hold-em-or-fold-em-...-q9ox14r69w (200) | ADD to research, second entry: newest AI-safety work, has numbers and a paper |
| Orb - Proactive AI (iOS) | yes (projects #1) | App Store id6776376035, version 1.0.11 released 2026-11-23, first release 2026-07-14; canonical URL apps.apple.com/us/app/orb-proactive-ai/id6776376035 | UPDATE link to the canonical App Store URL; drop the "Data Not Collected" clause (the live label reads "Data Not Linked to You") and the unverified "Swift/Capacitor" label |
| Grokking! Bubble Tower Jump (iOS game) | no | App Store id6788521690, version 2.0 released 2026-11-22, Games, "Plays offline. No ads, no in-app purchases. Your progress stays on your device."; support page ninjahawk.github.io/grokking-support/ (200) | SKIP after the taste check: a casual game with a thin blurb weakened the projects page for AI-lab readers |
| hollow-agentOS | yes ("309 stars") | github.com/ninjahawk/hollow-agentOS: 311 stars, 52 releases | UPDATE stars |
| Subtext | yes (research only) | github.com/ninjahawk/Subtext: 250 stars | UPDATE stars (245 -> 250); drop "no GPU required" (only the recorded demo runs without a GPU). Stays on research only (his 2026-07-12 call) |
| Confessor | yes | 10 stars, live sample report ninjahawk.github.io/Confessor/ | keep |
| Singleton Attractors preprint | yes | PDF in repo; github.com/ninjahawk/singleton-attractor (7 stars) | keep |
| Glemton (glemton-2) | yes (research) | github.com/ninjahawk/glemton-2 README: "Status: Early build", pipeline steps unchecked | REMOVE: the site said "built end to end", which the repo does not support yet; bongochat already shows a from-scratch model run |
| swarmsim | yes | 9 stars | keep |
| Redcoder | yes | public repo | keep |
| XViral | yes | 8 stars; README: withheld weights are free parameters "to be fitted", not yet calibrated | REMOVE after the taste check: scorer not calibrated yet; a virality tool is off-message for the target roles |
| bongochat | yes | 6 stars, v1.0 release | keep |
| intratexxxt | yes | public repo, 1 star | REMOVE after the taste check: low relevance to the target roles, and the name can read wrong to a skimming recruiter |
| VirtualPC | yes ("24 stars") | 24 stars | REMOVE after the taste check: reads as coursework next to the lead entries |
| S&Poke 500 | yes | poke500.com (200), repo S-and-Poke-500 updated daily | keep |
| Unit Converter (Android) | yes | Google Play page (200) | REMOVE: weakest entry for the target roles (taste check) |
| Blog | yes (sidebar, older blog URL) | blog.nathanlangley.dev (200), 21 posts | UPDATE sidebar link to blog.nathanlangley.dev |
| teleporty | no | 16 stars; speculative teleportation notes | SKIP: removed from the site on 2026-07-11 (his call); not relevant to the roles |
| KillClawd, Backlot | no | public repos | SKIP: he removed both on 2026-10-16; never re-add |
| research-plan, mech, mathchat, grokking-support, small/old repos | no | empty or near-empty READMEs, or support pages | SKIP: not portfolio items |
| hollow-agentOS home-page paragraph | yes | public autonomy log last updated 2026-04-03 does not record the "agent targeting its own execution engine" episode | TRIM to the validation-gate claim that the repo README supports |
