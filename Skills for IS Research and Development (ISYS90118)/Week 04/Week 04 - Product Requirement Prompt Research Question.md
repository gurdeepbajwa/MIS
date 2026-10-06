# Week 04 Research Question: Translating Business Needs into Requirements Plans

- Course: Skills for IS Research and Development (ISYS90118)
- Research area: Business analysis, requirements engineering, and Research through Design
- Parent tutorial: [[Week 04 - Theories Frameworks and Models Tutorial]]
- Related reading: [[Week 04 - Cluster 7 Design and Interaction Deep Dive]]
- Proposal tutorial: [[Week 06 - Research Proposal Tutorial]]
- Status: Earlier exploration, retained for reference. The current direction is [[Week 06 - Delivery Pressure and AI Coding Research Proposal]].

## Recommended Small-Paper Research Question

> **How does coverage of five predefined workflow exceptions differ between requirements plans created through user-led context provision and agent-led questioning for a fixed expense-approval scenario?**

In this study, a **requirements plan** is the final structured document that states what the feature must do, including its workflow rules and exceptions. After this definition, the study can call it the **plan**. It is not the AI coding agent's later implementation plan.

This version studies:

- one comparison: user-led context provision versus agent-led questioning;
- one part of context: workflow exceptions;
- one outcome: correct exception coverage;
- one artefact: the final requirements plan; and
- one fixed expense-approval scenario.

It does not study the full requirements document, code output, implementation plans, user roles, technical background, business value, or all forms of ambiguity.

### Five Predefined Exceptions

The scenario could contain these facts:

1. an expense above a stated amount needs a second approval;
2. a missing receipt needs a declaration;
3. an absent approver can delegate approval;
4. a claimant cannot approve their own expense; and
5. a rejected claim can be corrected and submitted again.

Both conditions must have access to the same facts. In the user-led condition, the participant decides which facts to provide. In the agent-led condition, the agent asks focused questions to elicit them.

### Main Measure

Score each exception in the final plan:

- `0`: absent or wrong;
- `1`: present but unclear or incomplete; or
- `2`: correct and clear.

The main result is the total exception-coverage score out of 10. Record whether the original business goal remains accurate as a basic quality check, not as a second main outcome.

## Broader Comparison Question

> **How do ambiguity and preservation of business intent differ between Product Requirement Prompts produced through user-led context provision and agent-led context elicitation from the same high-level expense-approval brief?**

This remains useful as a wider research question, but it covers two outcomes and every form of context or ambiguity in the PRP. It is too broad for the proposed small paper.

This question narrows the study to:

- one set of participants completing both or either context-gathering condition;
- one design intervention: agent-led context elicitation;
- one comparison condition: user-led context provision;
- one fixed expense-approval brief;
- one AI assistant, model, setup, and PRP format; and
- two main outcomes: ambiguity reduction and preservation of business intent.

An expert panel can create the reference checklist and rate the final PRPs without knowing which condition produced them. The panel may include business-analysis, product, requirements, and software-development experience. Participant technical experience can be recorded as background data, but it is not the research comparison.

### Supporting Questions

1. Which required data, workflow exceptions, access rules, integrations, and acceptance tests remain absent from each condition's final PRPs?
2. Which agent questions reveal new context rather than repeat, reword, or confirm facts already given?
3. Which parts of the participant's original business goal, desired outcome, users, and constraints remain accurate, become distorted, or disappear in each final PRP?
4. At what point do further questions add little new context but increase user effort?

Keep agent plans, code quality, business value, and the full development process outside this first study.

## What “Grilling” Means in the Study

Use the research term **adaptive AI questioning** or **AI-led requirements elicitation**. The protocol should:

1. read the current brief and answers;
2. identify the highest-priority missing or unclear item;
3. ask one focused follow-up question;
4. challenge vague terms such as *fast*, *secure*, *normal user*, or *approved*;
5. ask about examples, exceptions, constraints, and evidence;
6. record facts, assumptions, conflicts, and open questions separately;
7. summarise its current understanding for the user to correct; and
8. stop when it meets a stated rule rather than asking questions without a limit.

The intervention tests the design of the questioning process, not whether an AI can ask the largest number of questions.

## Different Roles of the Human and Agent

| Actor | Knowledge or action they should supply |
| --- | --- |
| Human participant | Business problem, desired outcome, users, current work, value, policy, domain knowledge, priorities, and unacceptable outcomes |
| AI assistant | Detect vague or missing points, organise context, ask focused questions, find conflicts, separate facts from assumptions, and state unresolved points |
| Human participant | Correct the AI's summary and approve whether the refined requirements still express the intended business need |

The agent should not invent missing business facts. It should turn uncertainty into a clear question or record it as unresolved.

## How the Agent Refines Ambiguous Context

The protocol should detect:

- vague terms such as *fast*, *easy*, *secure*, or *normal approval*;
- missing actors, actions, triggers, conditions, or outcomes;
- unclear data sources, fields, ownership, retention, or quality;
- unstated workflow exceptions and failure cases;
- undefined access and approval rules;
- missing system links or technical limits;
- conflicts between stated needs; and
- claims with no acceptance test.

For each issue, the agent should:

1. quote or point to the unclear part;
2. explain briefly what remains unknown;
3. ask one question that the participant can answer from business knowledge;
4. update the requirement without adding unsupported facts; and
5. ask the participant to confirm the revised meaning.

## Boundaries for the Study

### Participant Definitions

- **Participants:** people asked to turn the same high-level business brief into a PRP with the AI assistant. Technical experience is recorded but does not define the comparison groups.
- **Expert panel:** people with relevant business-analysis, product, requirements, or software-development experience who prepare the reference checklist and rate the PRPs.
- **Unit of analysis:** one participant's AI session and resulting PRP.

### Fixed Scenario

Use one brief for adding an expense-approval feature to an existing web system. Give every participant the same stated business goal, source material, time, PRP template, and AI access. Prepare an expert checklist of required details before collecting data.

### Study Conditions

- **User-led context condition:** the participant receives the business brief and supplies all context they think the AI needs. The AI may organise the material but does not ask follow-up questions.
- **Agent-led elicitation condition:** the participant begins with the same business brief. The AI follows the elicitation protocol, asks focused follow-up questions, summarises its understanding, and seeks confirmation before creating the PRP.

Hold these points constant where possible:

- the business-need scenario;
- the AI assistant and model;
- the PRP template;
- the task time;
- access to source material; and
- whether participants may ask another person for help.

Collect:

- AI chat records;
- each question asked by the AI and the information gained from it;
- the final PRP; and
- the participant's initial statement of business intent;
- time, question count, participant effort rating, and a blind expert rating against the checklist; and
- the participant's final rating of whether the PRP retains their intended meaning.

Compare:

- the percentage of required checklist items present in the final PRP;
- coverage by category: data, workflow exceptions, access rules, integrations, and acceptance tests;
- missing, unclear, conflicting, or assumed items;
- the percentage of initial business-intent statements represented correctly in the final PRP;
- business-intent statements that become distorted or disappear;
- questions and time needed; and
- participant-reported effort.

Define **ambiguity reduction** as the fall in the number of vague, missing, conflicting, or assumed items between the initial context and final PRP. Define **business-intent preservation** as the percentage of the participant's stated goals, users, desired outcomes, priorities, and constraints represented correctly in the final PRP. Do not use broad labels such as *good PRP*, *good plan*, or *good output* as measures.

## Working Definitions

A **business need** states the problem, goal, or desired change from the organisation's point of view. It explains why work may be needed.

A **business requirement** states an outcome or capability that the organisation or its users need. It should not assume a technical response too early.

A **system requirement** states what the system must do, how well it must do it, and which limits it must meet. It gives designers, developers, testers, and agents enough detail to act and check the result.

A **Product Requirement Prompt (PRP)** is a structured prompt that gives an AI coding agent the context, requirements, constraints, and checks for a software task.

An **agent plan** is the agent's proposed sequence of implementation steps. It may name the files, code changes, dependencies, tests, and checks needed to complete the PRP.

The **implementation output** includes the code changes, tests, explanations, and other evidence that the agent produces.

A **plan-to-output view** links each requirement and plan step to the code change, test, or other evidence that addresses it. It can also show omissions, changes to the plan, and unresolved points.

**Requirements translation** is the process of gathering business and user context, stating the needs, turning them into clear system requirements, and expressing them in a PRP that an agent can plan and implement. Translation does not mean changing words alone. It includes making choices, checking assumptions, resolving conflicts, adding technical detail, and retaining the reason behind each requirement.

These parts should remain distinct:

| Part | Main question |
| --- | --- |
| Business need | Do we understand the problem, goal, people, and setting? |
| Business and system requirements | Did we retain the need while adding enough detail to act? |
| PRP | Did we give the agent the right context, limits, and checks? |
| Agent plan | Did the agent propose a sound way to complete it? |
| Implementation process | Did the agent follow or revise the plan well? |
| Output | Does the result meet the stated needs? |
| Review view | Can a developer check the links and spot problems? |

## Research Problem

Business stakeholders, analysts, developers, and AI agents do not use the same terms or need the same level of detail. Each step from a business need to code can omit context, add an unchecked assumption, hide a conflict, or narrow the need too soon. A PRP may look complete in technical terms while failing to retain the business aim.

These gaps may lead to a sound implementation of the wrong requirement. They may also lead to weak agent plans, rework, defects, poor tests, or an output that stakeholders cannot accept. The problem therefore starts before the agent writes a plan.

The research should examine and refine the full chain:

> business need and context → business requirements → system requirements → PRP → agent plan → implementation → validation

## Earlier Broad Research Question

> **How can the process for creating and refining Product Requirement Prompts be designed to preserve business intent as needs and requirements are translated into implementable instructions for AI coding agents?**

This question remains useful as a wider research program, but it is too broad for the proposed first study. It treats the full translation process as the design object and includes several possible results: a process model, PRP structure, review checks, trace links, and a supporting tool.

## Supporting Questions

1. What business, user, domain, policy, data, and technical context must a PRP retain for an agent to plan the work?
2. Where do omissions, unclear terms, conflicts, and unchecked assumptions enter the path from business need to PRP?
3. How do stakeholders, analysts, and developers judge whether a PRP retains the original business intent and gives enough detail for implementation?
4. Which elicitation, representation, traceability, and validation steps reduce translation gaps?
5. How does the refined process affect agent-plan quality, requirement coverage, implementation defects, and rework?

## Narrower Alternative: Translation Gaps

> **What gaps arise when business needs are translated into Product Requirement Prompts for AI coding agents, why do they arise, and how do they affect agent plans and implementation outputs?**

This question first studies the current process. It fits if the project lacks enough time to design and test a refined process. It leans towards explanation rather than design and action.

## Narrower Alternative: Traceability Design

> **How can traceability between business needs, Product Requirement Prompts, agent plans, and implementation outputs help teams find and correct requirements-translation gaps?**

This version narrows the design work to one part of the process: retaining and checking links between stages.

## If the Aim Is to Test Cause

> **How does a structured PRP translation and validation process affect agent-plan quality, requirement coverage, implementation defects, and rework?**

This version needs a controlled comparison. The study should change one factor at a time while keeping the task, codebase, agent, model, tools, and test setting as stable as possible. Without that control, the study should say that factors are **linked to** or **associated with** outcomes rather than claiming that they cause them.

## Conceptual Model

| Stage | Candidate factors | Possible evidence or measures |
| --- | --- | --- |
| Context and business need | Stakeholders, goals, users, current process, policy, data, risks, value, and limits | Missing views; conflicting goals; source records |
| Requirements translation | Clear terms, retained reason, suitable detail, stated assumptions, resolved conflicts, and feasibility checks | Omissions; ambiguity; lost reasons; unchecked assumptions |
| PRP quality | Context, functional and quality needs, constraints, acceptance criteria, examples, risks, and open questions | Requirement coverage; expert rating; stakeholder approval |
| Plan quality | Correct steps, suitable detail, order, dependencies, file targets, tests, and checks | PRP coverage; invalid steps; review rating |
| Execution setting | Agent and model, tool access, codebase size, task difficulty, feedback, and human input | Tool failures; plan changes; retries; time |
| Output quality | Correctness, requirement coverage, tests, code quality, security, and limited unintended change | Test results; defects; expert review; changed scope |
| Business validation | Fit with the original need, stakeholder acceptance, value, and unwanted effects | Acceptance gaps; rework; stakeholder rating; rejected changes |

### Key Point

A good PRP, a good plan, sound code, and a useful business result are not the same outcome. The study must assess them separately. A technically correct output can still fail the business need. The study should also record the setting so that it does not blame the translation process for a tool failure or credit it for an easy task.

## Proposed Design Intervention

The main contribution could be a repeatable translation and validation process with these parts:

1. **Context gathering:** record stakeholders, goals, users, current work, rules, data, risks, and system limits.
2. **Layered requirements:** keep business outcomes, user needs, system requirements, quality needs, and constraints separate but linked.
3. **Assumption and question register:** show what remains unknown, who can answer it, and whether implementation can start.
4. **PRP structure:** give the agent the needed context, scope, acceptance criteria, examples, non-goals, and checks.
5. **Translation review:** ask business and technical reviewers to check different parts before the agent acts.
6. **End-to-end traceability:** link each business need to requirements, PRP sections, plan steps, code changes, and tests.
7. **Feedback and refinement:** use implementation gaps and review findings to improve both the PRP and the process.

A traceability view could show six linked columns:

1. business goal or problem;
2. business or user requirement;
3. system requirement and PRP item;
4. related agent-plan step;
5. code, test, or other output evidence; and
6. validation result, change, or unresolved point.

The view could flag:

- a business need with no system requirement;
- a requirement with no PRP item or plan step;
- a plan step with no output;
- code changes with no stated reason;
- a technical choice that changes the business meaning;
- a failed or missing test;
- a change from the plan and the reason for it; and
- a claim of completion with weak business or technical evidence.

## Research through Design Approach

1. Study how stakeholders, analysts, and developers now turn a business need into a PRP.
2. Map where context gets lost, changed, assumed, or added.
3. Create and try early versions of the translation process, PRP structure, and traceability view.
4. Use realistic tasks to follow requirements from need through agent output.
5. Record gaps, questions, plan changes, defects, rework, and stakeholder judgements.
6. Revise the process and artefacts based on the evidence.
7. State design principles that other teams can inspect and try.

The research contribution does not stop at the finished view. It must explain what the design work revealed and which principles others can use.

## A Small First Study

For a manageable first study:

- choose one type of small or medium software change;
- involve a business stakeholder or product owner, a business analyst, and a developer where possible;
- observe one current translation process and record its gaps;
- create one structured PRP process with trace links and review checks;
- run matched tasks with the current and refined processes;
- keep the coding agent and tool setup fixed;
- measure missing requirements, questions raised before coding, plan changes, defects, rework, and business acceptance; and
- interview participants about what the process clarified, hid, or made harder.

If access to real teams proves hard, the study could use a workshop with realistic scenarios and ask participants to translate, review, and implement the same needs with both processes.

## Link to Gregor

| Research part | Gregor type | Contribution |
| --- | --- | --- |
| Compare the types and amount of ambiguity in the two conditions | Type I: Analysis | A description or classification of observed differences |
| Explain why agent questions reduce ambiguity or change business intent | Type II: Explanation | An account based on dialogue records and participant evidence |
| Test whether agent-led elicitation reduces ambiguity while retaining intent | Type IV: Explanation and prediction | Predicted links tested through a controlled comparison |
| Design and refine the agent-led elicitation protocol | Type V: Design and action | A tested method, questioning rules, stopping rule, and design principles |

The current comparison question is not Type V by itself. If the study only records how the two conditions differ, it chiefly supports **Type I**. If it explains why the differences arise, it adds **Type II**. A controlled test of stated effects can support **Type IV**.

To make the main design contribution explicit, add this Type V question:

> **How should an agent-led context-elicitation protocol be designed to reduce ambiguity while preserving users' stated business intent when creating a Product Requirement Prompt from a high-level expense-approval brief?**

The Type V design question and the comparison question work together. The first asks what to build and which design rules to use. The second checks whether the designed protocol achieves its stated aims.

## Possible Cluster 7 Contributions

- **Artefact:** the PRP structure, traceability view, or supporting tool;
- **Empirical:** findings about translation gaps and their effects;
- **Theoretical:** a model of how business context moves through the PRP, plan, implementation, and validation stages;
- **Methodological:** a repeatable process for translating and validating requirements for agent work; and
- **Dataset:** an anonymised set of needs, requirements, PRPs, plans, changes, tests, and review findings, if ethics and code access allow it.

## Research Level

The main level is the **individual** because the study examines one person's context-gathering interaction with an AI assistant. It could later move to the group or organisational level if it studied team hand-offs, review roles, or firm-wide controls.

## Short Tutorial Pitch

> I want to compare user-led context provision with agent-led context elicitation when creating a Product Requirement Prompt from the same business brief. Technical background is not the comparison. The design part fits Gregor Type V because I would create and refine an agent questioning protocol aimed at reducing ambiguity without changing the user's stated business intent. Comparing the two conditions can provide Type I findings about their differences, Type II explanations of why the differences arise, or Type IV evidence if I test predicted effects under controlled conditions.

## References

Abubakar, M. A., Mohsenimofidi, S., Lulla, J. L., Zhang, J. M., Treude, C., Baltes, S., & Galster, M. (2026). *An exploratory study of agent plans for agentic AI coding tools in open-source software*. arXiv. https://arxiv.org/abs/2608.04661

Arora, C., Grundy, J., & Abdelrazek, M. (2023). *Advancing requirements engineering through generative AI: Assessing the role of LLMs*. arXiv. https://arxiv.org/abs/2310.13976

Beg, A., O'Donoghue, D., & Monahan, R. (2025). *Formalising software requirements using large language models*. arXiv. https://arxiv.org/abs/2506.10704

Gregor, S. (2006). The nature of theory in information systems. *MIS Quarterly, 30*(3), 611–642. https://doi.org/10.2307/25148742

Lipsanen, P., Rannikko, L., Christophe, F., Kalliokoski, K., Stirbu, V., & Mikkonen, T. (2026). *Shift-Up: A framework for software engineering guardrails in AI-native software development—Initial findings*. arXiv. https://arxiv.org/abs/2604.20436

Stappers, P. J., & Giaccardi, E. (2013). Research through design. In M. Soegaard & R. F. Dam (Eds.), *The encyclopedia of human-computer interaction* (2nd ed.). Interaction Design Foundation. https://www.interaction-design.org/literature/book/the-encyclopedia-of-human-computer-interaction-2nd-ed/research-through-design

Takerngsaksiri, W., Pasuksmit, J., Thongtanunam, P., Tantithamthavorn, C., Zhang, R., Jiang, F., Li, J., Cook, E., Chen, K., & Wu, M. (2024). *Human-in-the-loop software development agents*. arXiv. https://arxiv.org/abs/2411.12924

Wobbrock, J. O., & Kientz, J. A. (2016). Research contributions in human-computer interaction. *Interactions, 23*(3), 38–44. https://doi.org/10.1145/2907069
