# User Flows — Shared Evaluation Scorecard

Full happy path and core workflow documentation for the MVP.

Wireframe: [Excalidraw UI](https://excalidraw.com/#json=FYOLTq4ub2H2iLV8JQGo0,vqVCxb2JP9hd2qkPNqrQjg)  
Happy Flow Diagram: [Excalidraw Flow](https://excalidraw.com/#json=agLYrjwKJtDXrarXezDzT,mqWl5NGhGOolOoB_upAm1w)

---

## Flow 1 — Create Evaluation

**Actor:** Procurement Manager

1. Procurement manager logs in and navigates to Dashboard
2. Clicks "New Evaluation"
3. Enters evaluation name and description
4. Adds vendor names (1 or more)
5. Defines custom scoring criteria (e.g., Cost, Compliance, Security, Support Quality)
6. Sets evaluation deadline date
7. Clicks "Create" — evaluation is created in Draft state

**UI:** Evaluation creation form with inline vendor and criteria builder

---

## Flow 2 — Invite Stakeholders

**Actor:** Procurement Manager

1. From the evaluation detail page, clicks "Invite Stakeholders"
2. Searches for team members by name or email
3. Adds up to 10 stakeholders
4. Assigns role per stakeholder: Lead Evaluator / Reviewer / Approver
5. Clicks "Send Invites"
6. Stakeholders receive email notification with direct link to scoring interface
7. Evaluation status changes from Draft to Active

---

## Flow 3 — Stakeholder Scoring

**Actor:** Evaluator (Legal, Security, Finance, Operations)

1. Evaluator receives email notification with evaluation link
2. Opens scoring interface — sees list of vendors and criteria
3. For each vendor, scores each criterion using a slider or dropdown (1-10)
4. Optionally adds a comment per criterion for context
5. Can save progress and return before deadline
6. Submits scoring when complete — status updates to "Completed" for that stakeholder
7. Procurement manager sees real-time progress on dashboard

**UI:** Scoring matrix — vendors as columns, criteria as rows, input per cell

---

## Flow 4 — View Shared Scorecard

**Actor:** Procurement Manager

1. Navigates to evaluation detail page at any time during active evaluation
2. Sees aggregated scorecard with average score per vendor per criterion
3. Variance indicators show where stakeholders disagree:
   - Green: low variance (aligned)
   - Amber: moderate variance (review recommended)
   - Red: high variance (significant misalignment)
4. Can drill down into individual stakeholder scores per criterion
5. Can identify which stakeholders have not yet completed scoring

---

## Flow 5 — Time-Bound Evaluation

**Actor:** System (automated)

1. System sends reminder to all incomplete stakeholders 24 hours before deadline
2. System sends final reminder 4 hours before deadline
3. At deadline, scoring interface is locked for all stakeholders
4. Late edits are not accepted
5. Procurement manager is notified that evaluation is closed and final scorecard is ready

---

## Flow 6 — Decision Summary

**Actor:** Procurement Manager

1. Opens final scorecard after deadline
2. Reviews vendor rankings by total average score
3. Reviews misalignment areas and individual stakeholder rationale (comments)
4. Adds a final recommendation note
5. Exports decision summary as PDF or generates shareable link
6. Shares with leadership team for approval or sign-off
