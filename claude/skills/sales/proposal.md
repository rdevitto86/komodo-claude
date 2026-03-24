# Skill: /proposal

Draft a sales proposal or quote document for a prospect.

## Usage

```
/proposal <prospect-name> [--executive|--technical|--full] [--renewal]
```

- `<prospect-name>` — Company or contact name for the proposal.
- `--executive` — Executive summary only (1–2 pages): problem, solution, investment, next steps.
- `--technical` — Technical specification section only: architecture, integration, implementation plan.
- `--full` — Complete proposal including all sections (default).
- `--renewal` — Renewal or expansion proposal for an existing customer (adjust tone; reference existing relationship and outcomes).

---

## Before drafting

Ask the user for:
1. Prospect's stated problem or goal (verbatim from discovery if available).
2. Proposed solution and key features / services included.
3. Pricing: tier, seat count, contract term, one-time vs. recurring.
4. Competitive context: any known alternatives the prospect is evaluating.
5. Key stakeholders: economic buyer, champion, technical evaluator.
6. Agreed next steps or desired close date.

---

## Proposal sections

### Cover page
- Prospect company name and logo placeholder
- "Prepared for: [Contact Name], [Title]"
- "Prepared by: [Your Name], [Your Title]"
- Date and proposal validity period

---

### Executive summary (--executive or --full)

**The problem:**
Summarize the prospect's challenge in their language. Use specific details from discovery.

**Our solution:**
One paragraph: what we're proposing and why it addresses their specific problem better than alternatives.

**Expected outcomes:**
2–3 concrete outcomes with estimated metrics where possible (e.g. "reduce manual reconciliation time by ~40%").

**Investment:**
High-level pricing summary (detailed pricing in a separate section).

**Proposed next steps:**
1. [Action] — [Owner] — [Date]
2. ...

---

### Situation and requirements (--full)

Restate the prospect's requirements and constraints as understood. This section builds trust by showing you listened. Flag any requirements not covered by the proposed solution.

---

### Proposed solution (--full)

- Solution overview with key capabilities
- How it maps to each stated requirement
- What's included vs. out of scope
- Implementation timeline (phases, milestones, estimated duration)

---

### Technical details (--technical or --full)

- Architecture diagram placeholder
- Integration points and prerequisites
- Security and compliance posture
- Data handling and privacy
- Performance and SLA commitments

---

### Pricing and terms (--full)

| Item | Description | Qty | Unit Price | Total |
|------|-------------|-----|------------|-------|
| ... | ... | ... | ... | ... |

- Contract term: [X months / years]
- Payment terms: [net 30, annual upfront, etc.]
- Proposal valid until: [date]
- Any discounts applied and conditions

---

### Why us (--full)

3–4 differentiated reasons, not generic claims. Include a relevant customer proof point or case study excerpt.

---

### Next steps

| Action | Owner | Date |
|--------|-------|------|
| Sign proposal | [Prospect] | [Date] |
| Kickoff call | [AE + Prospect] | [Date] |
| ... | ... | ... |

---

## After generating

Remind the rep to:
- Have legal review any non-standard terms before sending.
- Confirm pricing with management if any discounts exceed standard thresholds.
- Send as a PDF with tracking enabled (DocuSign, PandaDoc, or similar).
- Log the sent proposal in CRM with the expected close date and deal value.
