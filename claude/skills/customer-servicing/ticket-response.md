# Skill: /ticket-response

Draft a customer-facing response to a support ticket.

## Usage

```
/ticket-response <ticket-id-or-description> [--complaint|--inquiry|--bug|--billing] [--tone formal|friendly]
```

- `<ticket-id-or-description>` — Paste the ticket content or provide a brief description of the issue.
- `--complaint` — Customer expressing dissatisfaction; prioritize empathy and resolution.
- `--inquiry` — Customer asking a question; prioritize clarity and completeness.
- `--bug` — Customer reporting a product defect; acknowledge, gather info, set expectations.
- `--billing` — Billing or payment issue; be precise and avoid ambiguous commitments.
- `--tone` — Response tone: `formal` (enterprise/B2B) or `friendly` (consumer/SMB). Default: `friendly`.

---

## Before drafting

Ask (or infer from context):
1. What outcome does the customer want?
2. Has this issue been resolved, is it in progress, or is the cause still unknown?
3. Are there any account-level escalation flags (at-risk, enterprise, VIP)?
4. Are there any policy constraints on what can be offered (refund eligibility, SLA terms)?

---

## Response structure

**For --complaint:**
1. Acknowledge the frustration (1–2 sentences, sincere, not generic).
2. State what happened or what you know so far.
3. Describe what action you are taking or have taken.
4. Provide a clear next step and timeline.
5. Close with a commitment to follow up.

**For --inquiry:**
1. Directly answer the question (lead with the answer, not preamble).
2. Provide supporting detail or steps if needed.
3. Offer a follow-up path if the answer is incomplete.

**For --bug:**
1. Acknowledge the issue and thank them for reporting it.
2. Confirm whether this is a known issue or under investigation.
3. Request any additional information needed to reproduce (OS, version, steps).
4. Set clear expectations on timeline for a fix or workaround.

**For --billing:**
1. Acknowledge the discrepancy or question factually.
2. State what the records show.
3. Describe the next step (investigation, correction, escalation to billing team).
4. Never promise a refund or credit without authorization — use "I'll look into this and follow up."

---

## Quality checks before outputting

- [ ] No generic opener ("I hope this message finds you well" etc.)
- [ ] Customer's name used at least once if available
- [ ] Concrete next step with an owner and timeline
- [ ] No internal jargon or ticket system references visible to the customer
- [ ] Spelling and grammar checked

---

## After generating

Flag to the agent if:
- The ticket involves a potential SLA breach — escalate to the account manager.
- The customer has mentioned legal action, regulatory bodies, or public escalation — route to management before sending.
- A credit or refund is implied by the draft — confirm authorization before sending.
