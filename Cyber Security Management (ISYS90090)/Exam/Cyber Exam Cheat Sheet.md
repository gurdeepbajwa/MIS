# Cyber Exam Cheat Sheet

Course: [[Cyber Security Management (ISYS90090)/Course Overview|Cyber Security Management (ISYS90090)]]
Type: Exam reference
Use: fast recall for multiple choice and short answer, and a concept bank for Section C.
Companions: [[Cyber Exam Study Guide - Section C]], [[Horizon Question Workbook - Facts and Insights]], [[Cyber Flashcard Deck]]

## Source Coverage and Gaps

- Weeks 2–9 come from your lecture notes, which draw on slides, transcripts, and Canvas.
- Week 10 comes from the **slides only**. There is no Week 10 lecture note or transcript in the workspace, and the prescribed reading (pp. 186–222) is not stored.
- Week 11 comes from a Canvas page capture. No slides or transcript were posted. Ahmad, Bosua, and Scheepers (2014, Table 1) on knowledge-leakage controls is **not in the workspace**, so the Week 11 control list below is deliberately thin. Add it when you have the table.
- Textbook pages are not stored. Whitman and Mattord (2022) points come from the lecturer's summaries.

## One-Screen Spine

`Triplet → Threats → Management practices → Controls → Strategy → Response → Knowledge`

| Week | Theme | Hook |
| ---: | --- | --- |
| 2 | Triplet model, CIA, roles, CISO | Asset ← risk ← threat; controls mitigate |
| 3 | Threat landscape | Actor, vulnerability, vector, attack, impact |
| 4 | Management overview | Risk, strategy, policy, SETA; process not product |
| 5 | Defence in depth | Separate, observe, mediate |
| 6 | Risk management | Identify, assess, respond, review |
| 7 | Policy | Four conditions, nine quality attributes |
| 8 | SETA | Why, how, what; seven steps; Kelman |
| 9 | Strategy | Nine paradigms; obscurity, weakest link, shared security |
| 10 | Incident response | Not preventative; kill chain; structure and gaps |
| 11 | Knowledge leakage | Data, information, knowledge; containers and flows |

## Section C in Five Lines

- **C1 (15):** five insights, each a derived root cause with at least two facts and "why it matters". Facts are written in the case. Insights are inferred.
- **C2 (10):** one risk. Asset, threat actor, specific vulnerability, impact, and why it beats the others.
- **C3 (25):** five recommendations. Each says what changes, how it reduces the C2 risk, and who owns it. Spread across altitude (strategic, tactical, operational) and type (formal, technical, informal).
- **Altitude:** strategic answers explain organisation design, ownership, and why teams do not talk. Operational answers add a tool or fix one person.
- **Assume:** the case concerns knowledge and capability rather than IT availability.

## Week 2 — Triplet, CIA, Roles, CISO

| Item | Recall |
| --- | --- |
| Triplet | Information resources (assets), threats, controls. Vulnerability gives the threat a path |
| Risk scenario | Specific threat exploits a specific vulnerability in a specific asset with a specific impact |
| Risk profile | All risk scenarios together |
| Risk appetite | Amount of risk the organisation accepts |
| Asset categories | Digital platforms; data and information; knowledge (explicit and tacit) |
| CIA | Confidentiality: read only by authorised. Integrity: changed only by authorised. Availability: usable when needed |
| Control categories | **Formal** (policy, standards; prescriptive), **informal** (education, culture; suggestive), **technological** (restrictive) |
| Four roles of information security | Protect ability to function; enable safe operation of applications; protect data, information, and knowledge; safeguard technology assets |
| CISO | Leads the security programme: strategy, policy, culture, risk, response, compliance, budget, teams |
| Survey cautions (Heidrick & Struggles 2022) | 327 respondents, self-reported, large-firm and US lean. CISOs often report to the CIO (38%); only 8% report to the CEO; stress 59% |
| Strategic lesson | Treat partners and suppliers as possible future threat actors. Threat intelligence looks at motives and warning signs |

## Week 3 — Threat Landscape

| Term | Meaning |
| --- | --- |
| Threat | Ongoing danger |
| Threat agent / actor | Who or what acts |
| Vulnerability | Weakness |
| Attack vector | Route used |
| Attack | Exploit that causes impact |
| Impact | Harm |

- **Motives:** extortion, theft, revenge, indirect access, competitive gain, national-security aims.
- **Taxonomy:** accidental or malicious; ad hoc or organised; lower or higher capability; operational or strategic motive.
- **Spectrum:** amateurs → hackers → insiders → advanced persistent threats.
- **APT cycle:** gather intelligence → study controls → enter → keep access → reach assets → finish objective and move on.
- **Attacker–defender imbalance:** attackers choose time, place, and method; know the target; focus fully; code copies cheaply; defenders have budgets, compliance, and a large attack surface.
- **Incident analysis:** incident (five Ws), trigger (why it is a security event), process (controls).
- **Fourteen threat categories (Whitman and Mattord):** IP compromise, software attacks, quality-of-service deviation, espionage or trespass, forces of nature, human error, information extortion, weak policy or planning, weak controls, sabotage, theft, hardware failure, software failure, obsolescence.
- **Exam habit:** give at least three correct, distinct points where the question allows.
- **Errors:** calling the attacker the threat (agent is the actor), calling a weakness a vector, treating every threat as external and deliberate.

## Week 4 — Management Overview

- **Security is a process, not a product.** No single control provides it. Organisations must understand assets and threats, choose matched controls, set rules, train people, test, respond, and review.
- **Risk phases:** identify → assess → respond → review. **Responses:** avoid, mitigate, transfer, accept. **Priority:** likelihood × impact on a consistent scale.
- **Compliance versus risk-based:** compliance gives a baseline and meets duties. It may not fit the organisation and does not prove security. Use compliance as the floor and risk assessment to tailor.
- **Strategy versus policy:** strategy chooses direction, priorities, and investment. Policy states rules and responsibilities.
- **SETA:** an informal control that explains rules and builds behaviour.
- **CISO roles:** strategist, advisor, technologist, guardian. The chart shows a desired shift from technologist and guardian towards strategist and advisor.
- **Policy success:** owner, reaches audience, readable, practical and enforceable, timely, fits culture, reviewed.

## Week 5 — Defence in Depth

- **Definition:** several successive, linked controls between actor and asset. Assume any single control may fail.
- **Three functions:** **separate** (firewalls, segmentation, VPN), **observe** (IDS, IDPS, multiple vantage points, logs), **mediate** (identity, authorisation, least privilege, need-to-know, encryption).
- **Detection types:** signature (known patterns, misses new attacks) and anomaly or behaviour (flags unusual activity, false alerts).
- **Attack surface:** what is exposed, misconfigured, leaking. A penetration test is a **dated snapshot**.
- **Deception:** honeypot, honeynet, padded cell.
- **Why the castle weakens:** cloud (data owned but not possessed), distributed workforces, AI.
- **Cloud:** IaaS, PaaS, SaaS. The organisation remains accountable.
- **Common errors:** treating a firewall as the whole perimeter, confusing authentication with authorisation, assuming VPN traffic is safe, treating a penetration test as proof of security.

## Week 6 — Risk Management

- **Identify:** establish context, identify assets (include knowledge), value assets, develop scenarios.
- **Scenario sentence:** [actor/event] exploits [weakness] affecting [asset], causing [CIA loss] and [business consequence].
- **Asset value ≠ scenario impact.** Weighted-factor example: 30 × 0.8 + 40 × 0.9 + 30 × 0.5 = 75.
- **Rating:** probability × impact on a defined matrix.
- **Lecture's response labels:** avoidance (prevent via safeguards), transference, mitigation (reduce impact via incident response), acceptance. Earlier tutorials used avoid as stop the activity and mitigate as reduce likelihood or impact. Know both and say what the control changes.
- **Residual risk:** what remains after controls. Risk appetite: amount and type accepted.
- **Three practice deficiencies (Webb et al., 2014):** perfunctory identification; weak grounding in the real situation; intermittent, non-historical assessment.
- **Three asset-identification deficiencies (Shedden et al., 2016):** coarse granularity, formal-process bias, neglected knowledge.

## Week 7 — Policy

- **Policy:** senior management's direction. Formal control.
- **Reasons:** marketing, politics and management, personnel management, standards accreditation.
- **Hierarchy:** policy → standard → procedure → guideline.
- **Scopes:** enterprise program, issue-specific, system-specific.
- **Bull's-eye:** policies → networks → systems → applications.
- **Four conditions:** dissemination, comprehension, compliance, uniform enforcement.
- **Nine quality attributes:** completeness, suitability, accuracy, interoperability, security, analyzability, stability, changeability, testability.
- **Höne and Eloff (2002), six activities:** development, styling, presentation, commitment, dissemination, maintenance.
- **Formal versus informal policy:** written rule versus accepted behaviour. If leaders ignore a rule, staff learn the rule is optional.

## Week 8 — SETA

| | Education | Training | Awareness |
| --- | --- | --- | --- |
| Question | Why | How | What |
| Level | Insight | Knowledge | Information |
| Objective | Understanding | Skill | Exposure |
| Aimed at | Security leaders | Everyday users needing skills | Everyone, repeatedly |
| Impact | Long term | Intermediate | Short term |

- **Good programme:** current, situated, small, sustained.
- **Seven steps:** scope, goals, and objectives → training staff → target audiences → motivate → administer → maintain → evaluate. The lecturer said that if the exam asks you to build a SETA programme, he wants the seven steps.
- **Step 1 is where programmes fail:** study the current culture first.
- **Kelman:** compliance (punishment, needs certain and severe sanctions), identification (belonging, role models), internalisation (own beliefs).
- **Challenges:** competes for attention, one size fits none, compliance drives the format, doing it properly is expensive. **Culture is the biggest barrier.**
- **Training tourism:** off-site training fades when people return to the organisation's inertia.

## Week 9 — Strategy

- **Definition to learn:** deciding how best to use defensive technologies and measures, deployed in a **coordinated** way, against **internal and external** threats, to provide CIA at **least effort and cost**, while being **effective**.
- **Nine paradigms:**
  - Behaviour: prevention, detection, response, deterrence, surveillance, deception.
  - Structure: perimeter, compartmentalisation, layering.
- **Distinctions:** surveillance is broad awareness and detection is narrow. Prevention is wider than perimeter. Deterrence needs sanctions that are certain and severe.
- **Combining:** weak prevention needs stronger detection and response.
- **Deception:** removes attacker leverage before the attack but must keep changing.
- **Three principles:** obscurity is not security; the weakest link depends on the attacker; shared security.
- **Bull's-eye (digital and cognitive environments):** the digital side has many layers and the human side has few, which is why social engineering often beats technical attack.
- **Cost rule (spoken):** spending much more than about 10% of an asset's value to protect it is a warning sign. This was stated verbally and is not a course formula.

## Week 10 — Incident Response (From Slides)

- **Incident response is not a preventative control.** It mitigates risk after a threat has acted.
- **Operational loop:** detect → contain → eradicate → recover, restoring the control-centred "shield" and business operations.
- **Early model:** logs → SIEM → SOC levels 1 to 3 → IT team → C-suite → board. Alerts climb the technology stack and reach executives as a status report. Nobody asks what the attacker was after.
- **Emergency-department problem:** response is so busy with volume that nobody sees the pattern of an organised, persistent attack.
- **Cyber kill chain (seven stages):** reconnaissance → weaponisation → delivery → exploitation → installation → command and control → actions on objectives. The slide groups these into preparation, intrusion, and active breach, with timelines of hours to months for early steps, seconds for the middle, and months for the end.
- **Research (two banks, same sector and attackers, different structures):**
  - **Bank H (fully insourced):** operations lead can reach twelve domain leads; Security Leadership Team forms within the hour; **two bridges** (operations and management); threat intelligence at three levels; blind spots eliminated deliberately; executives supply business context. The lever is **structure, authority, and the right people in one room**, not budget.
  - **Bank M (hybrid, outsourced specialists, internal coordination):** perception is sound but **comprehension breaks**; the experts are outside the room; information flow is transactional; sensemaking is sequential; the lever is **engagement across boundaries**. At least 60% of large organisations globally run this model.
- **Three gaps (every organisation studied had at least two):**
  - **Leadership:** the enterprise is not engaged with the response.
  - **Engagement:** the threat environment is not engaged with at all (who, why, will they return).
  - **Institutionalisation:** the incident does not change the organisation.
- **Prevention versus response (Week 10 strategic slide):** build a shield of safeguards against a broad spectrum, then respond to restore it after sophisticated, purposive attack.

## Week 11 — Knowledge Leakage (From Canvas Capture)

- **Information states:** resident (in a container) or transmitted (moving between containers).
- **Containers:** people, paper, digital media. The digital model adds printing, scanning, network transmission, photocopying, and conversion between digital and physical without a human.
- **Flows:** conversation, reading, writing, printing, scanning, copying, network transfer.
- **Impacts:** short term (lost revenue, breach of confidentiality agreements, lost productivity, effort to regain trust and market position) and long term (reputation and **competitive erosion**).
- **DIKW:** data, information, knowledge, wisdom. Data is raw. Information is data in context. Knowledge adds experience and judgement. Check Baskarada and Koronios (2013, pp. 5–8) for exact definitions.
- **Why it matters for security:** knowledge cannot be protected by protecting files alone.
- **Intelligence cycle:** introduced to improve situation awareness. The phases were not captured in the workspace. Check the slides.
- **Thompson and Kaarst-Brown (2005):** the paper lists **nine** dilemmas in Table 1. The Canvas page says seven, so confirm with your tutor which set is examined. Key ones for cases: classification systems lack coherence; "sensitivity" is vague; boundary-based models ignore people who cross boundaries; sharing information increases exposure but is often required; human judgement of sensitivity is poorly understood. A survey cited in the paper found that **39%** of organisations did not classify sensitive information (Hulme, 2001, as cited in Thompson & Kaarst-Brown, 2005, p. 248).

## Reading and Expert Opinion Takeaways

Short distillations of the extra readings you supplied. Attach each to the case concept it supports.

### Baskerville — Strategy in Information Security (Expert Insight, 2018)

- Past: when computers were isolated, physical locks gave near-complete security. Networking made leakage possible across cables and wiring.
- Attack **sophistication rises** because information assets are valuable, so attackers invest heavily.
- **Defence lags attack.** Responses are always a step behind and organisations must prepare for attacks they have not seen.
- **Two paradigms:**
  - **Business information systems security (BISS):** prevention and risk management; more prevention means less risk; reduce the probability of loss.
  - **Information warfare:** expect an innovative, unexpected attack on unnoticed vulnerabilities; agility and response matter more than prevention.
- **APTs bring warfare-style attacks into business.** Incident response therefore becomes more important within BISS.
- Organisations are **in transition**. Finance moved first. Small and medium enterprises may lack the resources for responsive security.
- **Persuading senior managers:** inform them with industry losses, attack examples, and safeguard costs. Planning for response is both necessary and expensive. After a major loss, "you don't have to convince them anymore"; before it, the security leader is effectively selling.
- **Use in cases:** Horizon's IT was in the BISS paradigm (availability, prevention, compliance) and FC Design behaved like the warfare paradigm. This supports an insight on mismatch between controls and adversary.

### Lim — Information Assurance and Enterprise Security Risk Management (2018)

- Treat information security as arising from a **business issue**, and IT risk as part of **holistic enterprise risk management**.
- If the organisation is digitised there is an IT component. If it is manual, it is a **process issue**.
- As digitalisation increases, revisit the organisation's **posture**: identify, then protect.
- Emphasise **resilience** and how quickly the organisation can **detect and remediate**.
- Attacks are "a matter of time", so have a **cyber response plan** (the transcript abbreviates this as "CBRP").
- **Use in cases:** supports arguments that security belongs under enterprise risk, and that response planning is a core requirement.

### Yuen — Security Analytics (2018)

- Everyone has **normal behaviour**. Analytics learns the pattern and flags abnormal actions.
- Attackers who take over accounts **do not fail the login**. They already hold valid credentials, and may pass two-factor authentication.
- Analytics acts as an **early warning** and prompts the question "is this really the user?"
- **Use in cases:** insider copying by authorised staff, or a privileged account used by an attacker (Horizon Scenes 4 and 14). Links to Week 5 anomaly detection. Limits: it triggers review, not proof, and needs people to respond.

### Yuen — Investment in Cyber Security Initiatives (2018)

- Key investments: data loss prevention and data protection; security incident monitoring and response.
- Organisations focused too much on **protection** ("locking your doors") and too little on **monitoring and response**. Security needs all three.
- Investment is moving to **security operations centres** to detect activity, understand what people are doing, and get early warning.
- **Use in cases:** Horizon had protection (firewall) but little internal monitoring or response structure.

### Yuen — Ransomware in Malaysia in 2017 (2018)

- 2017 was called the **year of ransomware**. It hit hospitals, airports, port terminals, and car manufacturers, not only end users.
- Ransomware is a **symptom of missing basic controls**. WannaCry had a patch available before it spread.
- Lesson: take **patching and host security** seriously across laptops, desktops, and servers.
- **Use in cases:** supports a recommendation on patching and hygiene, and an insight that unpatched systems are a vulnerability. It also echoes Jordan's plan to look for unpatched systems.

### IP Commission Report (Blair & Huntsman, 2013) — Selected Points

This is a US policy report supplied as extra reading, so use it for support rather than as the course definition.

- IP theft loss is estimated in the **hundreds of billions** of dollars per year (Commission on the Theft of American Intellectual Property, 2013, p. 2).
- IP can be stolen by cyber means and by **traditional** means: bribed or planted employees, employees who leave and share information, and long supply chains (pp. 10–12).
- Trade-secret theft runs mainly through **industrial and economic espionage** and **cyber espionage** (p. 39).
- **Economic espionage** benefits a foreign government. **Trade-secret theft** benefits an individual or organisation (p. 41).
- A Ford employee copied about 4,000 documents shortly before leaving for a Chinese carmaker (pp. 41–42).
- Targeted attackers often go after **lower-level employees** who may lack sensitive access but are easier to compromise (pp. 44–45).
- **Vulnerability mitigation** works against opportunistic hackers. **Threat-based deterrence** aims to raise the attacker's cost and reduce their incentive (pp. 79–80).
- Organisations still need best-in-class defences, **active monitoring**, personnel ready to act, and protection that travels with files such as meta-tagging, beaconing, and watermarking (pp. 80–81).
- **Use in cases:** it supports insights about departing employees, adaptive adversaries, and defences that must match targeted attackers.

## Distinctions That Appear in Multiple Choice

| Pair | Difference |
| --- | --- |
| Threat versus threat agent | Danger versus the person or event creating it |
| Vulnerability versus vector | Weakness versus route |
| Risk versus risk appetite | Scenario exposure versus acceptable level |
| Residual risk versus risk appetite | What remains versus what is accepted |
| Strategy versus policy | Choices versus rules |
| Policy versus SETA | Directive versus explanatory |
| Authentication versus authorisation | Who you are versus what you may do |
| IDS versus IDPS | Detects and alerts versus can also block |
| Signature versus anomaly detection | Known patterns versus unusual behaviour |
| Surveillance versus detection | Broad awareness versus specific behaviour |
| Prevention versus perimeter | Any blocking versus a boundary approach |
| Education, training, awareness | Why, how, what |
| Compliance versus risk-based | Baseline versus tailored priority |
| Data versus information versus knowledge | Raw, in context, with experience and judgement |
| Resident versus transmitted information | Stored versus moving |
| Explicit versus tacit knowledge | Written down versus held in a person |
| Economic espionage versus trade-secret theft | Foreign-government benefit versus private benefit |

## Last-Hour Checklist

- [ ] Recite the three Section C questions and their marks.
- [ ] Write the C2 triplet template from memory.
- [ ] State facts versus insights in one sentence.
- [ ] Write five root causes from the insight menu.
- [ ] Name the three defence-in-depth functions and give two controls each.
- [ ] List the seven SETA steps.
- [ ] List the four policy conditions.
- [ ] List the nine paradigms.
- [ ] Recall the seven kill chain stages.
- [ ] Recall the three response gaps.
- [ ] Rehearse one recommendation using what changes, how it reduces risk, and who owns it.

## References

Commission on the Theft of American Intellectual Property. (2013). *The IP Commission report*. The National Bureau of Asian Research.

Thompson, E. D., & Kaarst-Brown, M. L. (2005). Sensitive information: A review and research agenda. *Journal of the American Society for Information Science and Technology, 56*(3), 245–257.

Whitman, M. E., & Mattord, H. J. (2022). *Principles of information security*. Cengage.
