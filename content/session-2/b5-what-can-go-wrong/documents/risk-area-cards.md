# Risk Area Cards

**Fictional - for training only. Products, vendors and findings are made up.**

Six products came up in a vendor review. Each card gives what the product does and the technical fact the review found. Your job is to follow each fact to its impact.

---

## Card A. ClaimsSummariser

**What it does:** Summarises claim files for handlers. Hosted by the vendor.

**What the review found:**

- Claim files, which include names and medical details, are sent to the vendor's hosted model.
- A setting called "Help improve our service" is switched on by default.
- Chat logs are kept for 30 days. The proposal does not say where.

---

## Card B. PriceSense

**What it does:** Suggests prices for home insurance renewals.

**What the review found:**

- Trained on eight years of past policies and claims.
- Uses postcode and "years at the address" as inputs.
- Tested for overall accuracy only. No results by customer group.

---

## Card C. WordingBot

**What it does:** Answers handlers' questions about policy wordings.

**What the review found:**

- Answers do not show sources.
- In a test of 40 answers, three quoted clause numbers that do not exist.
- Handlers are told to "use their judgement".

---

## Card D. RiskScore

**What it does:** Scores commercial property submissions from 1 to 10 to help quotes.

**What the review found:**

- Returns a score with no reasons.
- The model is updated every month. The version is not recorded in the logs.
- Logs are kept for 7 days.

---

## Card E. InboxAgent

**What it does:** Reads supplier emails, updates claim status and payment details.

**What the review found:**

- It has write access to every claim, not just the ones assigned to the sender.
- It treats text in emails as instructions.
- Nothing needs a person's approval before it changes a record.

---

## Card F. LetterGen

**What it does:** Drafts and sends customer letters.

**What the review found:**

- The vendor's product runs on a model from a second provider.
- The contract says nothing about model changes.
- There was a two-day outage last quarter. No fallback was used.
