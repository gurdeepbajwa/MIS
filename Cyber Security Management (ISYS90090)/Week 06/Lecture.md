# Week 06 — Risk Management

Course: [[Cyber Security Management (ISYS90090)/Course Overview|Cyber Security Management]]

Sources: 2026 Week 6 slides, Canvas Module A, and selected assigned readings. Retrieved in Safari on 15 September 2026. The full lecture transcript is saved alongside the slides; this first study note summarises the slides and module, rather than every spoken example.

## Purpose

Information security risk management helps an organisation decide what to protect and where to spend its limited resources. Its aim is to reduce residual risk to a level the organisation accepts. It requires continuing review as assets, threats, dependencies and controls change.

The triplet model connects assets, threats and controls. A specific risk scenario describes how a threat exploits a weakness in a particular asset and causes an impact.

## 1. Identify Risks

1. **Establish context:** define the scope and boundaries of the assessment. Include relevant internal dependencies and external parties such as suppliers, partners, customers and regulators.
2. **Identify assets:** include services, data, information, knowledge and organisational capability, as well as hardware and software.
3. **Value assets:** identify which assets matter most to business objectives.
4. **Develop scenarios:** explain what could happen, the weakness that enables it, and the resulting loss of confidentiality, integrity or availability.

An asset is anything of value to the organisation. A capability combines people, processes and technology. Listing only an IT system may conceal the separate information and knowledge it supports.

### Asset valuation

The slides reproduce a weighted-factor worksheet with criteria for revenue, profitability and public image. The example weights are 30, 40 and 30, totalling 100. A score of 0.8, 0.9 and 0.5 gives `30 × 0.8 + 40 × 0.9 + 30 × 0.5 = 75`.

This ranks asset importance. It is distinct from rating the likelihood and impact of a particular risk scenario.

### Extra Materials — Writing a precise scenario

Use: **[Threat actor/event] exploits [specific weakness] affecting [asset], causing [CIA loss] and [business consequence].**

Example for practice: an attacker exploits an unsupported clinical application's reachable vulnerability, encrypts its records and delays treatment. The reachable vulnerability is an assumption until evidence confirms it; an old operating system alone does not establish exposure or a high likelihood.

## 2. Assess and Prioritise Risks

The course uses `Risk rating = Probability × Impact` with a consistent qualitative rating model.

- **Likelihood:** how likely the specified scenario is to occur. The lecture lists past records, experience, simulations, experiments and specialist judgement as evidence sources.
- **Impact/consequence:** the harm if that scenario occurs. The lecture considers direct financial cost, lost productivity, recovery of the asset or reputation, and penalties.
- **Priority:** compare the resulting ratings to decide which scenarios need attention first.

Impact depends on the scenario. Disclosure of a document may have a different cost from temporary loss of access to the same document. Do not assign one identical impact to every possible attack on an asset.

### Extra Materials — Matrix use

Define the meaning of Low, Medium and High before rating scenarios. Record reasons, existing controls and uncertain evidence. Numerical labels on a qualitative matrix support consistent ranking; they do not create precise probabilities.

The [[Cyber Security Management (ISYS90090)/Week 06/Tutorial|hospital workshop]] uses a 3 × 3 matrix. That is the exercise requirement, not a rule that all organisations use the same matrix.

## 3. Control Risks

The lecture's four response labels are:

| Strategy | Week 6 slide wording, paraphrased |
| --- | --- |
| Avoidance | Prevent the scenario by applying safeguards. |
| Transference | Transfer risk to another party or entity. |
| Mitigation | Reduce impact through incident response. |
| Acceptance | Understand the consequences and accept the risk. |

Select the strategy, select suitable controls, then implement them. Check feasibility and cost against the harm the controls address.

### Extra Materials — Terminology caution

Earlier tutorial notes use **avoid** for stopping an activity and **mitigate** for reducing likelihood, impact or both. Week 6 slides use **avoidance** more broadly for prevention and **mitigation** specifically for reducing impact. Recognise the lecturer's labels when answering a question framed around these slides, and explain what a control actually changes.

Transfer can shift some financial loss or duties; it does not guarantee that all exposure or responsibility disappears. Acceptance should follow assessment and an authorised decision, rather than neglect.

## 4. Review and Maintain

Revisit scenarios, likelihood, impact and controls as conditions change. Check that controls work and use lessons from earlier incidents and assessments. Canvas describes four phases: identification, assessment, response and review. Some presentations combine response and review under risk control; the lecture diagram also shows maintenance separately.

## Risk Appetite and Residual Risk

Canvas A.2.1 asks what influences how much risk an organisation will accept when balancing control investment against exposure. The module summary frames the objective as acceptable residual risk.

### Extra Materials — Plain definitions

- **Risk appetite:** the amount and type of risk an organisation is willing to take in pursuing its objectives.
- **Residual risk:** the risk that remains after the chosen controls operate.
- **Risk tolerance:** acceptable limits around risk exposure or variation in outcomes; check the textbook's precise wording when reading the assigned section.

Factors to consider include objectives, critical services, potential harm, obligations, resources and stakeholder expectations. The textbook itself is not saved in this course folder; these explanations do not replace its assigned section.

## Three Deficiencies in Risk Management

The lecture and Webb et al. (2014) identify:

1. **Perfunctory identification:** assessments identify risks superficially and omit important assets, relationships or attack scenarios.
2. **Weak grounding in the actual situation:** estimates rely too little on the organisation's real assets, threats, controls and evidence.
3. **Intermittent, non-historical assessment:** assessments occur infrequently and fail to learn from previous incidents and assessments.

These weaknesses can produce a plausible-looking ranking that directs resources towards the wrong problems.

## Related Deficiencies in Asset Identification

Keep this second set of three separate from the lecture's broader risk-management deficiencies. Shedden et al. (2016), listed as optional by Canvas, identify:

1. **Coarse granularity:** broad asset labels hide distinct content, uses and risk scenarios.
2. **Formal-process bias:** official process descriptions miss informal work, shortcuts and unofficial copies.
3. **Neglected knowledge:** systems and people appear in the inventory, while the specific knowledge needed for the business remains unidentified.

Their rich description method combines observation, interviews and document analysis with process maps and narratives. It complements traditional assessments by examining actual work. It is not presented as a fully validated replacement for all existing methods.

## Course Video

[Piya Shedden interview — Risk in Information Security, 13:31](https://canvas.lms.unimelb.edu.au/courses/237535/discussion_topics/1644110).

The supplied 2017 transcript highlights distributed ownership, technical staff lacking context about the data they protect, and differences between compliance, customer care and evidence-led risk decisions. Investment may follow risk evidence, breaches or regulatory pressure. Treat its industry examples as historical interview evidence.

## Sources and Reading

- Ahmad, A. (2026). *Risk management* [Week 6 lecture slides]. University of Melbourne. [Canvas file](https://canvas.lms.unimelb.edu.au/courses/237535/files/28540086).
- University of Melbourne. (2026). *Practice area A: Risk management* [Canvas module]. See [[Cyber Security Management (ISYS90090)/Weeks 06-07 - LMS Materials|LMS materials index]] for individual pages and readings.
- Prescribed textbook: Whitman and Mattord (2022), *Principles of information security*, Chapter 4, pp. 121–175. A.2 breaks this into pp. 122–128, 128–152 and 152–155. Its final range says “157–155”, an apparent typo; do not silently correct it.

## Applied Diataxis Notes

- [[Cyber Security Management (ISYS90090)/Week 06/Tutorial|Hospital risk register tutorial]]
- [[Cyber Security Management (ISYS90090)/Quizzes/Week 08 - Quiz Preparation|Weeks 6–7 quiz preparation]]
