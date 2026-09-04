# Reusable Business Input Template

Use this file as the input layer for the prompt system.

```yaml
business_name: "[BUSINESS NAME]"
business_type: "[SALON / CAFE / CLINIC / COACHING / AGENCY / OTHER]"
location: "[CITY, AREA, COUNTRY]"

business_description: "[1–3 factual sentences]"
target_customers: "[WHO THE BUSINESS SERVES]"
primary_goal: "[BOOKINGS / CALLS / ENQUIRIES / VISITS / OTHER]"

verified_services:
  - name: "[SERVICE]"
    details:
      - "[VERIFIED DETAIL]"
  - name: "[SERVICE]"
    details:
      - "[VERIFIED DETAIL]"

verified_differentiators:
  - "[FACTUAL DIFFERENTIATOR]"

brand_tone: "[FRIENDLY / PROFESSIONAL / CONFIDENT / PREMIUM / SIMPLE]"
preferred_language: "[LANGUAGE]"
cta_action: "[BOOK / CALL / VISIT / ENQUIRE]"

contact:
  phone: "[PHONE IF VERIFIED]"
  website: "[URL IF VERIFIED]"
  address: "[ADDRESS IF VERIFIED]"
```

## Claim-safety rule

Only use factual business claims that are supplied or verified.

If a detail is unknown, do not invent it. Use neutral wording or mark it as requiring client confirmation.
