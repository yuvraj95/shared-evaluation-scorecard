# PRD — Shared Evaluation Scorecard (MVP)
**Feature:** Shared Evaluation Scorecard  
**Product:** B2B Procurement SaaS  
**Author:** Yuvraj Gulati  
**Status:** MVP Prototype Shipped

---

## 1. Objective

Build an MVP of a Shared Evaluation Scorecard feature that enables procurement teams to collaboratively score vendors against custom criteria in a structured, asynchronous, and time-bound way — with early visibility into stakeholder misalignment.

---

## 2. Goals

| Goal | Metric |
|---|---|
| Reduce vendor evaluation cycle time | Target: 50% reduction |
| Increase stakeholder participation | Target: 90%+ engagement rate |
| Improve decision quality | Misalignments surfaced early, not at end |
| User satisfaction | Target: 4.0/5.0 satisfaction score |

---

## 3. Non-Goals (MVP)

- No ERP or existing procurement system integrations
- No real-time collaboration or live discussion threads
- No AI-based vendor scoring suggestions
- No mobile support (desktop only for MVP)
- No multi-round evaluations

---

## 4. Users

**Primary:** Procurement Managers — create evaluations, monitor progress, make final decisions  
**Secondary:** Evaluators (Legal, Security, Finance, Operations) — score vendors asynchronously

---

## 5. User Stories

**As a procurement manager**, I want to create a vendor evaluation with custom criteria so that all stakeholders score vendors on the same dimensions.

**As a procurement manager**, I want to see who has completed their scoring and where stakeholders disagree so I can address misalignment before making a decision.

**As an evaluator**, I want to score vendors at my own pace, with the ability to add comments for context, so I can contribute meaningfully without attending a meeting.

**As a procurement manager**, I want a deadline enforced automatically so evaluations don't drag on indefinitely.

**As a leadership stakeholder**, I want to receive a clean decision summary with scores and rationale so I can approve or review the procurement decision quickly.

---

## 6. Feature Scope — MVP

### Evaluation Creation
- Procurement manager creates new evaluation
- Adds vendor names
- Defines custom scoring criteria (e.g., cost, compliance, security, support)
- Sets evaluation deadline

### Stakeholder Management
- Invite 5-10 stakeholders by email or user lookup
- Assign roles: Lead Evaluator, Reviewer, Approver
- Stakeholders receive notification with evaluation link

### Scoring Interface
- Each stakeholder scores each vendor against each criterion
- Scoring input: slider or dropdown (1-10 scale)
- Optional free-text comment field per criterion
- Progress indicator showing completion status

### Shared Scorecard View
- Aggregated scores with average and variance per criterion per vendor
- Visual misalignment indicators: color coding (green = aligned, red = high variance)
- Procurement manager can see individual scores per stakeholder

### Time-Bound Evaluation
- Deadline set at creation
- Automated reminders sent to incomplete stakeholders (24h and 4h before deadline)
- Scoring locked automatically after deadline

### Decision Summary
- Final scorecard review view with vendor ranking
- Exportable/shareable summary report
- Export to PDF or shareable link for leadership

---

## 7. Acceptance Criteria

- [ ] Procurement manager can create an evaluation with at least 1 vendor and 1 criterion
- [ ] Up to 10 stakeholders can be invited and assigned roles
- [ ] Each stakeholder can score independently without seeing others' scores until deadline
- [ ] Aggregated scorecard is visible to procurement manager at any time
- [ ] Misalignment (high variance) is visually highlighted on the scorecard
- [ ] Automated reminders fire at 24h and 4h before deadline
- [ ] Scoring is locked after deadline — no late edits
- [ ] Decision summary can be exported as PDF or shared via link
- [ ] All flows work on desktop browsers (Chrome, Safari, Edge)

---

## 8. Success Metrics

| Metric | Target |
|---|---|
| Evaluation cycle time reduction | 50% |
| Stakeholder completion rate | 90%+ |
| User satisfaction score | 4.0/5.0 |
| Misalignments flagged and resolved before final decision | Tracked |
| Support tickets related to evaluation process | Reduction vs baseline |
