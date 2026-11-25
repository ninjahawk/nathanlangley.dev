VERDICT: PASS

Scope read: visible text, titles, meta descriptions and alt text of site/index.html, research.html, projects.html, contact.html; privacy.html skimmed. All files are valid UTF-8 (the em dashes, "Poké" and "©" render correctly).

Checked and clean (no failing findings):
- No self-assessments ("passionate", "driven", "fast learner", "hard-working"): none found.
- No buzzwords ("cutting-edge", "leverage", "synergy", "revolutionary", "game-changing", "seamless", "robust", "state-of-the-art", "groundbreaking"): none found.
- No mention that AI wrote or helped write the text.
- No stale tense: "B.S. expected December 2026", "graduating December 2026", "In November 2026, I entered", "In summer 2026 I also did undergraduate research" are all correct as of 2026-11-24.
- names is consistent across pages: livenerf, Hold 'Em or Fold 'Em, Apart Research AI x Epistemics, Subtext, hollow-agentOS, Claude Opus/Haiku/Sonnet 5.5, "1,900+ GitHub stars" (index and research agree).
- Tone reads as an engineer with results: concrete numbers (78-question locked panel, AUROC 0.78/0.81, 2.3 GPU-hours, 6.8% chance-normalized), and honest negative results ("the data does not yet support the critical assumption", "no change detected", "but not whether incorrect answers were repaired"). That honesty is a strength.

Notes (style or judgement, not failures):
1. contact.html, "I'm open to AI-safety research-engineering roles, fellowships, and research collaboration." This narrows the ask to safety research engineering. A recruiter for AI engineering, ML infrastructure or forward-deployed roles may read it as "not interested". Suggested fix if those roles are wanted: "I'm open to AI-safety research engineering, ML engineering and infrastructure, and forward-deployed engineering roles, plus fellowships and research collaboration."
2. index.html, "I also work on LLM interpretability", "I also study autonomous multi-agent systems", "In summer 2026 I also did undergraduate research". Three "also"s in four paragraphs. Suggested fix: drop "also" from the second and third ("I study autonomous multi-agent systems." / "In summer 2026 I did undergraduate research...").
3. index.html, "what autonomous AI systems do when nobody is watching." Slightly dramatic for an otherwise plain page. Acceptable; a plainer option is "and how autonomous AI agents behave without supervision."
4. projects.html (bongochat), "Raw MMLU is 30.1%; normalized for chance it is 6.8%, which is the point of the chart." Reads like README copy and leans on the thumbnail. Suggested fix: "...normalized for chance it is 6.8%: the chance floor accounts for nearly all of the raw score."
5. projects.html (bongochat), "benchmarked against 2026 frontier models on full test sets". A 125M model against frontier models can read as a joke without the framing; the next sentence supplies it, so this stays. Fine as is.
6. projects.html (S&Poké 500). A Pokémon-card index is the weakest fit for an AI-lab reader, but it shows a shipped daily data pipeline (GitHub Actions, live site) and sits last, so it helps more than it hurts. Optional: lead with the engineering ("rebuilt daily by a GitHub Actions pipeline from TCGplayer prices").
7. Star-count format differs: "1,900+ GitHub stars", "250 GitHub stars" (research.html) vs "311 stars · 52 releases" (projects.html). Suggested fix: "311 GitHub stars". "52 releases" is a weak metric and could be dropped.
8. Link-label casing: "Live Site" (projects.html, S&Poké 500) vs "Live demo", "Sample report", "Server code" elsewhere. Suggested fix: "Live site".
9. research.html, Hold 'Em entry opens "This study tested Claude Haiku 5.5 and Sonnet 5.5..." while the other entries use fragment-style descriptions ("A daily, append-only benchmark...", "A coupled-ODE model..."). Optional: "Tests Claude Haiku 5.5 and Sonnet 5.5 on 300 coding problems each..."
10. Header "Physics Senior & AI-Safety Researcher" vs "AI safety" in body text. Hyphenating as a compound modifier in a title is fine; noting it only for consistency.
11. privacy.html (skim only), "analyse" is British spelling while the rest of the site uses American spelling. Suggested fix: "analyze".

Summary: PASS. No self-assessments, buzzwords, hype, AI-authorship mentions, stale wording or names errors. 11 minor notes, the most useful being widening the roles listed on the contact page.
