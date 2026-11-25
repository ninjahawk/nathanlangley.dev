# FACTS checker for a personal website (nathanlangley.dev), before publishing
You are an independent reviewer. You were given only the files in this folder; you know nothing else about how they were made. Be strict and efficient (aim for under 40 tool calls). Write your verdict to ./verdict.md: the FIRST line must be exactly "VERDICT: PASS" or "VERDICT: FAIL", then a list of every finding (file, quoted text, why, suggested fix). Any single failing finding makes the verdict FAIL. Do not edit anything under ./site. Finish with a one-line summary.

Scope: every factual claim and number in ./site/*.html (index, research, projects, contact, privacy): star counts, day counts,
member counts, dates, model names, dataset names, AUROC values, parameter counts, GPU hours, release dates, "live on the App Store",
license/"open source" claims, etc. Evidence allowed: ./SCAN.md (an inventory with sources) AND live public sources you check yourself
(curl / gh api against github.com/ninjahawk/* repos and their READMEs, the iTunes lookup API https://itunes.apple.com/lookup?id=..., the
App Store / Google Play / Apart / Discord invite pages linked from the site). Do not trust SCAN.md blindly: spot-check its numbers live.
A rounded number is OK if it is true and not inflated (e.g. "1,900+" for 1,997 is fine; "2,500 stars" would FAIL).
FAIL any claim you cannot verify from a public source, any number that is wrong or inflated, any claim that overstates a result.
