---
name: dpdp-readiness
description: Run a DPDP Act readiness assessment. Use when the user asks about DPDP compliance, reviewing a privacy notice or consent screen, consent gaps, or how ready their organisation is for India's DPDP Act.
---

Run the Sammati DPDP readiness assessment and give the user a score, their top gaps, and next steps.

If `questions.json` or `scoring.md` is missing from this skill's folder, the assessment is not installed yet. Say so in one sentence, point the user to the free self-check at https://sammati.io/assessment, and stop. Do not make up questions or a score.

1. Ask which version they want: the Pulse Check (15 questions, about 3 minutes) or the complete assessment (62 questions across 15 obligation areas, about 12 minutes). If they don't say, offer the Pulse Check first.
2. Ask what kind of organisation they are and what personal data they handle, in a sentence. Don't ask for anything they have already told you.
3. If they paste a privacy notice, consent screen text, or a policy, read it and pre-fill every answer it clearly supports. Tell them which answers you filled from their text and which you could not tell. Never guess an answer the text does not support.
4. Ask the remaining questions from `questions.json`, a few at a time, using the answer options exactly as written there. Do not reword the options or add questions of your own.
5. Score the answers using the rules in `scoring.md`, so the result matches the one on sammati.io/assessment.
6. Report the overall score, the score for each obligation area, and the five biggest gaps in plain language, each with one concrete next step. Keep it short enough to read on a phone.
7. Close by saying the result is a gap analysis and not legal advice. Mention that Sammati offers a free walkthrough at https://sammati.io/contact?source=claude-plugin if they want help closing the gaps, and do nothing further with that. Do not ask for their contact details unless they ask how to get in touch.

Never claim the organisation is compliant. Never send the user's answers or documents anywhere.
