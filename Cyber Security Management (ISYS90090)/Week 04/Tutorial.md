# Week 04 Tutorial

Course: [[Cyber Security Management (ISYS90090)/Course Overview|Cyber Security Management (ISYS90090)]]
Week: 04
Topic: Risk Identification and Management Practices
Type: Tutorial

## Source Material

- Live tutorial notes supplied on 18 August 2026.
- [[Cyber Security Management (ISYS90090)/Assets/Week 03 - Horizon Teaching Case Complete Canvas.txt|Complete Horizon teaching case, Scenes 1–14]].
- [[Cyber Security Management (ISYS90090)/Week 03/Horizon Case Study|Complete Horizon case analysis]].

## Live Tutorial Notes — Expand Later

### Risk-Management Phases

The tutor described four continuing phases:

1. **Risk identification:** Identify the assets, weaknesses, threats, threat actors, and possible risk scenarios.
2. **Risk assessment:** Estimate each scenario's likelihood and impact or severity, then set its priority.
3. **Risk response or treatment:** Avoid, mitigate, transfer, or accept the risk.
4. **Review:** Check that the process and controls work and look for changes that alter the risk.

Risk management is continuous. A change to an asset, system, process, threat, actor, or control should trigger fresh identification and assessment rather than wait for the next fixed review.

### Risk Identification

- Risk identification aims to find all relevant risks the organisation may face.
- The organisation should express each risk as a specific risk scenario rather than use a broad threat label.
- The tutor named four parts needed to identify a risk scenario:

  1. **Asset:** What has value and needs protection?
  2. **Weakness or vulnerability:** What makes the asset open to harm?
  3. **Threat:** What danger could affect the asset?
  4. **Threat actor:** Who or what may cause the harm?

- Later analysis should make clear how the actor uses the weakness and what impact may follow.

### Purpose of Risk Management

- Risk management is mainly about **prioritisation**.
- Organisations face many assets, threats, threat actors, and risk scenarios but have limited time, staff, money, controls, and effort.
- They must decide which risks need attention first and where security resources will reduce the most important exposure.
- The core process described by the tutor is:

  `identify risks → prioritise risks → address them with available resources`

- Risk assessment supports this choice by showing which scenarios matter most.
- An organisation with unlimited resources could attempt to address every risk, but real organisations must make choices and accept some remaining risk.

### Likelihood and Impact

Risk assessment examines two separate questions:

1. **Likelihood:** How likely is the risk scenario to occur?
2. **Impact or severity:** If it occurs, how serious will the harm be?

- A scenario may have low likelihood but very high impact.
- High impact does not make an event likely, and low likelihood does not make its impact small.
- Assess both dimensions before deciding the risk priority and response.
- The assessment should use one precise risk scenario so that the stated likelihood and impact refer to the same event.

### Risk Response or Treatment

This overlaps with risk responses covered in the Business Analysis course.

| Response | Meaning | Effect on the risk | Tutorial example |
| --- | --- | --- | --- |
| Avoid | Stop or do not begin the activity that creates the risk scenario. | Removes exposure to that specific scenario. | Do not use a route known to contain the danger. |
| Mitigate | Add controls that reduce likelihood, impact, or both. | Lowers the risk but may leave residual risk. | Following speed limits reduces accident likelihood; wearing a seatbelt reduces injury impact. |
| Transfer | Shift some financial cost, service, or handling duty to another party. | Does not stop the event itself; it changes who bears part of its cost or operation. | Buy insurance or outsource payment processing so the retailer does not store card details. |
| Accept | Make an informed decision to retain the risk without further treatment. | The organisation bears the impact if the event occurs. | Accept a low-impact risk when treatment would cost more than the harm it is expected to prevent. |

Key distinctions:

- A mitigation control may target likelihood, impact, or both; state which one it changes.
- Insurance does not stop an accident or reduce its likelihood. It transfers agreed financial costs.
- Outsourcing can transfer a task and some exposure, but the organisation should still manage supplier and business risk.
- Risk acceptance may be suitable when the risk falls within appetite or when further treatment costs more than the likely benefit.
- Acceptance should still involve ownership, approval, documentation, and monitoring. It should not result from overlooking the risk.

### Strategy

- **Core point:** Strategy provides direction and defines the high-level objective the organisation is working toward.
- The tutor linked the origin of strategy to **generalship**: how a leader directs available people and resources to achieve an objective.
- A strategy begins with a high-level objective rather than a small operational task.
- It explains how the organisation will use limited resources and coordinated action to move toward that objective.
- Historical examples used in class included conquest as Alexander the Great's high-level objective and freedom for enslaved people as Spartacus's objective.
- In cybersecurity management, a strategy should therefore connect security resources and choices to a clear organisation-level objective.
- The live explanation ended before the tutor presented the supporting strategy slide; add its remaining parts when provided.

#### Intended and Emergent Strategy

- **Intended strategy:** The direction and objective chosen in advance. Leaders deliberately plan how to move toward it.
- **Emergent strategy:** The direction or pattern that develops through actual choices, events, and changing conditions, including outcomes that were not part of the original plan.
- An organisation will still develop a direction through its actions even when it has not stated a clear strategy.
- Without a deliberate objective, its choices may support another party's aims or lead to an outcome it did not choose.
- Compare the original intention with the outcome that emerges to understand what the organisation's strategy became in practice.
- The tutor linked the intended–emergent distinction to Mintzberg and the earlier discussion of the 5 Ps.
- Strategy is not fixed. Leaders cannot know every future condition when they form it.
- Monitor the assumptions and conditions used to create the strategy.
- When those conditions change, adjust the strategy while keeping the intended high-level objective in view.
- This makes strategy an active process of direction, review, learning, and change rather than a one-time plan.

#### Link to Mintzberg's 5 Ps

- Strategy can be examined and aligned through Mintzberg's 5 Ps: **plan, ploy, pattern, position, and perspective**.
- Use the tutor's next explanation to show how each P relates to intended, emergent, and cybersecurity strategy.

#### Why Strategy May Be the Most Important Practice

1. **It sets direction and objectives:** Strategy defines what the organisation seeks to protect and the security outcome it wants to achieve.
2. **It guides scarce resources:** Strategy helps leaders choose which risks, assets, controls, and projects deserve time, money, and staff.
3. **It aligns and adapts the other practices:** Risk management, policy, training, culture, and technical controls can work toward the same objective and change when business conditions or threats change.

Strategy is not sufficient on its own. Its importance comes from giving the other management practices a shared direction and basis for decisions.

##### Comparison with Policy, SETA, and Risk Management

| Practice | What it does | Why strategy comes first if one practice must be ranked highest |
| --- | --- | --- |
| Policy | Records high-level rules and principles. | Policy needs a chosen direction before it can state which principles and expectations matter. |
| SETA | Builds security knowledge, skill, awareness, and culture. | SETA needs strategy and policy to define the behaviour and capability the organisation wants staff to develop. |
| Risk management | Identifies, assesses, prioritises, and treats risk. | Strategy defines business objectives, asset priorities, and risk appetite, which give risk decisions their business context. |
| Strategy | Sets objectives, direction, priorities, and how resources support them. | It connects the other three practices and helps them work toward the same business outcome. |

Risk information should also inform and change strategy. The relationship is not one-way, and strategy cannot replace policy, SETA, or risk management.

### Policy

- A policy is a document that states the high-level principles guiding what the organisation seeks to achieve.
- An information security policy states the organisation's high-level security principles and direction.
- The tutor described policy as a written expression of strategy that people can see and follow.
- Policy sets direction and expectations; detailed steps should sit in supporting standards, procedures, or work instructions.

#### Security Document Hierarchy

1. **Policy:** Sits at the top and states the organisation's high-level principles and direction. The managing director, CEO, board, or another suitable senior authority approves and signs it.
2. **Standards:** Set required rules or minimum requirements that support the policy.
3. **Procedures:** State who performs a task and how they perform it.
4. **Guidelines and supporting documents:** Give extra advice, examples, or information that helps people apply the policy and related controls.

Examples:

- A supplier-security policy may require the organisation to assess supplier risk.
- A supplier security-assessment procedure then explains who assesses each supplier and the steps they follow.
- An access-control standard may set minimum rules for granting, reviewing, and removing access.

Each lower-level document should trace back to and support the policy above it.

### Informal Controls and Security Culture

- Security culture is an **informal control** because it seeks to influence how people understand risk and behave at work.
- Training, education, and awareness help shape that behaviour and reinforce the organisation's security expectations.
- The purpose of a security education, training, and awareness program is to build the desired security culture across the organisation.
- The tutor's spoken acronym for this program was unclear and needs confirmation.
- Strong technical controls still depend on people who configure, operate, review, and use them.
- Staff who do not understand security may bypass controls, misuse access, miss warning signs, or cause incidents.
- Effective learning should explain **why** a security rule matters, not only what staff must do or how to do it.
- Formal policy, informal culture and learning, and technical controls should support one another.

## Follow-Up

- [x] Confirm the tutor's full four risk-management phases and their order.
- [ ] Confirm whether the course places risk identification inside risk assessment.
- [ ] Add a complete risk-scenario example from the tutorial.
- [x] Confirm the four risk-response options: avoid, mitigate, transfer, and accept.

## Horizon Case Links for Week 04

- **Scene 7:** Missing security strategy, narrow IT focus, weak training, and siloed ownership.
- **Scene 11:** Security strategy must match the actual adversary and risk.
- **Scene 12:** Weak risk identification, assessment, prioritisation, and review.
- **Scene 13:** Policy exists but fails as a practical organisational control.

See [[Cyber Security Management (ISYS90090)/Week 03/Horizon Case Study|Complete Horizon case analysis]] for facts, insights, and responses.
