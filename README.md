# Future Interns — Prompt Engineering Task 1

## AI Website Copy Generator for Local Businesses

**Task:** Future Interns Prompt Engineering — Task 1  
**Repository format:** `FUTURE_PE_01`  
**Demonstration client:** Crown Studio, Guwahati, Assam  
**Business type:** Boutique/family salon  
**Primary tool:** ChatGPT  
**Research date:** 4 September 2026

---

## 1. Project Objective

This project demonstrates a reusable prompt system for generating conversion-focused website copy for a real local business.

The system is designed to generate:

- Homepage copy with a clear value proposition
- Service-page content
- Persuasive CTA sections
- Tone-adapted copy
- Website-ready output
- A quality-control pass to reduce generic, unsupported, or weak copy

The prompt framework is reusable: a future client can replace the business inputs without rewriting the entire prompt architecture.

---

## 2. Business Chosen

### Crown Studio — Guwahati

Crown Studio is presented on its official website as a boutique salon in Guwahati. Its stated positioning focuses on bespoke trends and editorial elegance. The site highlights three core expertise areas:

1. Hair Styling
2. Skin Therapy
3. Bridal & Makeover

The official site also states that the studio is on Panjabari Road near Biponon Khetra, opposite Organic Market Complex, Barbari Village, Guwahati, Assam 781037, and provides a booking phone number.

### Source

Official website: https://crownstudioluxe.com/

Important: marketing copy in this project is generated from the source facts above. Claims that are not supported by the source are intentionally avoided.

---

## 3. Prompt System Architecture

The workflow is:

```text
Business Inputs
      ↓
Fact / Claim Guard
      ↓
Audience + Goal Definition
      ↓
Value Proposition
      ↓
Homepage Prompt
      ↓
Services Prompt
      ↓
CTA Prompt
      ↓
Tone Adaptation
      ↓
Website Copy QA
      ↓
Final Publish-Ready Copy
```

### Why this is prompt engineering rather than random content generation

The system separates the task into controlled stages. Each stage has:

- Inputs
- Role/context
- Explicit output requirements
- Brand/tone constraints
- Claim-safety rules
- Formatting requirements
- A validation step

This makes the process repeatable across different local businesses.

---

## 4. Deliverables

### Website copy
- Homepage
- Services page
- CTA sections

### Prompt system
- Master workflow
- Homepage prompt
- Services prompt
- CTA prompt
- Tone adaptation prompt
- Quality-control prompt

### Documentation
- Business research/profile
- Prompt logic
- Test cases
- Quality-control results

### Bonus
A static HTML website preview using the generated copy is included in `/website`.

---

## 5. Tools

The Future Interns brief allows suitable AI tools and specifically lists ChatGPT, Claude and Gemini, along with AI website builders such as Lovable and Framer AI.

For this demonstration:

**Primary LLM:** ChatGPT  
**Documentation:** Markdown  
**Website preview:** HTML/CSS  
**Version control target:** GitHub public repository

---

## 6. How to Reuse the System

Replace the fields in `business/business-input-template.md`.

Then run the prompts in this order:

1. `prompts/00_master_system.md`
2. `prompts/01_homepage_prompt.md`
3. `prompts/02_services_prompt.md`
4. `prompts/03_cta_prompt.md`
5. `prompts/04_tone_adaptation.md`
6. `prompts/05_quality_control.md`

For a new client, do not copy unsupported facts from the Crown Studio example. Replace them with verified business information.

---

## 7. Final Result

The generated Crown Studio copy is in:

`outputs/final_website_copy.md`

The prompt testing evidence is in:

`testing/prompt_tests.md`

The business facts used are in:

`business/crown_studio_profile.md`

---

## 8. Submission Checklist

- [x] Real local business selected
- [x] Structured reusable prompts
- [x] Homepage copy
- [x] Services content
- [x] CTA sections
- [x] Tone adaptation
- [x] Quality-control prompt
- [x] Prompt logic documented
- [x] Generated outputs documented
- [x] Business/source information documented
- [x] Website preview included
- [ ] Push repository publicly to GitHub using the required name `FUTURE_PE_01`

