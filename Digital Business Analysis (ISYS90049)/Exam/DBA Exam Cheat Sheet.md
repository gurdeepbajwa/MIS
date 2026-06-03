# DBA Exam Cheat Sheet

Course: [[Digital Business Analysis (ISYS90049)/Course Overview|Digital Business Analysis]]  
Use: pre-exam revision only. The exam is closed book.

## Exam Shape

The DBA exam is a 2-hour closed-book written exam. The sample material points to four 25-mark sections:

| Section | Main skill tested |
| --- | --- |
| Planning | Plan the BA work, identify needs, risks, context, stakeholders, elicitation, governance, and scope. |
| Strategy analysis | Analyse current state, root causes, future state, constraints, gaps, and change strategy. |
| Requirements analysis and design | Classify, write, model, verify, validate, and justify requirements and design options. |
| Solution evaluation | Choose measures, metrics, KPIs, evaluation tasks, limitations, benchmarking, and value-improvement actions. |

## Core Answer Formula

Use this for most written answers:

1. Identify the business need or analysis problem.
2. Name the relevant BA concept, task, model, or technique.
3. Define it briefly.
4. Apply it to the case facts.
5. State the BA output produced.
6. Explain how it improves value, decision quality, stakeholder alignment, or risk reduction.

Strong answers use the case, not generic definitions.

## Section 1 - Planning

### Planning Tasks

| Task | What it does |
| --- | --- |
| Plan BA approach | Defines BA activities, methods, tools, timing, and deliverables. |
| Plan stakeholder engagement | Identifies stakeholders and how the BA will communicate, collaborate, and manage involvement. |
| Plan BA governance | Clarifies decision rights, approvals, change control, and prioritisation. |
| Plan BA information management | Defines how BA information is documented, stored, shared, accessed, and retained. |
| Identify BA performance improvements | Measures and improves the BA work itself. |

### Planning Aspects to Mention

Background, context, scope, approach, activities, complexity and risk, approval, time, cost, resources, governance, stakeholder access, information management.

### BA Planning Risks

Planning risks are risks to the analysis work, not just the final solution.

| Risk | Consequence | Mitigation |
| --- | --- | --- |
| Poor stakeholder access | Incomplete or biased requirements. | Secure sponsor support, schedule early interviews, use workshops or surveys where access is limited. |
| Unclear scope | Scope creep and conflicting expectations. | Define in-scope and out-of-scope areas, use POPIT, confirm with decision makers. |
| Time pressure | Shallow analysis and premature solution design. | Prioritise high-risk areas, use targeted elicitation, plan review points. |
| Weak governance | Slow or contested decisions. | Define approval roles, escalation paths, and change control. |
| Low domain knowledge | Misinterpretation of business need. | Use domain experts, document analysis, and validation sessions. |

### Context and Scope Tools

| Tool | Best use |
| --- | --- |
| PEST or PESTLE | External political, economic, social, technological, legal, and environmental influences. |
| Porter's Five Forces | Industry and competitive pressure. |
| SWOT | Internal strengths/weaknesses plus external opportunities/threats. |
| POPIT | Scope change across people, organisation, process, information, and technology. |
| Stakeholder matrix | Influence and impact: key players, keep satisfied, keep informed, monitor. |

### Planning Traps

- Jumping straight to a system or solution.
- Treating stakeholder engagement as a contact list rather than a plan.
- Confusing BA work risks with solution risks.
- Listing techniques without explaining why they fit the case.
- Ignoring governance, approval, and information management.

## Section 2 - Strategy Analysis

### Need, Requirement, Goal, Objective

| Concept | Meaning |
| --- | --- |
| Business need | The problem or opportunity explaining why change may be required. |
| Business requirement | High-level outcome or condition needed to address the business need. |
| Business goal | Qualitative statement of what the business wants to achieve. |
| Business objective | Measurable target supporting the goal. Should be SMART. |

Flow: business need -> business requirement -> business goal -> SMART objective.

### Current State

Current state analysis explains how the organisation currently operates in relation to the need. It should be focused, evidence-based, and relevant to the case.

Use POPIT:

- People: skills, capacity, culture, workload, stakeholder expectations.
- Organisation: structure, roles, responsibilities, strategy, governance.
- Process: workflows, handoffs, manual work, bottlenecks.
- Information and Technology: systems, data, integrations, tools, infrastructure.

### Problem and Root Cause Analysis

| Concept | Meaning |
| --- | --- |
| Symptom | Observable effect of the problem. |
| Cause | Reason the problem exists. |
| Root cause | Deeper cause that prevents recurrence if addressed. |

| Technique | Best use |
| --- | --- |
| Five-Why method | Probe causal chains; needs evidence and right stakeholders. |
| Fishbone diagram | Organise multiple possible causes across categories. |
| Pareto analysis | Prioritise the few causes creating most impact. |
| Process model | Show workflow, handoffs, delays, rework, and bottlenecks. |
| Customer journey map | Show user experience, touchpoints, emotions, pain points, and opportunities. |

### Future State and Change Strategy

Future state describes the desired "what", not the detailed "how". It defines success, value, outcomes, solution space, and required organisational conditions before selecting a specific solution.

| Concept | Meaning |
| --- | --- |
| Solution scope | What needs to change. |
| Solution | How those changes will be made. |
| Constraint | Budget, time, technology, resource, policy, or regulation limit. |
| Gap analysis | Compares current and future state to identify required changes. |
| Change strategy | High-level approach for moving from current state to future state. |

Implementation approaches:

- Single-stage implementation: suitable for small or tightly coupled changes.
- Gradual or phased implementation: useful when change is large, risky, or disruptive.
- Incremental implementation: delivers capability in useful parts.
- Iterative implementation: refines the solution through feedback and learning.

### Strategy Analysis Traps

- Accepting a manager's preferred solution without testing the underlying need.
- Describing current state as general background instead of case-relevant evidence.
- Defining future state with too much solution detail too early.
- Forgetting constraints, readiness, transition, or change risk.
- Treating symptoms as root causes.

## Section 3 - Requirements Analysis and Design

### Requirement Types

| Type | Meaning |
| --- | --- |
| Business requirements | Goals, objectives, and outcomes explaining why change has been initiated. |
| Stakeholder requirements | Stakeholder needs that must be met to achieve business requirements. |
| Solution requirements | Capabilities and qualities of a solution that meet stakeholder requirements. |
| Functional requirements | What the solution must do. |
| Non-functional requirements | How well or under what conditions the solution must operate. |
| Transition requirements | Temporary capabilities or conditions needed to move from current to future state. |

### Functional vs Non-Functional

Functional: system behaviour, feature, service, or action.  
Non-functional: usability, performance, reliability, availability, security, privacy, compliance, recovery, scalability, or sustainability.

Example:

- Functional: The app must allow members to book available classes.
- Non-functional: The app must show available classes within two seconds during peak booking periods.

### Good Requirement Attributes

Atomic, complete, consistent, concise, feasible, unambiguous, testable, prioritised, understandable.

Avoid vague words such as easy, fast, user-friendly, robust, and seamless unless they are converted into measurable criteria.

### Verification vs Validation

| Concept | Question answered |
| --- | --- |
| Verification | Is the requirement written and modelled well? |
| Validation | Is it the right requirement for the business need, goals, scope, and stakeholders? |

A verified requirement may still fail validation if it is clear and testable but does not support the real business need.

### Requirements Lifecycle

TMPAA:

- Trace requirements.
- Maintain requirements.
- Prioritise requirements.
- Assess requirement changes.
- Approve requirements.

Traceability chain:

Business need -> business requirement -> stakeholder requirement -> solution requirement -> functional/non-functional/transition requirement.

### Models and Design Tools

| Tool | Use |
| --- | --- |
| Process model or BPMN | Show activity flow, decisions, handoffs, and process logic. |
| Matrix | Compare requirements, stakeholders, priority, value, or traceability. |
| Wireframe | Low-fidelity interface structure for early discussion. |
| Prototype | Representation of solution behaviour or design at low, medium, or high fidelity. |
| Use case | Actor-system interaction scenario. |

Use case elements: actor, trigger, pre-condition, post-condition, normal flow, alternative flow.

Use case relationships:

- Include: required interaction reused by another use case.
- Extend: optional or conditional interaction added under certain conditions.

### Requirements Traps

- Confusing business objectives with system requirements.
- Writing non-functional requirements as vague quality words without measurable criteria.
- Treating verification and validation as the same.
- Choosing one model for every audience.
- Forgetting transition requirements such as migration, training, support, or rollout readiness.

## Section 4 - Solution Evaluation

### Evaluation Purpose

Solution evaluation checks whether an implemented or active solution delivers intended business value. It is not just a project delivery review.

### Evaluation Tasks

| Task | Purpose |
| --- | --- |
| Measure solution performance | Define and collect relevant performance measures. |
| Analyse performance measures | Compare actual performance with expected value. |
| Assess solution limitations | Identify internal solution factors blocking value. |
| Assess enterprise limitations | Identify organisational factors blocking value. |
| Recommend actions to increase value | Close the gap between potential and actual value. |

### Measure, Metric, KPI

| Concept | Meaning | Example |
| --- | --- | --- |
| Measure | Direct count or value. | Number of support tickets. |
| Metric | Derived or interpreted value. | Average response time; churn rate. |
| KPI | Key metric tied to strategic objective. | Customer retention rate if retention is the goal. |

Relationship:

Goals and objectives -> critical success factors -> KPIs -> metrics -> measures.

### Good Metrics

Good metrics should be clear, relevant, economical, adequate, quantifiable, trustworthy, and credible.

Do not choose metrics only because data is easy to collect. Choose metrics because they show progress toward the business objective.

### Solution vs Enterprise Limitations

| Limitation type | Meaning | Example |
| --- | --- | --- |
| Solution limitation | Internal problem inside the solution. | Missing feature, poor usability, weak integration, incorrect data, slow performance. |
| Enterprise limitation | Organisational problem outside the solution. | Poor training, resistance, weak process, policy conflict, lack of operational readiness. |

### Benchmarking and A/B Testing

Benchmarking compares performance to internal units, competitors, peers, public data, functional equivalents, or world-class performers.

A/B testing compares two variants of a solution element against a metric. It needs enough data volume to avoid misleading results.

### Evaluation Traps

- Choosing vanity metrics that do not link to business goals.
- Confusing measures, metrics, and KPIs.
- Treating early low adoption as automatic solution failure.
- Ignoring enterprise limitations when the system itself works.
- Recommending technical changes when training, process, or governance is the real issue.

## High-Yield Distinctions

| Distinction | How to remember it |
| --- | --- |
| Business need vs business requirement | Need = why change is required; requirement = high-level outcome or condition needed. |
| Business requirement vs solution requirement | Business requirement stays closer to business outcomes; solution requirement describes capabilities or qualities of the solution. |
| Current state vs future state | Current = what is happening now; future = what should exist after change. |
| Solution scope vs solution | Scope = what must change; solution = how it will change. |
| Verification vs validation | Verification = written well; validation = right for the need. |
| Functional vs non-functional | Functional = what it does; non-functional = how well it works. |
| Measure vs metric vs KPI | Measure = raw value; metric = interpreted value; KPI = key metric tied to strategic objective. |
| Solution limitation vs enterprise limitation | Solution = inside the solution; enterprise = organisation around the solution. |

## Quick Templates

### Planning Risk Paragraph

One BA planning risk is [risk]. In the case, this matters because [case fact]. If unmanaged, it may cause [consequence]. The BA should mitigate it by [action], so that [analysis output or value].

### Technique Choice Paragraph

[Technique] is suitable because the case involves [problem/context]. It helps the BA [what the technique reveals]. The output would be [model/table/description], which supports [decision, requirement, scope, or value].

### Root Cause Paragraph

The visible symptom is [symptom], but the BA should not assume it is the root cause. Using [technique], the BA can test whether [possible cause] is supported by [evidence]. This prevents recommending a solution that treats symptoms rather than the underlying problem.

### Requirement Paragraph

A [functional/non-functional/transition] requirement is: [requirement]. This is a good requirement because it is [quality attributes] and links to [business need or stakeholder need]. It should be verified for quality and validated against [goal, objective, solution scope, or stakeholder value].

### Evaluation KPI Paragraph

A suitable KPI is [KPI]. It links to the business goal of [goal] because it shows [value]. It should be measured [frequency] using [data source]. The BA should compare actual performance with [target/benchmark] and investigate [solution or enterprise limitations] if performance is below expectation.

## Last-Minute Memory List

- Always state the business need before the solution.
- Use POPIT when the case is broader than technology.
- Say why a technique fits the case.
- Distinguish symptoms, causes, and root causes.
- Keep future state at the outcome level before detailed design.
- Make requirements testable and unambiguous.
- Verification and validation are not the same.
- KPIs must link to business goals.
- Evaluation focuses on value, not only project completion.

## Source Notes

- [[11-Hour Exam Study Prep]]
- [[../Week 01/Lecture|Week 01 Lecture]]
- [[../Week 02/Lecture|Week 02 Lecture]]
- [[../Week 03/Lecture|Week 03 Lecture]]
- [[../Week 04/Lecture|Week 04 Lecture]]
- [[../Week 05/Lecture|Week 05 Lecture]]
- [[../Week 07/Lecture|Week 07 Lecture]]
- [[../Week 08/Lecture|Week 08 Lecture]]
- [[../Week 09/Lecture|Week 09 Lecture]]
- [[../Week 10/Lecture|Week 10 Lecture]]
- [[../Week 11/Lecture|Week 11 Lecture]]
