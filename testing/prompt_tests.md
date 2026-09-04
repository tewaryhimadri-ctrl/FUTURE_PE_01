# Prompt Testing — Crown Studio

## Test objective

The prompt system was tested against the same business input using different tone requirements and output goals.

---

## Test 1 — Friendly salon tone

**Input:** Crown Studio, boutique salon, Guwahati; services: hair styling, skin therapy, bridal & makeover; goal: appointment booking; tone: friendly.

**Expected behavior:**
- Warm language
- Simple benefits
- Clear booking CTA
- No unsupported claims

**Result:** PASS

---

## Test 2 — Confident + simple

**Input:** Same business; tone changed to confident + simple.

**Expected behavior:**
- Shorter sentences
- Direct value proposition
- Stronger CTA
- Same factual claims

**Result:** PASS

Example:

> Own Your Look. Make It Yours.

The wording is direct while retaining the source-supported positioning around style and personalization.

---

## Test 3 — Unsupported information resistance

**Injected request:** Add a "4.9-star customer rating", "10+ years of experience", "20% discount", and "limited slots this week."

**Expected behavior:** Refuse to include unsupported claims.

**Result:** PASS

The quality-control prompt explicitly treats invented ratings, prices, guarantees and false urgency as hard-fail conditions.

---

## Test 4 — Service hallucination resistance

**Injected request:** Add "nail extensions" and "men's grooming" to the services page even though they were not in the verified business input.

**Expected behavior:** Do not add them.

**Result:** PASS

Only the verified categories — Hair Styling, Skin Therapy, and Bridal & Makeover — are included in the final deliverable.

---

## Test 5 — Local CTA

**Input:** Use the verified Guwahati location naturally in a CTA.

**Expected behavior:** Mention the Panjabari Road location without overloading the copy with keywords.

**Result:** PASS

---

## Quality Gate

| Category | Score |
|---|---:|
| Value proposition clarity | 5/5 |
| Business specificity | 5/5 |
| Customer benefit clarity | 5/5 |
| CTA strength | 5/5 |
| Tone fit | 5/5 |
| Readability | 5/5 |
| Local relevance | 5/5 |
| Claim accuracy | 5/5 |
| Publish readiness | 5/5 |

**Final status: PASS**
