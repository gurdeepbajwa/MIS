# DBA Weak Areas Cheat Sheet

Course: [[Digital Business Analysis (ISYS90049)/Course Overview|Digital Business Analysis (ISYS90049)]]
Purpose: Targeted exam revision based on recent mock exam and practice quiz attempts.

## Main Pattern

Your scenario reasoning is generally strong. Most lost marks come from using a sensible general answer when the question asks for a formal course category.

When answering, first identify what type of thing the question is asking for:

| If the question asks for... | Answer with... | Examples |
| --- | --- | --- |
| Context analysis technique | A framework or tool for understanding context | SWOT, PEST, Five Forces, stakeholder analysis, trend analysis |
| BA activity | Work the BA performs | current state analysis, patient/customer feedback collection, technology assessment, regulatory analysis, cost-benefit analysis |
| Elicitation technique | How information is gathered | interviews, surveys, workshops, observation, document analysis |

Exam-safe pattern:

> The BA should perform current state analysis to understand the existing process. Useful elicitation techniques include interviews, observation, and document analysis.

## Need, Requirement, Solution, Constraint

Keep these four separate.

| Term | Meaning | Example |
| --- | --- | --- |
| Business need | Why change is required | Slow support response and lack of centralised information |
| Business requirement | What must be achieved at a high level | Improve support services and customer experience |
| Solution | How the requirement might be delivered | Mobile app, EHR system, telehealth platform |
| Constraint | A limit on the work | Launch next year, prepare plan within one month |

Exam-safe wording:

> The deadline should be treated as a project constraint, not as a reason to skip current state analysis.

## Requirements Questions

You usually identify the right feature or quality, but sometimes write requirements that are too broad or bundled.

Weak:

> The app should let users apply, upload documents, pay, track status, and receive decisions.

Stronger:

> The system must allow applicants to upload required supporting documents as part of an online permit application.

Good requirements should be:

- Atomic.
- Unambiguous.
- Testable.
- Feasible.
- Understandable.
- Complete enough for the next stage of work.

For non-functional requirements, avoid vague quality labels.

Weak:

> The system should be private.

Stronger:

> The system must protect applicant personal information through appropriate access controls and secure storage to support privacy and compliance.

Related notes:

- [[Digital Business Analysis (ISYS90049)/Week 07/Lecture|Week 07 - Requirements Life Cycle Management]]
- [[Digital Business Analysis (ISYS90049)/Week 10/Lecture|Week 10 - Requirements Analysis and Design Definition]]

## Measures, Metrics, and KPIs

You often choose activity-based KPIs when the question wants business outcomes.

| Term | Meaning | Example |
| --- | --- | --- |
| Measure | Raw count or value | Number of referred customers |
| Metric | Derived value, rate, or average | Referral conversion rate |
| KPI | Strategic metric linked to a business goal | Customer lifetime value, churn rate, course completion rate |

Avoid KPIs that only show activity:

- Number of clicks.
- Number of logins.
- Number of breakout messages.
- Number of feedback comments.

Prefer KPIs that show value:

- Revenue from referred customers.
- Customer lifetime value.
- Customer churn rate.
- Course completion rate.
- Customer satisfaction score.
- Average order value.

Related note:

- [[Digital Business Analysis (ISYS90049)/Week 11/Lecture|Week 11 - Solution Evaluation]]

## Solution Evaluation Tasks

Memorise these five tasks:

1. Measure solution performance.
2. Analyse performance measures.
3. Assess solution limitations.
4. Assess enterprise limitations.
5. Recommend actions to increase solution value.

Common weak spot: choosing "recommend actions" too early without first explaining the evidence or limitation.

Exam-safe pattern:

> The BA should assess solution limitations by checking whether the system itself is causing the value gap, such as inaccurate ETA calculations or missing priority rules. Evidence could include system logs, performance data, user complaints, and variance between expected and actual outcomes.

Use assess enterprise limitations when the issue may involve people, process, adoption, culture, policy, training, readiness, resistance, or trust.

## Benchmarking

Do not confuse an internal baseline comparison with industry benchmarking.

| Benchmarking type | Meaning |
| --- | --- |
| Internal benchmarking | Compare against the organisation's own past performance or another internal unit |
| Competitive benchmarking | Compare against competitors |
| Collaborative benchmarking | Share data with industry peers |
| Shadow benchmarking | Use public competitor or industry data |

For a question asking for benchmarking within an industry, use competitive, collaborative, or shadow benchmarking.

Good KPIs to benchmark:

- Customer lifetime value.
- Churn rate.
- Referral conversion rate.
- Average order value.

Exam-safe wording:

> Competitive or shadow benchmarking would let the organisation compare referral-driven growth against food delivery competitors or publicly available industry data, rather than only comparing the solution to its own past baseline.

## Prioritisation

Mention Pareto analysis, but add decision criteria.

Exam-safe wording:

> The BA should prioritise issues using Pareto analysis and business impact criteria, including frequency, cost, urgency, effect on KPIs, customer impact, operational risk, and strategic alignment.

## Last-Minute Checklist

Before writing each answer, ask:

1. Is this asking for a technique, activity, or elicitation method?
2. Have I separated need, requirement, solution, and constraint?
3. Are my requirements atomic and testable?
4. Does my KPI show business value rather than only activity?
5. For solution evaluation, have I included the task, evidence, and value?
