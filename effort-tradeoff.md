# Tech and Effort Tradeoffs — MVP

## Approach

The goal of this MVP is to validate the core value proposition — structured, asynchronous, collaborative vendor evaluation with misalignment visibility — with the minimum viable scope. Every tradeoff below is made to reduce build complexity without compromising the core user value.

---

## Tradeoff Table

| Use Case Included | Tradeoff Made to Keep MVP Light |
|---|---|
| Multi-stakeholder collaborative scoring | Limit to 5-10 stakeholders per evaluation |
| Customizable evaluation criteria | Manual criteria setup — no AI-suggested or template criteria |
| Score visualization and misalignment detection | Simple color-coded variance indicators — no advanced analytics |
| Time-boxed evaluations with reminders | Asynchronous input only — no real-time co-editing |
| Summary dashboard | Simplified view — no detailed reporting or drill-down exports beyond PDF |
| Platform support | Desktop only — mobile support deferred to post-MVP |

---

## Additional Tradeoffs

### No ERP or Procurement System Integrations
**Decision:** Build as a standalone tool for MVP  
**Reason:** Integrations add significant engineering complexity and dependency risk. Core value can be validated without them.  
**Post-MVP:** Integration with tools like SAP Ariba, Coupa, or internal ERP systems based on enterprise demand.

### No Real-Time Collaboration
**Decision:** Asynchronous scoring only — stakeholders cannot see each other's scores until deadline  
**Reason:** Prevents anchoring bias (early scores influencing later ones). Keeps the build simpler. Aligns with how procurement teams actually work across time zones.  
**Post-MVP:** Optional discussion threads per criterion after scoring is complete.

### No AI Scoring Suggestions
**Decision:** Human scoring only for MVP  
**Reason:** AI suggestions require historical vendor data and training that doesn't exist yet. Building this prematurely would produce low-quality suggestions and erode trust.  
**Post-MVP:** AI-based scoring recommendations after sufficient data is collected from real evaluations.

### No Mobile Support
**Decision:** Desktop only  
**Reason:** Procurement evaluation is a considered, time-intensive task — not a mobile use case for the primary user. Reduces responsive design scope significantly for MVP.  
**Post-MVP:** Mobile-responsive UI based on usage data.

### Manual Reminder Configuration
**Decision:** Fixed reminder schedule (24h and 4h before deadline)  
**Reason:** Configurable reminders add UI and logic complexity. Fixed schedule covers 90% of use cases for MVP.  
**Post-MVP:** Configurable reminder frequency per evaluation.

---

## What We Are NOT Building in MVP

- ERP / procurement system integrations
- Real-time collaboration or live discussion threads
- AI-based vendor scoring suggestions
- Multi-round evaluations
- Role-based access controls beyond Lead / Reviewer / Approver
- Audit logs for compliance
- Mobile support
- Advanced analytics and custom reporting dashboards
