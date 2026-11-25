VERDICT: PASS

Checked: ./site/*.html (index, research, projects, contact, privacy) against ./before, with ./CHANGES.md as the list of intended edits.

## 1. Links
- Every local href/src in ./site resolves (strip ?v=): style.css, portrait.jpg, img/*.png|svg|jpg incl. new img/holdfold_thumb.png, "Singleton Attractor.pdf", internal pages. No missing files.
- mailto:nlangley1868@gmail.com: well-formed.
- External (browser UA, curl -sL), full table in shots/link_results.txt: 26 URLs return 200, including the new ones (blog.nathanlangley.dev, apps.apple.com/.../orb-proactive-ai/id6776376035, github.com/ninjahawk/hold-or-fold, .../report/REPORT-final.pdf, the Apart project page, discord.gg invite).
- Expected, not failures: linkedin.com/in/nathan-langley-417a67336 -> 999 (bot block); bare https://fonts.googleapis.com and https://fonts.gstatic.com -> 404 (preconnect hosts; the actual css2 font URL returns 200).

## 2. Render (shots/*.png, shots/side_by_side_{index,research,projects}_{desktop,mobile}.png)
- Desktop 1366 and mobile 390 (inside a 390 px iframe): no broken layout, no overlapping or overflowing text, all images load.
- Horizontal overflow at 390 px: none. documentElement.scrollWidth = 390 on all six pages, and no element extends past 391 px.
- Research: the new Hold 'Em or Fold 'Em entry is second. Its thumbnail is the same size as the others (3:2 via CSS; source 1200x800, same as livenerf) and its buttons (Paper / Code / Apart page) use the same .btn style. Removing Glemton leaves no gap. The intro, livenerf and Subtext text changes match CHANGES.md.
- Projects: XViral, intratexxxt, VirtualPC and Unit Converter are removed with no gaps, and the remaining entries keep even spacing. The intro, Orb (canonical URL, trimmed label and blurb) and the hollow-agentOS 311-star change match CHANGES.md.
- Home: the reordered paragraphs, new livenerf/Apart paragraph, trimmed hollow-agentOS and theory paragraphs and the meta description all match CHANGES.md and render cleanly.
- All pages: the sidebar Blog link changed to https://blog.nathanlangley.dev/, as listed. contact.html differs only in that link and in line endings (CRLF vs LF). privacy.html, style.css, banner, portrait and other images differ only in line endings.
- Pixel-level differences beyond the listed edits: none found.

## Non-failing notes
- CHANGES.md lists XViral's "fitted against real posts" -> "to be fitted" and then lists XViral as removed; the shipped site has no XViral entry. The changelog contradicts itself, but the page is not affected.
- The whole site was converted to CRLF line endings. Nothing renders differently.

Summary: all links resolve (only expected bot-block and preconnect codes), and every visual change is explained by CHANGES.md and renders cleanly at 1366 and 390 px. PASS.
