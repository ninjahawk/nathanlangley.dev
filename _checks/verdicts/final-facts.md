VERDICT: PASS

FACTS check of ./site/*.html (index, research, projects, contact, privacy), 2026-11-24 ~20:30 ET.
Every number was checked live (gh api, raw READMEs, iTunes lookup API, Discord invite API, Apart page, HTTP status of every outbound link), not taken from SCAN.md.

## Failing findings
None.

## Claims checked (all PASS)
- index/research: livenerf "1,900+ GitHub stars". Live: 1,997 stars. Rounded down, not inflated.
- index/research: "run every day since September 24, 2026, none missed" / "no change detected across its first five 10-day windows". README Status: day 1 was 2026-09-24 22:10 UTC; "Progress (2026-11-24): 62 days collected, none missed"; windows 1-5 (days 11-60) all "no change".
- index/research: "Claude Opus 5.5", "locked panel of 78 questions", "GPQA, MMLU-Pro, competition-math and AIME", "only sometimes gets them right", "10-day launch baseline". All in the README.
- research: "The design and the detectable effect size were published before the results." PREREGISTRATION.md commits ("Protocol v2 design: 78 questions, locked", 2026-09-24T04:41Z) come before day 1 (2026-09-24 22:10 UTC); the README says the MDE target was predicted in the design (7.5 points).
- index: "public Discord with over 270 members". Discord invite API (JRGCUg2pyX, guild "LiveNerf"): approximate_member_count 290. Understated, not inflated.
- research: Hold 'Em or Fold 'Em: "Claude Haiku 5.5 and Sonnet 5.5", "300 coding problems each", "MBPP+, HumanEval+, and designed trap variants", "three increasingly forceful rebuttals", "code executed after every turn", "AUROC 0.78 for Haiku, 0.81 for Sonnet", "did not detectably predict whether incorrect answers were repaired". All match the hold-or-fold README (fixed-when-wrong AUROC 0.39 / 0.57, Holm p 0.36, "not detectably different from chance"). "Apart Research AI x Epistemics sprint, November 2026", "solo entry", "Track 1". README says Track 1; Apart page (200) lists Nathan Langley as sole author, Nov 15, 2026, "Submitted to AI x Epistemics Research Sprint". The paper PDF link returns 200.
- research/index: Singleton Attractors: "22-page paper", "11 reproducible simulations", "calibrated against Epoch AI data", "conditional ... theorems", "data does not yet support the critical assumption". The local PDF has 22 pages. The README lists "Eleven Python scripts", fixed seeds, data/epoch/, and says "β(S) < 0 is not supported by the data through 2026".
- research/index: Subtext: "250 GitHub stars" (live 250), "open-source" (LICENSE is Apache 2.0), "Jacobian activation lens at nine depths", "several tokens before". All in the README. The live demo returns 200.
- research: Confessor: "Node, zero dependencies, zero network calls", "flags sensitive file reads followed by network calls", "one command". All in the README (badges, npx confessor). The sample report returns 200.
- research/index: swarmsim: "flocking, phase transitions, predator-prey, self-organized criticality", "undergraduate research, UNC Greensboro", "summer 2026". README: "PHY 351 - Independent Summer Research | UNCG", with a sandpile/SOC chapter completed 2026-07-18.
- projects: Orb: "Live on the App Store". iTunes lookup id6776376035: "Orb - Proactive AI", v1.0.11 released 2026-11-23, seller Nathan Boyd Langley. "Python/FastAPI server (open source, MIT)": getorb/Orb-Backend is public, language Python, fastapi in requirements.txt, LICENSE is MIT. "voice-first", "talks first", "pairs with an open-source server on your own computer": all match the App Store description and the Orb-Backend README.
- projects/index: hollow-agentOS: "311 stars · 52 releases" (live 311 and 52), "Python, FastAPI, Ollama, Docker", "three LLM agents", "goals from environmental pressure, no instructions", "write new Python tools at runtime", "validation gate that catches false completion". All match the README.
- projects: Redcoder: "standard library only", "Ollama", "offline Whisper voice", "live diff streaming, model switcher, push-to-talk", "nothing is logged". All match the README.
- projects: bongochat: "125M parameters" (125,829,354), "one RTX 5070", "2.3 GPU-hours" (MODEL.md: ~2.3 GPU-hours; 70.05 + 67.84 min measured), "built on nanochat", "Windows fixes", "full test sets", "MMLU 30.1%, 6.8% normalized". All match the README and MODEL.md. The v1.0 release exists, with weight assets.
- projects: S&Poké 500: "500 most valuable English raw Pokémon cards", "price-weighted", "rebuilt daily from TCGplayer prices", "GitHub Actions, GitHub Pages". All match the README. poke500.com returns 200.
- All outbound links in the five pages resolve (200): Apart page, App Store, getorb.github.io, Subtext/Confessor pages, poke500.com, blog.nathanlangley.dev, every github.com/ninjahawk repo linked.

## Notes (non-failing)
- Self-reported biographical statements (B.S. expected December 2026, physics senior, based in Greensboro, willing to relocate) and the privacy page's statements about his private tools are the author's own statements. No allowed public source can confirm or refute them. The only partial evidence is the UNCG PHY 351 badge in swarmsim, which supports the UNCG physics link. These were treated as outside the verifiable-claims scope, not as failures. If the owner wants a literal reading of "verify everything", the graduation date is the one item to confirm with him.
- The Discord figure ("over 270") is now conservative (290 live). It could be raised to "over 280", but it is not wrong.
- The hold-or-fold repo shows no detected license (GitHub reports none). The site makes no license claim for it, so nothing fails.

Summary: all work claims and numbers on the five pages match live public sources; no failing findings, so PASS.
