# Practice Case 01 — The Confidential Briefing

Course: [[Cyber Security Management (ISYS90090)/Course Overview|Cyber Security Management (ISYS90090)]]
Source: [[Cyber Security Management (ISYS90090)/Assets/Week 04 - Confidential Briefing Case Study.pdf|Confidential Briefing case]]
Date: 18 August 2026
Type: Exam case-analysis practice

## Exam Rule: Facts Are Not Insights

- If the case directly states or shows something, it is a **fact**.
- An **insight** is an inferred pattern, problem, or root cause that explains several facts.
- A strong answer states the insight and then cites the facts that support the inference.
- Do not rename a fact and present it as an insight.

Use this form:

> **Insight:** [Inferred root problem]. **Supported by:** [two or more case facts]. **Triplet:** [asset, threat, and control implication].

## Five Triplet-Based Insights

### Insight 1: No party owns the briefing's security from creation to disposal

This is inferred from the movement of the briefing between the doctor, hospital office, chief of staff, government email, paper copy, and spoken discussion, followed by uncertainty about every possible route.

- **Asset:** Confidential briefing and the professional judgement it contains.
- **Threat:** Disclosure through any party or format involved in its lifecycle.
- **Control implication:** Assign one information owner, define custody at every transfer, record each copy, and confirm return or destruction.

### Insight 2: Security controls follow the container rather than the information

The organisations appear to control the patient record and email system separately, but the same sensitive meaning moves into paper and speech without equal control. This suggests that protection depends on where the content sits rather than what the content means.

- **Asset:** The confidential meaning of the briefing across digital, paper, and spoken forms.
- **Threat:** Loss of confidentiality when content moves to a less controlled form.
- **Control implication:** Apply one classification and handling rule to the information regardless of format.

### Insight 3: Senior staff culture allows urgency and convenience to override secure handling

This is inferred from Cole discussing the content while moving between meetings, requesting another copy to avoid carrying paper, leaving uncertainty about the printed copy, and using an unlocked drawer.

- **Asset:** Limited access to the briefing and its recommendations.
- **Threat:** Negligent disclosure by an authorised insider or opportunistic access by another person.
- **Control implication:** Provide role-specific training, secure storage, approved communication channels, and handling rules designed for senior staff working under time pressure.

### Insight 4: Security monitoring is too digital and cannot explain a cross-channel leak

The IT team can show that the email was not forwarded, but the office cannot trace paper access or spoken disclosure. This indicates that the control environment gives more visibility to systems than to the information itself.

- **Asset:** Confidentiality and traceability of the briefing.
- **Threat:** Physical access, overhearing, verbal relaying, photography, or another unlogged transfer.
- **Control implication:** Join digital logs with physical-access records, copy custody, secure-meeting practice, and staff interviews.

### Insight 5: Weak evidence preservation has turned containment into uncertainty

The office cannot reconstruct who held the paper, who heard the call, or which route reached the journalist. This suggests the organisation did not design its process to preserve evidence for a high-impact disclosure.

- **Asset:** The briefing, the ability to investigate it, and trust in the Prime Minister's office.
- **Threat:** Continued disclosure, false attribution, delayed containment, and poor decisions before the election.
- **Control implication:** Use numbered copies, access and custody records, rapid escalation, evidence-preservation steps, cross-channel investigation, and a time-sensitive response plan.

## Overall Root Insight

The core failure is the absence of information-centred governance across organisations and formats. The briefing's sensitivity did not produce one owner, one classification, one handling model, or one investigation trail.

## Self-Check

Before calling a point an insight, ask:

1. Is this wording already stated in the case?
2. Which two or more facts support my inference?
3. Does the inference explain why the incident became possible or difficult to manage?
4. Can I link it to an asset, threat, vulnerability, or control gap?
