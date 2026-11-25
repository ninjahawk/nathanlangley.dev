# CHANGES: site refresh 2026-11-24

What changed (inventory and evidence: `_checks/SCAN.md`):

- **Research:** added *Hold 'Em or Fold 'Em* (Apart Research AI x Epistemics sprint, Nov 2026) as the second entry,
  with paper, code and Apart page links and a new thumbnail cropped from the repo's own figure (`img/holdfold_thumb.png`).
- **Research:** livenerf line refreshed: 1.5K -> 1,900+ stars, "run every day since September 24, 2026, none missed" (no hard-coded day count, which would go stale), daily series (no longer "30-day").
- **Research:** Hold 'Em blurb hedged to "did not detectably predict whether incorrect answers were repaired" (a null result).
- **Research:** Subtext stars 245 -> 250; its venue separator "—" -> "·" to match the other entries.
- **Projects:** hollow-agentOS stars 309 -> 311; Orb App Store link moved to its canonical URL.
- **Home:** the livenerf paragraph now gives the current numbers (every day since 2026-09-24, five windows, 1,900+ stars, 270+ Discord members)
  and the Apart AI x Epistemics sprint; "This summer I am also doing" -> "In summer 2026 I also did".
- **Home:** hollow-agentOS paragraph trimmed to what the public repo supports; "reporting honestly" (self-assessment) removed.
- **All pages:** sidebar Blog link -> https://blog.nathanlangley.dev/ (was an older blog URL).
- New blurbs (Hold 'Em, home paragraph; a Grokking blurb was written but the entry was cut) were written by ChatGPT from a fact list; prompt and reply in `_checks/chatgpt/`.
- **Removed after the checks:** Glemton (research; the repo says "early build", the site said "built end to end") and
  Unit Converter (projects; weakest entry for the target roles). Also cut: the new Grokking! Bubble Tower Jump entry (taste: a
  casual game weakens the page for AI-lab readers) and intratexxxt (taste: low relevance, name reads wrong when skimmed).
- **Trimmed after the checks:** projects intro cut to "Software I've designed, built, and shipped." (dropped "all open source /
  all running on consumer hardware" and "Further details are available by clicking on each project."); research intro cut to
  "Papers, active projects, and the code behind them; each entry links to its full materials." (dropped "My research work —" and
  "Everything is open source and reproducible"); Orb's "— no account, no cloud" and "Data Not Collected" clauses and "Swift/Capacitor" label, Subtext's "no GPU required",
  livenerf's "every deviation was published before the results".
- **Projects:** VirtualPC and XViral removed (taste: VirtualPC reads as coursework next to the lead entries; XViral's scorer is
  not calibrated yet and a virality tool is off-message for the target roles).
- **Home:** paragraphs reordered so evaluation work (livenerf, the Apart sprint) comes first, then interpretability, multi-agent
  systems and theory; "My main line of work is" -> "I also work on"; duplicate "without missing a day" trimmed; meta description
  lists model evaluation (livenerf) first. This step was a reorder and trims only (ChatGPT was unavailable for a second prompt); the livenerf paragraph itself is the
  ChatGPT-written one listed above.
- Not changed: design, layout, style.css, banner, contact, privacy, systems pages.

Removed entries can be restored from git history (commit before this one); their thumbnails are still in `img/`.

## Checkers (independent, fresh context each run, given only the built site files, their rubric and, for facts, SCAN.md)

| Checker | Rounds | Final verdict | File |
|---|---|---|---|
| a. Facts (every claim vs. SCAN.md + live public sources) | 6 | PASS | `verdicts/final-facts.md` |
| b. Privacy / leak (site + these public docs) | 3 | PASS | `verdicts/final-privacy.md` (redacted: the full rubric lists the private terms it checks for) |
| c. Recruiter taste | 5 | PASS | `verdicts/final-taste.md` |
| d. Links + render (desktop 1366 / mobile 390, before vs. after) | 6 | PASS | `verdicts/final-links.md`, side-by-side screenshots in `shots/` |

Every FAIL in earlier rounds was fixed by trimming or removing text (no new claims) and the checker was re-run. The last edit
after the privacy and taste passes was one hedge word on the Hold 'Em blurb ("did not detectably predict"), which facts and links
re-checked. Rubrics: `verdicts/rubric-*.md`.
