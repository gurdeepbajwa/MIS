# Lecture

Course: [[Digital Business Analysis (ISYS90049)/Course Overview|Digital Business Analysis (ISYS90049)]]
Week: 07
Topic: Requirements Life Cycle Management

## Topic

Requirements Life Cycle Management

## Key Concepts

### Needs and Requirements

A requirement is a usable representation of a need. Requirements help describe what value could be delivered if the requirement is fulfilled.

The distinction between business needs and business requirements is not always sharp:

| Concept | Focus |
| --- | --- |
| Business need | Why something is needed, usually because of a problem or opportunity. |
| Business requirement | A high-level statement of how the need could be addressed. |

Example pattern:

| Need | High-level business requirement |
| --- | --- |
| Reduce IT costs. | Merge IT systems. |
| Increase process efficiency. | Replace manual activities. |
| Improve customer satisfaction. | Improve customer service and support. |

### Requirements and Design Cycle

Requirements and designs evolve together. Business analysts consider:

- What is needed to address the problem.
- What stakeholders need to do their jobs.
- What the solution needs to be.
- What is needed to transition the business to use the solution.

### Types of Requirements

| Requirement type | Meaning |
| --- | --- |
| Business requirements | Goals, objectives, and outcomes that explain why a change has been initiated at the business level. |
| Stakeholder requirements | Needs of stakeholders that must be met to achieve the business requirements. |
| Solution requirements | Capabilities and qualities of a solution that meet stakeholder requirements. |
| Transition requirements | Temporary requirements needed to move from the current state to operational use of the solution. |

### Functional and Non-Functional Requirements

Solution requirements can be functional or non-functional:

| Type | Focus |
| --- | --- |
| Functional requirements | What the solution or system should do, including behaviours, functions, and services. |
| Non-functional requirements | Conditions and qualities the solution must satisfy, such as usability, performance, reliability, availability, recovery, privacy, compliance, or sustainability. |

### Attributes of a Good Requirement

| Attribute | Meaning |
| --- | --- |
| Atomic | Self-contained and understandable independently. |
| Complete | Detailed enough to guide further work at the right level of detail. |
| Consistent | Aligned with stakeholder needs and not conflicting with other requirements. |
| Concise | Contains no unnecessary content. |
| Unambiguous | Clear enough to determine whether the solution meets the need. |
| Understandable | Uses terminology suitable for the intended audience. |
| Feasible | Possible within agreed risk, schedule, and budget. |
| Testable | Can be verified once implemented. |

### Requirements Life Cycle Management

Requirements Life Cycle Management manages requirements and designs from inception to retirement.

It aims to:

- Maintain relationships between related requirements and designs.
- Keep business, stakeholder, solution, and transition requirements aligned.
- Support impact analysis when change occurs.
- Prioritise requirements based on value, risk, sequence, or constraints.
- Ensure requirements are approved and maintained for possible reuse.

Requirements lifecycle management is a supporting and recurring area of business analysis. Requirements exist across planning, elicitation, analysis, design, delivery, and evaluation, so the analyst revisits lifecycle management throughout the initiative rather than treating it as a single phase.

The lecture uses the acronym TMPAA:

| Task | Purpose |
| --- | --- |
| Trace requirements | Ensure requirements are aligned with each other and with higher-level needs. |
| Maintain requirements | Keep requirements accurate, consistent, accessible, and reusable. |
| Prioritise requirements | Rank requirements by relative importance, value, sequence, or necessity. |
| Assess requirement changes | Evaluate impacts and implications of proposed changes. |
| Approve requirements | Reach agreement and approval with key stakeholders. |

TMPAA is flexible. Not every cycle of analysis requires every task with the same level of formality. Traceability and approval are usually important, while prioritisation may be lighter when the change is small or priorities are already stable.

### Trace Requirements

Traceability links requirements across levels, such as:

Business needs -> business requirements -> stakeholder requirements -> solution requirements -> functional, non-functional, and transition requirements.

Traceability enables:

- Faster impact analysis.
- Identification of inconsistencies and gaps.
- Better understanding of scope and complexity.
- Assessment of which requirements have or have not been addressed.

Common relationships between requirements:

| Relationship | Meaning |
| --- | --- |
| Derive | One requirement is derived from another. |
| Depend | One requirement is only meaningful, or easier to implement, if another requirement is implemented. |
| Validate | A requirement is linked to an element, such as a test case, that verifies success. |

### Maintain Requirements

Maintaining requirements ensures they remain accurate and consistent.

Requirements should:

- Use a consistent format and wording.
- Follow a standard review and approval process.
- Be accessible and understandable.
- Be checked against approved requirements before new requirements are accepted.
- Support reuse in the current initiative or similar future initiatives.

### Prioritise Requirements

Prioritisation ranks requirements by relative importance. Priorities may change as context changes.

Possible prioritisation bases:

- Cost, effort, and resources.
- Expected benefits or value.
- Risk that value will not be delivered.
- Dependencies between requirements.
- Penalty or negative consequence of not implementing.
- Regulatory obligation.
- Time sensitivity.
- Stability or likelihood of change.

Stakeholders often need to make trade-offs. Prioritisation should distinguish between what is needed, wanted, and merely liked.

MoSCoW is one prioritisation method:

| Priority | Meaning |
| --- | --- |
| Must | Required. |
| Should | High priority. |
| Could | Desirable but not necessary. |
| Won't | Not included now, but may be considered later. |

### Assess Requirement Changes

Assessing changes means evaluating the impact of proposed changes to requirements or designs.

Assessment should consider:

- Alignment with overall strategy.
- Impact on business or stakeholder value.
- Impact on delivery time or resource requirements.
- Changes to risks, opportunities, or constraints.
- What needs to be documented and communicated to stakeholders.

The formality of assessment depends on the governance process and the significance of the proposed change.

Digital tools, including AI-enabled work management platforms, may assist with tracing, maintaining, prioritising, and assessing requirements by finding links, suggesting updates, or summarising impacts. Human judgement remains necessary for approval, stakeholder agreement, value trade-offs, and risk-sensitive decisions.

### Approve Requirements

Approval establishes agreement on new or changed requirements.

Approval should:

- Resolve conflicts and open issues.
- Follow the business analysis governance process.
- Communicate requirements clearly to approving stakeholders.
- Be formal or informal depending on the chosen approach.
- Communicate outcomes to affected stakeholders.
- Be tracked and managed.

### Textbook Connections

- Milani Chapter 15 connects requirements lifecycle management to solution design.
- Milani explains that requirements are elicited, analysed, refined, captured, prioritised, approved, maintained, and changed over time.
- The lecture's requirement types align with Milani's distinction between business, stakeholder, functional, non-functional, data, and transition requirements.
- Milani emphasises that requirements should collectively deliver the desired value, not merely document stakeholder requests.
- The lecture's quality attributes align with Milani's verification and validation focus: requirements should be usable, understandable, complete, consistent, traceable, and connected to business value.

## Summary

- Requirements are usable representations of needs and should focus on value to be delivered.
- Requirements can be business, stakeholder, solution, or transition requirements.
- Solution requirements include functional requirements and non-functional quality conditions.
- Good requirements are atomic, complete, consistent, concise, unambiguous, understandable, feasible, and testable.
- Requirements Life Cycle Management manages requirements from inception to retirement through trace, maintain, prioritise, assess, and approve tasks.
- Strong lifecycle management keeps requirements aligned with business value and makes change easier to assess.

## Notes

Reading: Milani Chapter 15.

References:

- IIBA. (2015). _A guide to the Business Analysis Body of Knowledge_ (3rd ed.).
- Milani, F. (2019). _Digital business analysis_. Springer. https://doi.org/10.1007/978-3-030-05719-0
