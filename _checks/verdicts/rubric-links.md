# LINKS + RENDER checker for a personal website (nathanlangley.dev), before publishing
You are an independent reviewer. You were given only the files in this folder; you know nothing else about how they were made. Be strict and efficient (aim for under 40 tool calls). Write your verdict to ./verdict.md: the FIRST line must be exactly "VERDICT: PASS" or "VERDICT: FAIL", then a list of every finding (file, quoted text, why, suggested fix). Any single failing finding makes the verdict FAIL. Do not edit anything under ./site. Finish with a one-line summary.

./site = the new version (not live yet; check it as local files). ./before = the currently live version.
1. Links: extract every href and src in ./site/*.html. External URLs: curl -sL -o /dev/null -w '%{http_code}' (use a browser
   User-Agent; LinkedIn may return 999 to bots and fonts.googleapis/preconnect hosts may not return 200 on the bare host: note those as
   expected, not failures). Internal links/images: the file must exist in ./site (strip ?v= query strings). mailto: just check format.
   FAIL on any 4xx/5xx/timeout that is not an expected bot-block, or any missing local file.
2. Render: take headless screenshots of index.html, research.html and projects.html from BOTH ./before and ./site at desktop
   (1366 wide) and mobile (390 wide) widths, full page. Microsoft Edge is at "C:/Program Files (x86)/Microsoft/Edge/Application/msedge.exe"
   (use --headless=new --disable-gpu --hide-scrollbars --screenshot=<abs path> --window-size=W,H with a tall H such as 6000, file:/// URLs).
   Save them in ./shots/ and build side-by-side before|after images (Python PIL) in ./shots/side_by_side_*.png. Look at them.
   FAIL on broken layout, overlapping/overflowing text, missing or broken images, horizontal overflow at 390 px, or any visual change
   other than the new/changed entries (new entries must match the look of existing ones: same thumbnail size, same button style).

AMENDMENT: ./CHANGES.md lists the intended edits (entries added, entries removed, intro and home-page text trimmed or rewritten).
Changes listed there are intended and are NOT failures by themselves; still check that they render cleanly (no gaps, no broken
layout where entries were removed). Any visual change NOT explained by CHANGES.md is still a failure.
