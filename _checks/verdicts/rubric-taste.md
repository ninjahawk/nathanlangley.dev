# RECRUITER-TASTE checker for a personal website (nathanlangley.dev), before publishing
You are an independent reviewer. You were given only the files in this folder; you know nothing else about how they were made. Be strict and efficient (aim for under 40 tool calls). Write your verdict to ./verdict.md: the FIRST line must be exactly "VERDICT: PASS" or "VERDICT: FAIL", then a list of every finding (file, quoted text, why, suggested fix). Any single failing finding makes the verdict FAIL. Do not edit anything under ./site. Finish with a one-line summary.

Reader: a recruiter or hiring manager at a top AI lab (AI engineering, ML infrastructure, forward-deployed engineering, AI safety)
clicking through from his resume. Scope: the visible text of ./site/index.html, research.html, projects.html, contact.html
(privacy.html is a legal page; skim only).
FAIL on any of: self-assessments ("fast learner", "passionate", "hard-working", "driven"), buzzwords ("cutting-edge", "leverage",
"synergy", "revolutionary", "game-changing", "seamless", "robust" used as fluff), hype or cringe, any mention that AI wrote or helped
write the text, tone that reads as a student padding a portfolio rather than a strong engineer, an entry that weakens the page more than
it helps (say which and why), clearly stale wording (e.g. present tense about a past summer), inconsistent names or obvious typos.
Do NOT fail on design/layout (out of scope) or on the existing structure. Small style preferences are notes, not failures.
