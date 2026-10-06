# Week 06 Tutorial

Course: [[Cyber Security Management (ISYS90090)/Course Overview|Cyber Security Management (ISYS90090)]]
Week: 06
Topic: Cybersecurity Risk Register
Type: Tutorial

## Source Material

- Live tutorial scenario supplied on 1 September 2026.

## Scenario: Merciless Hospital

### Given Facts

- The hospital runs critical clinical applications on premises.
- These applications support core hospital business and care processes.
- The hospital holds highly sensitive patient data.
- Some systems use obsolete or legacy operating systems.
- The scenario names **Scattered Spider** as the threat actor and states that it targets Australia and healthcare.
- The scenario associates the actor with ransomware and extortion.
- The hospital forms part of critical infrastructure.

Do not treat an unstated detail as a fact. Record assumptions and validate them during the assessment.

## Required Workshop Output

- Apply the principle of at least three: identify at least three distinct risk scenarios.
- For each scenario, identify the asset, weakness, threat, threat actor, impact, likelihood, impact rating, and overall risk rating.
- Use a three-by-three matrix with Low, Medium, and High levels.
- Record the results in a risk register.

## Three-by-Three Risk Matrix

| Impact \ Likelihood | Low | Medium | High |
| --- | --- | --- | --- |
| **High** | Medium | High | High |
| **Medium** | Low | Medium | High |
| **Low** | Low | Low | Medium |

The matrix is a workshop model. The organisation should define and approve its own rating criteria and thresholds.

## Draft Risk Register

| ID | Asset | Precise risk scenario | Weakness or vulnerability | Threat | Threat actor | Likelihood | Impact | Rating |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| R1 | Availability of critical clinical applications | Scattered Spider exploits an unpatched flaw in an obsolete clinical-system operating system and deploys ransomware, stopping clinicians from using the application during patient care. | Obsolete or unsupported operating system with security flaws that may not receive fixes | Ransomware encryption and service disruption | Scattered Spider | High | High | High |
| R2 | Confidentiality of sensitive patient data | Scattered Spider gains access through a vulnerable legacy system, copies patient data, and threatens to publish it unless the hospital pays. | Legacy access path to sensitive data and missing security updates; connection to the patient-data store must be confirmed | Data theft and extortion | Scattered Spider | Medium | High | High |
| R3 | Integrity of clinical information | After compromising an obsolete system, Scattered Spider's ransomware corrupts or alters clinical records, causing staff to rely on incomplete or incorrect information. | Obsolete system, weak integrity protection, or weak recovery validation; the exact control gap must be checked | Ransomware-related corruption or unauthorised change | Scattered Spider | Medium | High | High |

## Rating Reasons

- **R1 likelihood — High:** The case gives both an exposed weakness and an actor associated with ransomware against this sector. Confirm network exposure and current controls before finalising the rating.
- **R2 likelihood — Medium:** Extortion fits the stated actor, but the case does not prove that the obsolete system can reach patient data.
- **R3 likelihood — Medium:** Corruption can occur during ransomware, but the case does not state that deliberate clinical-data alteration is the actor's main objective.
- **All three impacts — High:** Loss of application availability, patient confidentiality, or clinical-data integrity may harm care, safety, legal duties, operations, and trust.

## Triplet Check

For each row, confirm:

1. **Asset:** Is it exact enough to value and protect?
2. **Threat:** What harmful event can affect that asset?
3. **Threat actor:** Who may cause the event, and what do their motives and methods suggest?
4. **Vulnerability:** Which specific weakness enables the event?
5. **Control:** Which treatment would reduce likelihood, impact, or both?

## Follow-Up

- [ ] Confirm which obsolete systems store or can reach patient data.
- [ ] Check whether the systems are internet-facing or reachable through remote access.
- [ ] Review network separation, identity controls, patch exceptions, monitoring, backups, and recovery testing.
- [ ] Add risk owners and treatment actions after the workshop group chooses its final scenarios.
