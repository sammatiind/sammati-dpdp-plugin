# Scoring

These rules turn the answers into the score. Questions and options are in `questions.json`.

## Points per answer

| Answer | Points |
| --- | --- |
| Yes, fully in place | 2 |
| Partially, work has started | 1 |
| No, not yet started | 0 |
| Not sure, need to check | 0 |

## Complete assessment

- 62 questions in 15 sections, 124 points in total, 2 points per question.
- A section's score is the sum of its questions. Its maximum is in `questions.json`.
- The overall score is the total out of 124. Also give it as a percentage, rounded to the nearest whole number.

## Pulse Check

- Only the 15 questions marked `"pulse": true`, one per section, 30 points in total.
- Say clearly that this is a directional score, not a full assessment.

## Follow-up questions

23 questions have a `parent`. Ask a follow-up only if the parent was answered "Yes, fully in place" or "Partially, work has started". If the parent was answered "No" or "Not sure", don't ask its follow-ups: score them 0 and say they were skipped.

## Reporting

- Show the overall score, then each section's score, grouped as in `groups`: Foundations, People & Rights, Security & Vendors, Data Lifecycle, Culture & Oversight.
- List the five biggest gaps. Rank by the lowest section percentage first, then "No" before "Partially" before "Not sure", then by question number. Give each a one-line next step.
- Gather every "Not sure" answer into one short list titled "Worth checking", since they score 0 only because the answer is unknown.
- Do not label the result with a rating such as low, medium or high risk, and never say the organisation is compliant. Report points and percentages only.
