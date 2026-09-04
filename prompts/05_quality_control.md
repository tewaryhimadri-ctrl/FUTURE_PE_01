# Website Copy Quality-Control Prompt

Review the generated copy against the business input.

Score each category from 1–5:

1. Value proposition clarity
2. Business specificity
3. Customer benefit clarity
4. CTA strength
5. Tone fit
6. Readability
7. Local relevance
8. Claim accuracy
9. Publish readiness

## Hard-fail conditions

Mark `FAIL` if the copy:
- invents a price
- invents a review/rating
- invents an award/certification
- invents a service
- invents a guarantee
- invents a business result
- invents a contact detail
- makes an unsupported medical claim
- uses fake scarcity or false urgency

## Revision step

For every category below 4, provide one specific revision.

Then output a final corrected version.

## Final gate

Return:

`PASS` only when there are no hard-fail conditions and every score is at least 4.
