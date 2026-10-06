# Week 07 — Information Security Policy

Course: [[Cyber Security Management (ISYS90090)/Course Overview|Cyber Security Management]]

Sources: current 2026 Week 7 slides, Canvas Module B, Höne and Eloff (2002), and Onibere's course interview. Retrieved in Safari on 15 September 2026. Full lecture slides and transcript are saved; this first note summarises the slide/module concepts, rather than every spoken example.

## What Policy Does

A policy communicates senior management's direction to people who make decisions and perform work. The more detailed Olson and Abrams definition also covers how an organisation manages, protects and distributes resources, who receives authority, and the conditions for exercising it.

Policy is a **formal control**. It sets expectations and responsibility. Its effectiveness depends on how it affects routine decisions and behaviour.

## Reasons for Having Policy

| Motivation in the course | Purpose |
| --- | --- |
| Marketing | Demonstrate commitment to security to the board and external parties. |
| Politics/management | Clarify obligations and responsibility, direct security work and spending, and provide continuity when managers change. |
| Personnel management | Define acceptable behaviour, create awareness and state consequences and due process for breaches. |
| Standards accreditation | Provide documented security direction required for relevant accreditation. |

The lecture calls policy relatively cheap to write but difficult to implement. It should support the business, involve end users, receive management support and align with applicable obligations.

## Policy Types and Hierarchy

The slides describe managerial, operational, acceptable-use and strategic policies. Strategic policy overlaps managerial and operational concerns.

They also identify three scopes: enterprise information security program policy, issue-specific policy and system-specific policy. Do not confuse this scope classification with the levels of documentation below.

| Document | Function |
| --- | --- |
| Policy | Senior management's direction and requirements. |
| Standard | Specific requirements that support the policy. |
| Procedure | Who does what and the steps for carrying it out. |
| Guideline | Advice that supports sound application. |

### Extra Materials — Example

A policy requires protection of confidential records. A standard specifies approved storage and access requirements. A procedure tells staff how to request and review access. A guideline helps staff handle an unusual sharing request. Exact mandatory status should follow the organisation's definitions.

## Bull's-Eye Model

The lecture presents this order: **policies → networks → systems → applications**.

Its logic is to establish usable, communicated and enforced policy, then secure networks, critical systems and applications. Learn the order and its rationale. This is the course's sequencing model; it does not by itself settle how to handle an urgent live incident.

## Four Conditions for Effectiveness

1. **Reading/dissemination:** the intended audience receives and can access the policy.
2. **Comprehension:** the audience understands what it requires.
3. **Compliance/agreement:** the audience agrees to comply.
4. **Uniform enforcement:** the organisation enforces it consistently across the audience.

Policies also require continuing review and maintenance.

### Extra Materials — How to test these

Check distribution and access records, use short scenarios to test understanding, obtain acknowledgements, and review how managers handle comparable breaches. A signature can show acknowledgement but does not by itself prove understanding or consistent behaviour.

## Nine Policy Quality Attributes

These attributes come from the lecture's two policy-quality tables. They are distinct from the four implementation conditions above.

| Attribute | Meaning | How to assess it |
| --- | --- | --- |
| Completeness | Covers all relevant security requirements. | Map objectives and directives to statements; identify gaps. |
| Suitability | Fits this organisation and its culture. | Compare with needs, obligations and actual behaviour. |
| Accuracy | Correctly expresses the requirements. | Have relevant business, security and legal stakeholders review wording. |
| Interoperability | Works with the organisation's other policies. | Check for conflicts, gaps and inconsistent structure or wording. |
| Security | Protects the policy's own confidentiality, integrity and availability. | Avoid exposing attack-enabling details while ensuring intended users can access what they need. |
| Analyzability | Allows systematic examination for faults. | Check logical structure and whether related statements can be found and reviewed. |
| Stability | Limits unintended effects when parts change. | Assess dependencies and whether a change creates new problems elsewhere. |
| Changeability | Can adapt efficiently to new conditions. | Check whether related statements form clear modules that can be revised. |
| Testability | Allows evaluation of effectiveness, including after changes. | Trial a policy module and collect usable feedback before wider deployment. |

### Extra Materials — Common distinctions

- Complete does not necessarily mean accurate: every topic could appear but contain incorrect requirements.
- Accurate does not necessarily mean suitable: technically correct wording may be unusable for the intended staff.
- Changeability concerns making an update; stability concerns avoiding unwanted effects from that update.
- Policy security does not mean keeping the entire policy secret from employees who must use it.

## Effective Policy: Assigned Reading

Höne and Eloff (2002) link effectiveness to users understanding what is expected and using the policy in their work. A document must be meaningful and practical for its audience and support the organisation's objectives.

Their six supporting activities are **development, styling, presentation, commitment, dissemination and maintenance**:

- Involve stakeholders and intended users in development.
- Use clear wording and a tone that suits the organisation's communication style.
- Keep the main document short and readable; use supporting documents for detail.
- Show management commitment through behaviour and participation.
- Distribute and explain the policy through channels staff use.
- Review it as the organisation changes, with attention to normal business cycles.

## Official Policy and Actual Practice

The module warns that policies can be too prescriptive, too abstract, irrelevant or complex. A policy that conflicts with how people work may have little practical effect.

The lecturer links policy with risk assessment, SETA and technical controls. Onibere's 2017 interview distinguishes compliance as a driver from active management of threats and risks. Changes in the threat environment, business or organisational capability should prompt review. Training should explain and reinforce the policy, including for senior managers.

## Course Video and Reading

- [Mazino Onibere interview — Policy in Information Security, 6:10](https://canvas.lms.unimelb.edu.au/courses/237535/discussion_topics/1644107). The RTF transcript is saved locally.
- Prescribed textbook: Whitman and Mattord (2022), *Principles of information security*, Module 3 policy section, pp. 88–104. The textbook itself is not saved in the course assets.
- The ANZ suite is a teaching example from approximately 2004/2005, used with permission. Do not present it as ANZ's current policy.

## References

Ahmad, A. (2026). *Information security policy* [Week 7 lecture slides]. University of Melbourne. https://canvas.lms.unimelb.edu.au/courses/237535/files/28665328

Höne, K., & Eloff, J. H. P. (2002). What makes an effective information security policy? *Network Security, 2002*(6), 14–16. https://canvas.lms.unimelb.edu.au/courses/237535/files/28186995

Onibere, M., & Ahmad, A. (2017). *Policy in information security* [Video]. University of Melbourne. https://canvas.lms.unimelb.edu.au/courses/237535/discussion_topics/1644107

## Applied Diataxis Notes

- [[Cyber Security Management (ISYS90090)/Week 07/Tutorial|Policy case diagnosis workshop]]
- [[Cyber Security Management (ISYS90090)/Quizzes/Week 08 - Quiz Preparation|Weeks 6–7 quiz preparation]]
- [[Cyber Security Management (ISYS90090)/Weeks 06-07 - LMS Materials|Source files and module index]]
