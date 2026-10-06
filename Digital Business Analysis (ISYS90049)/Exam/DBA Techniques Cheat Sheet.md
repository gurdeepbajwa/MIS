# DBA Techniques Cheat Sheet

Course: [[Digital Business Analysis (ISYS90049)/Course Overview|Digital Business Analysis]]  
Use: quick technique selection and exam revision. Covers the techniques and frameworks appearing in the DBA weekly notes and exam material.

## How to Use This Sheet

In an exam answer, do not only name a technique. Use this pattern:

1. Name the technique.
2. Define what it does.
3. Explain why it fits the case facts.
4. State the output it produces.
5. Link the output to value, risk reduction, stakeholder alignment, decision quality, or requirements quality.

## Fast Selection Guide

| If the question asks you to... | Use these first |
| --- | --- |
| Frame the BA work | BACCO, BA plan, predictive/adaptive/hybrid approach, governance, information management, BA performance measures |
| Understand external context | PEST/PESTLE, Porter's Five Forces, industry trends |
| Understand internal context | Strategy analysis, business model analysis, capability analysis, SWOT, POPIT |
| Define scope | Scope definition, POPIT, stakeholder analysis, solution scope |
| Identify and manage stakeholders | Stakeholder identification, onion diagram, attitude analysis, influence-impact matrix, stakeholder management plan |
| Gather information | Document analysis, interview, survey, observation, workshop, focus group |
| Diagnose a problem | Problem statement, root cause analysis, Five Whys, fishbone diagram, Pareto analysis, process model, data triangulation |
| Manage requirements over time | Trace, maintain, prioritise, assess changes, approve requirements; MoSCoW |
| Analyse current and future state | Current state analysis, POPIT, personas, customer journey maps, future state analysis, SMART objectives |
| Plan the change | Gap analysis, readiness assessment, risk assessment, transition planning, implementation approach |
| Specify solution detail | Requirements classification, matrices, BPMN/process models, wireframes, prototypes, use cases, requirements architecture |
| Compare solution options | Design options, cost-benefit/value comparison, feasibility/risk/alignment assessment |
| Evaluate a live solution | Measures, metrics, KPIs, performance analysis, limitation assessment, A/B testing, benchmarking, continuous monitoring |

## Foundations

| Technique or framework | Use | Output | Watch for |
| --- | --- | --- | --- |
| BACCO/BACCM | Frame change by checking need, solution, stakeholder, value, context, and change. | Shared language for the analysis problem. | Do not treat it as a process sequence; it is a concept model. |
| BABOK knowledge areas | Organise BA work across planning, elicitation, lifecycle management, strategy, requirements/design, and evaluation. | Broad map of BA responsibilities. | Do not imply the areas must happen in a strict waterfall order. |
| Predictive approach | Plan formally when problem, scope, solution direction, and timing are relatively clear. | Phase-based BA approach and deliverables. | Avoid using it where uncertainty requires learning. |
| Adaptive approach | Analyse iteratively when the solution is uncertain or feedback is needed. | Iterative requirements, learning, and refinement. | Adaptive does not mean analysis stops. |
| Hybrid approach | Combine formal governance with iterative discovery or delivery. | Mixed BA plan suited to large organisations. | Explain which parts are formal and which parts iterate. |

Source: [[Digital Business Analysis (ISYS90049)/Week 01/Lecture|Week 01]], [[Digital Business Analysis (ISYS90049)/Week 02/Lecture|Week 02]], [[Digital Business Analysis (ISYS90049)/Week 06/Lecture|Week 06]]

## Planning and Monitoring

| Technique or task | Use | Output | Exam trap |
| --- | --- | --- | --- |
| BA plan | Define background, context, scope, approach, activities, complexity, risk, approval, resources, and timing. | Business analysis plan. | Do not write a project delivery plan only. |
| Plan stakeholder engagement | Decide who to involve, why, when, and how. | Engagement and communication approach. | Do not reduce it to a contact list. |
| Plan BA governance | Clarify decision rights, approvals, prioritisation, and change control. | Governance approach. | Mention who approves changes and how conflicts escalate. |
| Plan information management | Decide how BA information is captured, stored, shared, accessed, and retained. | Information management approach. | Include privacy, sensitive information, and access rights when relevant. |
| BA performance improvement | Measure and improve the analysis work itself. | BA performance measures and improvement actions. | Do not confuse this with solution evaluation. |
| Complexity and risk assessment | Identify conditions that make the BA work harder or riskier. | BA risks and treatments. | Planning risks affect analysis quality, not only final implementation. |
| Prioritisation approach | Define how BA work, changes, or requirements will be ranked. | Decision criteria and priority process. | Tie priority to value, risk, constraints, dependencies, or regulation. |

Source: [[Digital Business Analysis (ISYS90049)/Week 02/Lecture|Week 02]]

## Context Analysis

| Technique | Best for | Output | Exam trap |
| --- | --- | --- | --- |
| PEST | Broad external forces: political, economic, social, technological. | External context factors affecting the need or solution. | Do not list generic trends; connect each to the case. |
| PESTLE | PEST plus legal and environmental factors. | Wider external risk/opportunity scan. | Use legal/environmental only when relevant. |
| Porter's Five Forces | Industry competition and market pressure. | Competitive pressure analysis. | This is industry-level, not internal process analysis. |
| Porter's generic strategies | Position the organisation by cost/differentiation and broad/focused market scope. | Strategic positioning view. | Use only when strategy or competitive positioning matters. |
| Business model analysis | Understand how the organisation creates, delivers, and captures value. | Business model implications for change. | Do not treat it as a list of departments. |
| Capability analysis | Identify what the organisation can or must be able to do. | Capability gaps or strengths. | A digital solution fails if required capabilities are missing. |
| SWOT | Combine internal strengths/weaknesses with external opportunities/threats. | Context summary for needs, options, and barriers. | Keep internal and external factors separate. |
| POPIT | Analyse people, organisation, process, information, and technology together. | Holistic scope/current-state/future-state view. | Do not make every problem a technology problem. |

Source: [[Digital Business Analysis (ISYS90049)/Week 03/Lecture|Week 03]], [[Digital Business Analysis (ISYS90049)/Week 04/Lecture|Week 04]], [[Digital Business Analysis (ISYS90049)/Week 08/Lecture|Week 08]], [[Digital Business Analysis (ISYS90049)/Week 09/Lecture|Week 09]]

## Scope, Stakeholders, and Elicitation

| Technique | Best for | Output | Exam trap |
| --- | --- | --- | --- |
| Scope definition | Clarify solution, product, project, or BA work boundaries. | In-scope and out-of-scope statement. | Separate BA work scope from solution scope. |
| Stakeholder identification | Find people/groups affected by, interested in, or needed for the change. | Stakeholder list. | Include knowledge holders, users, decision makers, regulators, support, and delivery roles where relevant. |
| Stakeholder onion diagram | Show closeness to the initiative. | Involvement map. | Closeness is not the same as authority. |
| Stakeholder attitude analysis | Understand support, neutrality, or opposition. | Engagement risk view. | Explain likely reason for attitude, such as workload, status, risk, or incentives. |
| Influence-impact matrix | Decide how closely each stakeholder should be managed. | Key players, keep satisfied, keep informed, monitor. | Do not confuse high impact with high influence. |
| Stakeholder management plan | Define why, what, when, how, and where communication occurs. | Engagement plan. | Strong plans adapt by stakeholder group. |
| Document analysis | Review existing documents, reports, policies, models, data, or instructions. | Existing evidence, gaps, conflicts, assumptions. | Check relevance and conflicts; documents may be outdated. |
| Interview | Elicit deep qualitative insight from one or a small number of stakeholders. | Rich stakeholder perspective and assumptions. | Avoid leading questions and unsupported opinions. |
| Survey | Collect structured input from many people. | Broad quantitative or standardised feedback. | Low depth and response bias are risks. |
| Observation | Study work as it is actually performed. | Evidence of real process, workarounds, delays, or behaviours. | People may behave differently when watched. |
| Workshop | Bring stakeholders together to elicit, model, validate, prioritise, or decide. | Shared understanding, models, decisions, or validated outputs. | Workshops need preparation and facilitation; do not use them for sensitive issues too early. |
| Focus group | Gather feedback from a selected group with relevant experience. | Group feedback on needs, issues, concepts, or reactions. | Dominant voices can distort results. |

Source: [[Digital Business Analysis (ISYS90049)/Week 04/Lecture|Week 04]]

## Problem Analysis

| Technique | Best for | Output | Exam trap |
| --- | --- | --- | --- |
| Problem definition | Clarify current situation, problem, stakeholders, impacts, and challenges. | Clear analysis focus. | Do not accept a requested solution as the problem. |
| Problem statement | State the problem, affected stakeholders, and business impact. | Concise problem statement. | A vague statement weakens every later technique. |
| Root cause analysis | Investigate why the problem exists. | Causes and stronger explanation of the business need. | Needs evidence, not only opinions. |
| Five Whys | Probe a narrow causal chain from symptom to deeper cause. | Possible cause chain. | Can oversimplify complex, multi-cause problems. |
| Fishbone diagram | Organise many possible causes into categories. | Cause-and-effect map. | Does not prioritise causes by itself. |
| 6M categories | Structure fishbone causes: machine, method, material, man, measurement, milieu. | Cause categories. | Use only where the categories fit the context. |
| Pareto analysis | Rank causes by frequency, impact, or contribution. | Vital-few cause ranking. | Requires cause data; frequency is not always business importance. |
| Process model | Show workflow, handoffs, decisions, bottlenecks, delays, and rework. | Process view of the problem. | A process model is evidence for analysis, not automatically the solution. |
| Triangulation | Compare interviews, workshops, documents, observation, and data. | Validated problem evidence. | One stakeholder view is not enough for a strong root-cause claim. |

Common sequence: define problem -> gather evidence -> identify possible causes -> organise causes -> prioritise causes -> propose corrective actions or further analysis.

Source: [[Digital Business Analysis (ISYS90049)/Week 05/Lecture|Week 05]], [[Digital Business Analysis (ISYS90049)/Week 05/Root Cause Analysis Techniques Reference|Root Cause Analysis Techniques Reference]]

## Requirements Lifecycle Management

| Technique or task | Use | Output | Exam trap |
| --- | --- | --- | --- |
| Requirements classification | Separate business, stakeholder, solution, functional, non-functional, and transition requirements. | Clear requirement types. | Do not confuse business objectives with system requirements. |
| Trace requirements | Link needs to requirements, designs, tests, and changes. | Traceability chain. | Use traceability to explain impact analysis and gap detection. |
| Maintain requirements | Keep requirements accurate, accessible, consistent, and reusable. | Maintained requirement set. | Maintenance is ongoing, not clerical filing. |
| Prioritise requirements | Rank requirements by value, risk, dependency, regulation, cost, or time sensitivity. | Priority order. | Explain trade-offs, not only labels. |
| MoSCoW | Classify requirements as must, should, could, or will not for now. | Practical priority categories. | "Must" should mean genuinely required, not merely desired. |
| Assess requirement changes | Evaluate impacts of proposed changes. | Change impact assessment. | Include strategy, value, time, resources, risks, constraints, and communication. |
| Approve requirements | Gain stakeholder agreement according to governance. | Approved requirement baseline or decision record. | Approval should resolve conflicts and communicate outcomes. |

Traceability chain: business need -> business requirement -> stakeholder requirement -> solution requirement -> functional/non-functional/transition requirement.

Source: [[Digital Business Analysis (ISYS90049)/Week 07/Lecture|Week 07]], [[Digital Business Analysis (ISYS90049)/Week 10/Lecture|Week 10]]

## Current and Future State Strategy Analysis

| Technique | Best for | Output | Exam trap |
| --- | --- | --- | --- |
| Current state analysis | Explain how the organisation currently operates in relation to the need. | Focused current state description. | Do not write general company history. |
| Business need/source analysis | Identify why change is needed and whether it is top-down, bottom-up, middle management, or external. | Need origin and evidence focus. | Source shapes stakeholders and evidence needed. |
| Personas | Represent research-based customer or user segments. | Persona profile for analysis and design. | Personas are not decorative biographies; they guide priorities and needs. |
| Customer journey map | Show customer/user experience across phases and touchpoints. | Journey phases, actions, thoughts, feelings, pain points, opportunities. | Use the customer's perspective, not only internal process steps. |
| Future state analysis | Describe what the business should be like after change. | Desired outcomes, value, and future conditions. | Define the "what" before prematurely choosing the "how". |
| SMART objectives | Make goals specific, measurable, achievable, relevant, and time-bounded. | Measurable objectives. | A SMART objective is not the same as a system requirement. |
| Solution scope | Define what must change to reach the future state. | Solution boundary and included changes. | Solution scope is not the final solution design. |
| Constraints analysis | Identify budget, time, technology, resource, policy, and regulatory limits. | Explicit feasibility constraints. | Constraints shape trade-offs and option selection. |
| Gap analysis | Compare current and future states. | Gaps, examples, responsible units, actions, size estimates. | Gaps can cross POPIT areas. |
| Readiness assessment | Assess whether the organisation can adopt and sustain the change. | Readiness risks and preparation needs. | A good solution can fail if the enterprise is not ready. |
| Transition planning | Plan staged movement from current state to future state. | Transition states, releases, training, communication, support. | Include temporary requirements and adoption work. |
| Change strategy | Select a high-level approach for moving to the future state. | Change approach and rationale. | Explain why the approach fits size, risk, complexity, readiness, and value. |

Source: [[Digital Business Analysis (ISYS90049)/Week 08/Lecture|Week 08]], [[Digital Business Analysis (ISYS90049)/Week 09/Lecture|Week 09]], [[Digital Business Analysis (ISYS90049)/Week 09/How to Build a Future State and Gap Analysis|How to Build a Future State and Gap Analysis]]

## Implementation and Risk Techniques

| Technique | Best for | Output | Exam trap |
| --- | --- | --- | --- |
| Single-stage implementation | Deliver all key changes in one major release. | One-release transition approach. | Best for smaller or tightly coupled changes; riskier for large disruptive change. |
| Gradual implementation | Break a large change into stages or smaller projects. | Staged implementation path. | Explain how stages reduce disruption or risk. |
| Incremental implementation | Deliver useful capability in increments. | Progressive value delivery. | Each increment should add usable value or coverage. |
| Iterative implementation | Refine the solution through repeated feedback cycles. | Learning-based refinement. | Fits uncertainty; needs feedback and governance. |
| Risk assessment | Identify uncertainty affecting objectives, transition, or value realisation. | Risk register or risk analysis. | Include likelihood, impact, timing, warning signs, and tolerance. |
| Risk treatment | Decide avoid, transfer/share, mitigate, accept, or increase readiness. | Treatment actions. | Match treatment to the risk; do not only list generic mitigations. |

Source: [[Digital Business Analysis (ISYS90049)/Week 09/Lecture|Week 09]]

## Requirements Analysis and Design Definition

| Technique | Best for | Output | Exam trap |
| --- | --- | --- | --- |
| Specify and model requirements | Convert elicitation results into usable textual or visual representations. | Requirements, models, and design representations. | Choose representations for audience and information type. |
| Requirements quality check | Test requirements against atomic, complete, consistent, concise, feasible, unambiguous, testable, prioritised, and understandable. | Verified requirement quality. | Vague words like "fast" or "user-friendly" need measurable criteria. |
| Requirement verification | Check whether requirements are written and modelled correctly. | Requirement quality findings. | Verification asks "is it written well?" |
| Requirement validation | Check whether requirements are right for the business need, goals, scope, and stakeholders. | Alignment findings. | Validation asks "is it the right requirement?" |
| Requirements architecture | Organise views, model types, attributes, relationships, conflicts, dependencies, and completeness. | Coherent requirement structure. | This checks the set of requirements, not only individual statements. |
| Matrix | Compare structured information such as requirements, stakeholders, priority, value, or traceability. | Comparison or traceability table. | Good for structured data, weaker for complex flows. |
| BPMN/process model | Represent activity flow, decisions, handoffs, events, and process logic. | Process diagram/model. | Needs the right level of detail for the audience. |
| Organisational model | Show groups, roles, relationships, or reporting structures. | People/role view. | Useful when change affects responsibilities. |
| Decision model | Show decision logic or rationale. | Decision rules or decision structure. | Use when choices or business rules drive behaviour. |
| Functional decomposition | Break a capability or function into smaller parts. | Function hierarchy. | Do not lose the business purpose behind the breakdown. |
| Data model | Show data structures and relationships. | Data/information view. | Useful when data quality, ownership, or integration matters. |
| Interface model | Show information exchanged between systems, users, or components. | Interface requirements. | Important for integration-heavy digital solutions. |
| State model | Show states and transitions for an object or process. | State transition view. | Useful when lifecycle status matters. |
| Wireframe | Low-fidelity interface structure for discussion. | Screen layout concept. | Wireframes focus on structure, not branding or final visual design. |
| Prototype | Represent solution behaviour or design at low, medium, or high fidelity. | Testable or discussable design representation. | Higher fidelity can create false certainty and cost more to change. |
| Use case diagram | Show actors, system boundary, use cases, and relationships. | Visual actor-system interaction map. | Actors are direct interactors; stakeholders may be broader. |
| Use case narrative | Describe trigger, pre-condition, normal flow, alternative flow, and post-condition. | Step-by-step interaction scenario. | Include/extend relationships must be used correctly. |
| User story | Express a user-centred need in backlog-friendly language. | Short requirement statement for iterative delivery. | Not enough alone for complex rules, data, or process detail. |
| Design options | Compare possible ways to satisfy requirements and future state. | Viable solution options. | The analyst recommends; authorised stakeholders decide. |
| Potential value analysis | Compare expected benefits, costs, feasibility, risk, and alignment. | Recommended option rationale. | Benefits should relate to the original need, not unsupported revenue claims. |

Source: [[Digital Business Analysis (ISYS90049)/Week 10/Lecture|Week 10]]

## Solution Evaluation

| Technique or task | Use | Output | Exam trap |
| --- | --- | --- | --- |
| Measure solution performance | Define and collect data about solution effectiveness. | Performance measures. | Plan measures early; not all available data is useful. |
| Analyse performance measures | Compare actual performance with expected value. | Performance interpretation and variance analysis. | A value gap may reflect delayed adoption, not immediate failure. |
| Assess solution limitations | Identify internal solution factors limiting value. | Solution limitation findings. | Examples: missing feature, poor usability, weak integration, bad data, slow performance. |
| Assess enterprise limitations | Identify organisational factors outside the solution limiting value. | Enterprise limitation findings. | Examples: training gaps, resistance, poor process, weak readiness, policy conflict. |
| Recommend actions to increase value | Address causes of underperformance. | Recommended improvement, change, retirement, or no action. | Match action to the limitation, not to the symptom. |
| Continuous monitoring | Evaluate metrics over suitable intervals. | Trend view and ongoing improvement triggers. | Choose intervals deliberately; dashboards are not evaluation by themselves. |
| Measures | Direct counts or values. | Raw data points. | Example: number of support tickets. |
| Metrics | Derived or interpreted values. | Performance indicators. | Example: average response time or churn rate. |
| KPIs | Metrics tied to key business objectives. | Strategic performance indicators. | Not every metric is a KPI. |
| A/B testing | Compare two variants against a selected metric. | Evidence of which version performs better. | Needs enough usage volume to be reliable. |
| Benchmarking | Compare performance to internal units, competitors, peers, or leading performers. | Comparative performance gaps and improvement targets. | Public data may be incomplete or misleading. |

Measurement chain: goals and objectives -> critical success factors -> KPIs -> metrics -> measures.

Source: [[Digital Business Analysis (ISYS90049)/Week 11/Lecture|Week 11]]

## Technique Pairings That Score Well

| Pairing | Why it works |
| --- | --- |
| PEST + SWOT | PEST identifies external forces; SWOT converts internal/external context into strategic implications. |
| POPIT + gap analysis | POPIT structures current and future state; gap analysis identifies required changes. |
| Stakeholder matrix + elicitation plan | The matrix shows who matters; the plan explains how to involve them. |
| Document analysis + interviews | Documents provide existing evidence; interviews explain context, exceptions, and assumptions. |
| Observation + process model | Observation shows real work; the process model makes workflows and bottlenecks visible. |
| Fishbone + Pareto | Fishbone organises possible causes; Pareto prioritises the causes with greatest evidence of impact. |
| Personas + journey maps | Personas define the user segment; journey maps show that user's experience across touchpoints. |
| SMART objectives + KPIs | Objectives define the target; KPIs monitor whether the target is being achieved. |
| Use cases + wireframes | Use cases show interaction flow; wireframes show interface structure. |
| Traceability + validation | Traceability links requirements to needs; validation checks whether those links are meaningful. |

## Common Technique Mistakes

- Listing techniques without explaining why they fit the case.
- Jumping from a symptom to a solution without problem analysis.
- Treating technology as the whole change instead of using POPIT.
- Treating stakeholder analysis as a list of names.
- Calling every metric a KPI.
- Confusing SMART objectives with system requirements.
- Confusing verification with validation.
- Using a customer journey map as an internal process map.
- Treating a wireframe as a finished design.
- Recommending a solution without connecting it to need, value, feasibility, risk, and requirements.

