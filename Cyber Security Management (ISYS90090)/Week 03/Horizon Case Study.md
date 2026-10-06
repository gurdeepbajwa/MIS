# Horizon Case Study — Scenes 1–14

Course: [[Cyber Security Management (ISYS90090)/Course Overview|Cyber Security Management (ISYS90090)]]
Introduced: Week 03
Type: Tutorial and exam case-analysis reference

## Source Material

- [[Cyber Security Management (ISYS90090)/Assets/Week 03 - Horizon Teaching Case Complete Canvas.txt|Complete 2026 Canvas Horizon teaching case, Scenes 1–14]].
- [[Cyber Security Management (ISYS90090)/Week 03/Lecture|Week 03 threat landscape lecture]].
- [[Cyber Security Management (ISYS90090)/Week 03/Tutorial|Week 03 tutorial]].
- [[Cyber Security Management (ISYS90090)/Week 04/Tutorial|Week 04 tutorial]].

## Purpose

The case follows a planned campaign by FC Design to obtain Horizon Automotive's designs, commercial information, production knowledge, and staff capability. It provides a continuing case for applying threat, asset, control, management, risk, strategy, policy, culture, and incident-analysis concepts.

The case should support skill transfer to a new exam case. Do not rely on memorising its names or plot.

## Whole-Case Map

`strategic aim → intelligence collection → technical and human access → information and knowledge theft → missed warnings → business harm → diagnosis and management reform`

## Scene Reference

| Scene | Main event | Strong insight | Main course links |
| ---: | --- | --- | --- |
| 1 | Horizon loses a contract to FC Design, which offers a similar car at a lower price. | A business loss may reveal a security failure before the firm understands the attack. | Business impact, warning signs, competitive threat |
| 2 | Horizon links FC Design to Emil, a former R&D engineer, and checks his past access. | Valid staff access may support an insider attack when used for an unauthorised purpose. | Insider threat, intellectual property, access monitoring |
| 3 | FC Design hires Oliver to collect designs, suppliers, material prices, and other intelligence. | The operation has a strategic sponsor, clear objective, funding, and long time horizon. | Espionage, sponsor versus operator, threat motive |
| 4 | Emil copied files, but Horizon lacks need-to-know rules and ownership beyond IT systems. | Horizon treats information security as IT security and leaves paper, people, knowledge, and information without clear ownership. | Four roles of information security, governance, information versus IT security |
| 5 | Horizon links the insider, finance-network intrusion, and physical visit. | Separate incidents form one patient campaign, but siloed teams fail to join the evidence. | TTPs, threat intelligence, incident sequence, situational awareness |
| 6 | Jordan plans several entry routes, custom malware, backdoors, persistence, and theft. | A capable attacker changes methods and uses several paths rather than depend on one flaw. | Attack vectors, attacker–defender imbalance, advanced persistent threat |
| 7 | Leaders diagnose systemic flaws and appoint an enterprise-wide Chief Security Officer. | IT-focused metrics and compliance gave false assurance because no one managed knowledge leakage across the firm. | Strategy, governance, CISO or CSO, SETA, cross-team ownership |
| 8 | Jordan maps Horizon, enters through a fake antivirus update, and finds an air-gapped R&D network. | Human trust can bypass perimeter controls, while asset separation can still limit an attacker's reach. | Reconnaissance, phishing, malware, social engineering, air gap |
| 9 | Oliver advises FC Design to recruit a Horizon engineer after technical access fails to reach R&D. | Threat actors may shift from systems to people when knowledge or offline assets remain out of reach. | Insider recruitment, knowledge leakage, adaptive adversary |
| 10 | Karim identifies Horizon's main asset as its capability and specialised knowledge, not each completed car. | Poor asset definition leads to weak security; competitive capability sits across information, people, judgement, processes, and tools. | Assets, tacit and explicit knowledge, people–process–technology |
| 11 | Karim rejects Horizon's single perimeter and starts with the intelligent adversary and risk. | Defence must match the actor, objective, and TTPs rather than apply a standard perimeter to every organisation. | Security strategy, risk-led controls, monitoring, defence in depth |
| 12 | Horizon's last risk assessment was three years old, treated IT as one asset, used broad risks and gut-feel ratings, and lacked information classification. | A stale and vague assessment cannot identify, rank, or treat specific knowledge-leakage risks. | Risk identification, likelihood, impact, classification, review |
| 13 | Horizon's policy is old, technical, unreadable, held by IT, and unknown to other leaders. | A policy cannot guide behaviour if it is inaccessible, outdated, narrow, and disconnected from strategy and business ownership. | Policy hierarchy, communication, review, formal and informal controls |
| 14 | Jordan combines online research, targeted denial of service, phone pretexts, identity use, vendor impersonation, and a malicious update. | The breach is a staged social and technical sequence; each event supplies information or access for the next step. | Attack chain, TTPs, social engineering, privileged access, detection |

## Detailed Analysis: Scenes 4–9

Quick revision: [[Cyber Security Management (ISYS90090)/Week 03/Horizon Scenes 04-09 - Quick Reference|Horizon Scenes 04–09 — Quick Reference]].

### Scene 4 — Information Security Ownership

#### Facts

- Emil copied hundreds of files shortly before leaving.
- Horizon had already briefed Anders, but another business issue took priority.
- Emil held authorised R&D access.
- Horizon had no need-to-know policy.
- IT did not know which server information was sensitive.
- Paper files and staff conversations sat outside IT's stated role.

#### Insight

Horizon has no enterprise owner for information and knowledge security. It grants access by team and system but does not govern how authorised people use, copy, combine, or transfer valuable content.

#### Needed response

- Assign business owners to information and knowledge assets.
- Classify sensitive content.
- Apply need-to-know and least-privilege access.
- Monitor unusual copying and access behaviour.
- Join HR departure processes with business, legal, physical, and cyber-security checks.

### Scene 5 — One Campaign, Several Events

#### Facts

- Emil could reach R&D designs but not finance data.
- A prior zero-day intrusion spent time inside the finance network.
- FC Design representatives visited Horizon, asked detailed questions, and took photographs.
- Teams recorded these events but did not connect them.

#### Insight

FC Design ran a long-term campaign through insider, cyber, physical, and relationship channels. Horizon's teams saw separate events rather than one threat actor pursuing one strategic objective.

#### Needed response

- Combine incident, access, HR, physical-security, legal, and business reports.
- Use threat intelligence to link motive, sponsor, targets, and TTPs.
- Set triggers for escalation when several events involve the same asset or actor.

### Scene 6 — Planned Technical Intrusion

#### Facts

Jordan considers unpatched flaws, executive laptops, VPN access, wireless access, network errors, devices, zero-days, custom malware, and several backdoors.

#### Insight

The attacker is funded, adaptable, and persistent. Closing one route will not end the risk because the objective remains and the attacker can change vectors.

#### Needed response

- Patch and test systems.
- Limit privileged and remote access.
- Separate networks and monitor movement between zones.
- Monitor behaviour rather than rely only on known malware signatures.
- Plan detection, containment, recovery, and investigation.

### Scene 7 — Systemic Management Failure

#### Facts

- Horizon has no leakage-mitigation strategy.
- It has a history of misdirected contracts and staff copying data to personal devices.
- IT reports strong availability, standard controls, access records, and compliance.
- Annual training covers technical events but not knowledge leakage.
- Teams rarely compare security information.
- Horizon appoints a Chief Security Officer with enterprise-wide responsibility.

#### Insight

Horizon optimised IT operations and compliance but did not manage the business risk of losing its competitive capability. The central problem is not the absence of all controls; it is poor direction, scope, ownership, and coordination.

#### Needed response

- Define an organisation-wide leakage strategy.
- Give a senior security leader clear authority and access to business decisions.
- Expand security beyond systems to data, information, knowledge, paper, devices, people, and partners.
- Train staff to recognise and report behaviour linked to key business risks.
- Review incidents across functions rather than within one team.

### Scene 8 — Reconnaissance, Entry, and the Air Gap

#### Facts

- Jordan maps systems, software, staff roles, usernames, access, and files through technical tools and public sources.
- He can map the supply chain and reach finance records.
- R&D designs sit behind an air gap.
- He entered by pretending to supply an urgent antivirus update that contained malware.
- He plans to hide the targeted operation inside a larger visible attack and delete logs.

#### Insight

Jordan uses public information and staff trust to defeat the boundary controls. The air gap limits his direct reach, but it does not protect knowledge held by employees or prevent a shift to a human route.

#### Needed response

- Verify vendors and updates through a trusted channel.
- Restrict who can install software and updates.
- Monitor privileged actions and retain protected logs.
- Limit public exposure of staff roles and system details.
- Protect offline assets through staff, visitor, device, and insider controls.

### Scene 9 — Recruiting the Missing Capability

#### Facts

- The attacker can obtain finance information but not the offline engineering files.
- Oliver recommends recruiting Horizon engineers rather than forcing the technical route.
- He profiles employees and selects one likely to accept an offer.

#### Insight

FC Design needs both explicit information and practical knowledge. When technical controls block one asset, the operation targets a person who can carry or recreate the missing capability.

#### Needed response

- Identify staff who hold rare or high-value knowledge.
- Reduce single-person dependence and document transferable knowledge where possible.
- Strengthen departure, conflict-of-interest, confidentiality, and access-review processes.
- Monitor unusual copying without treating every departing employee as malicious.
- Improve retention and provide safe ways to report recruitment or coercion attempts.

## Detailed Analysis: Scenes 10–14

### Scene 10 — The Real Asset

Horizon first identifies its cars as the asset. Karim corrects this: the lasting asset is the capability to design and build cars customers will buy. That capability includes technical information, engineering experience, judgement, values, production methods, tools, supplier knowledge, and staff practice.

The key lesson is to define the asset at the level that creates business value. Protecting files alone cannot protect a capability spread across people, processes, and technology.

### Scene 11 — Strategy Must Match the Adversary

Horizon has an air-gapped R&D network but relies on one outer boundary for much of the firm and does not monitor internal activity. Standard controls may suit common outages or automated attacks, but FC Design is an intelligent actor that studies the target and adapts.

The key lesson is that control selection begins with the exact risk. Horizon needs internal monitoring, network separation, several control layers, and a strategy aimed at the theft of capability rather than only service availability.

### Scene 12 — Weak Risk Assessment

Horizon treats all IT as one asset, names only a few broad risks, rates likelihood and impact through group judgement, has not completed a formal assessment for three years, and does not classify information.

The key lesson is that vague inputs produce weak priorities. Horizon must identify specific assets and risk scenarios, use evidence for likelihood and impact, record assumptions, classify information, assign owners, and reassess when assets, threats, processes, or controls change.

### Scene 13 — Policy Without Organisational Effect

Horizon has many technical policies, but the main binder is old, hard to read, kept by IT, and unknown to business leaders. It relies on commands and penalties without a clear link to Horizon's knowledge risk or current strategy.

The key lesson is that a formal document does not become an effective control merely because it exists. Policy needs senior ownership, clear language, access, communication, SETA support, procedures, standards, review, and controls that enforce its direction.

### Scene 14 — Full Attack Sequence

Jordan's route is:

1. Map Horizon's public and digital footprint.
2. Choose a trusting employee and a privileged IT worker.
3. Cause a targeted denial-of-service problem.
4. Impersonate a service provider and collect an employee ID.
5. Use that identity to report a fake infection to IT.
6. Place a false public notice about the invented malware.
7. Impersonate the antivirus vendor and send a malicious update.
8. Cause the privileged IT worker to install the malware.
9. Open a remote connection with high privileges.

The key insight is that no single event explains the breach. The attacker creates a believable sequence in which each social and technical step prepares the next one.

## Cross-Scene Root Causes

- Horizon defines security too narrowly as IT availability and boundary defence.
- It fails to identify specialised knowledge and competitive capability as assets.
- It lacks a strategy for knowledge leakage.
- Business, HR, IT, legal, physical security, and R&D work in silos.
- It records warnings but does not link them into a threat picture.
- Risk assessments are stale, broad, subjective, and incomplete.
- Policy exists but does not guide the organisation's actual security behaviour.
- Training covers routine technical events rather than Horizon's main business risks.
- Controls do not match a funded, intelligent, and adaptive adversary.

## Exam Answer Structure

1. State two or more relevant case facts.
2. Infer the root problem or insight those facts support.
3. Name the asset, actor, motive, vulnerability, vector, and impact.
4. Explain why current management practices or controls failed.
5. Recommend actions that address the root cause and urgent symptoms.
6. Link each action to strategy, risk, policy, SETA, governance, or technology as relevant.

Use this form:

> The case states **[facts]**. Together, they show **[root problem]** because **[reasoning]**. This exposes **[asset]** to **[actor and risk]**, causing **[impact]**. Horizon should **[response]**, supported by **[matching management practice or control]**.

## Source Limits

- The story is fictional and designed for teaching.
- Treat technical claims in character dialogue as part of the case, not as verified current security guidance.
- Use the exact weekly question when deciding which scenes and concepts to apply.
