# Week 03 Lecture

Course: [[Cyber Security Management (ISYS90090)/Course Overview|Cyber Security Management (ISYS90090)]]
Week: 03
Topic: Understanding the Cyber-Threat Landscape

## Source Material

- 2026 Canvas Module 3 pages 3.1, 3.2, 3.4, and 3.5, supplied on 11 August 2026.
- [[Cyber Security Management (ISYS90090)/Assets/Week 03 - Threat Actors and Attacks Transcript.vtt|Week 03 lecture transcript]] supplied on 11 August 2026.
- [[Cyber Security Management (ISYS90090)/Assets/Week 03 - Threat Landscape Slides.pdf|Week 03 threat landscape slides]]. The deck dates from 2024, so the 2026 Canvas module takes priority where course details differ.
- Whitman and Mattord (2022), *Principles of Information Security*, pp. 34–74. This is the prescribed reading, but the textbook extract is not stored in the workspace.
- [[Cyber Security Management (ISYS90090)/Week 03/Tutorial|Week 03 Horizon teaching case tutorial]].

## Intended Learning Outcomes

- Identify a range of information security threat actors.
- Identify common cybersecurity attacks on organisations.
- Distinguish a threat, threat agent, vulnerability, vector, attack, and impact.
- Explain how threats may act and how an organisation can reduce the related risk.

## Topic Map

`Asset → threat and threat agent → vulnerability and vector → attack → impact → controls`

Week 2 introduced assets, threats, vulnerabilities, and controls. Week 3 examines the threat side in more detail. It asks who or what can cause harm, how the harm may occur, and what the organisation should do before and after an incident.

## Core Terms

| Term | Course meaning | Key question |
| --- | --- | --- |
| Asset | Information, knowledge, systems, devices, or other resources that have value. | What needs protection? |
| Threat | An object, person, or entity that poses an ongoing danger to an asset. | What could cause harm? |
| Threat agent or actor | The person, group, event, or process that creates the impact. | Who or what acts? |
| Vulnerability | A weakness that a threat agent can exploit. | Which weakness makes harm possible? |
| Attack vector | The route or method used to reach and exploit the target. | How does the attack reach the asset? |
| Attack | An action in which a threat agent exploits a vulnerability and creates an impact. | What harmful action took place? |
| Impact | The harm caused to the organisation or asset. | What was lost, changed, stopped, or damaged? |
| Control | A measure that prevents, limits, detects, or helps recovery from harm. | How will the organisation reduce the risk? |

A threat can exist without an attack. An attack occurs when a threat agent acts through a weakness and causes harm.

### Extra Materials: Direct Example

- **Asset:** Payroll database.
- **Threat:** Unauthorised access and theft of staff data.
- **Threat actor:** A criminal group.
- **Vulnerability:** No multi-factor authentication and weak staff checks of login pages.
- **Vector:** A phishing email linked to a fake login page.
- **Attack:** The group steals a password, signs in, and copies payroll records.
- **Impact:** Loss of confidentiality, possible fraud, legal work, and loss of trust.
- **Controls:** Multi-factor authentication, staff training, email filtering, access limits, login alerts, and an incident response plan.

## Why Precise Threat Scenarios Matter

The lecturer stressed that an organisation cannot defend against an abstract risk. Managers must name the exact asset, actor, weakness, vector, and impact before they can choose a suitable control.

Two scenarios may contain the same actor and asset but need different controls because the weakness differs. For example:

- An attacker exploits a weak password. The organisation needs stronger authentication and password controls.
- The same attacker uses an active staff member's valid account. The organisation needs access limits, behaviour monitoring, review of unusual use, and clear ownership.

Broad terms can hide this difference. Each asset–threat actor–vulnerability combination forms a separate risk scenario, though managers may group scenarios that need the same treatment.

## Threat-Actor Motives

The lecture identifies several reasons why actors target organisations:

- **Extortion:** Block access or threaten disclosure to force payment.
- **Resource or information theft:** Take data, computing resources, money, or other assets.
- **Revenge:** A current or former insider acts because of a real or perceived grievance.
- **Indirect access:** Attack one organisation because it has a trusted link to the intended target.
- **Competitive gain:** Steal information or knowledge needed to copy a product, process, or capability.
- **National-security aims:** Disrupt a state, defence supplier, central bank, critical service, or related supply chain.

The motive affects the defence. A financially motivated group may leave when attack costs become too high. A team funded by a determined sponsor may be replaced when it fails, so the defender must understand and address the sponsor's aim rather than focus only on each attacking team.

## Threat-Actor Taxonomy

The lecturer uses the following set of distinctions:

1. **Accidental or malicious:** A careless employee differs from an actor who intends harm.
2. **Ad hoc or organised:** An angry insider or inexperienced attacker acting without a long plan differs from a funded team.
3. **Lower or higher capability:** A loosely organised activist or insider differs from a trained and well-funded cyber team.
4. **Operational or strategic motive:** Some teams attack for their own reward, while others act for a sponsor with a wider aim.

The lecture also places actors on a rough spectrum:

`amateurs → hackers → insiders → advanced persistent threats`

Capability often raises the target's risk, but patience and the ability to learn matter as well. A less skilled actor who studies the organisation and tests its controls may pose more risk than a skilled actor who gives up quickly.

### Advanced Persistent Threat Pattern

The lecturer describes a broad cycle for a well-resourced and persistent actor:

1. Collect intelligence about the target.
2. Study its controls and weak points.
3. Find and exploit an entry route.
4. Gain control and maintain access.
5. Reach the required assets.
6. Complete the objective and target further organisations if needed.

## Attacker–Defender Imbalance

The main lecture theme is that attackers hold several built-in advantages:

- They choose when, where, and how to attack.
- They choose how long to prepare before the defender sees the first sign.
- They know the target, while the target may not know who they are.
- They can focus their full team on one operation, while a large firm cannot turn every employee into one joined defence team.
- They may attack from anywhere with network access.
- Harmful code can spread in seconds while human decisions and firm-wide action may take days or longer.
- Modern firms have large and sometimes unknown attack surfaces due to phones, laptops, cloud services, suppliers, and unreported technology use.
- Creating harmful code may cost time and money, but copying and distributing it costs very little.

Defenders also face compliance work, limited budgets, staff shortages, and a lack of specialist skills. This helps explain why cyber spending and the number of incidents can rise at the same time.

The lecturer therefore argues that security must cover the whole organisation. A capable attacker may avoid strong digital controls and seek help from an insider, contractor, partner, or user with valid access.

## Categories of Threat

The course uses the following categories from Whitman and Mattord.

| Category | Course examples | Main concern |
| --- | --- | --- |
| Compromise to intellectual property | Piracy and copyright infringement | Loss or misuse of protected ideas, designs, code, or creative work |
| Software attacks | Viruses, worms, macros, and denial of service | Harmful code or traffic attacks systems and services |
| Deviation in quality of service | ISP, power, or WAN provider issues | A supplier provides less service than the organisation needs |
| Espionage or trespass | Unauthorised access or data collection | An actor enters a system, site, or information source without permission |
| Forces of nature | Fire, flood, earthquake, and lightning | A natural event damages or stops resources |
| Human error or failure | Accidents and staff mistakes | An unplanned human act creates exposure or harm |
| Information extortion | Blackmail and threatened disclosure | An actor uses control of information to force payment or action |
| Missing or weak policy or planning | No backup and recovery plan before a drive failure | The organisation lacks clear rules, ownership, or plans |
| Missing or weak controls | A network has no firewall control | The organisation lacks a needed safeguard |
| Sabotage or vandalism | Destruction of systems or information | A person deliberately damages an asset |
| Theft | Unlawful taking of equipment or information | The organisation loses physical or information assets |
| Hardware failure or error | Equipment failure | A device fault harms service or data |
| Software failure or error | Bugs, code faults, and unknown loopholes | A software defect creates failure or exposure |
| Technological obsolescence | Old technology | Old systems may lack support, safe updates, or suitable controls |

The table shows why cybersecurity covers more than hackers and malware. Threats may come from people, weak management, failed technology, outside suppliers, or natural events. They may also be internal or external, and deliberate or accidental.

## Incident, Trigger, and Process

The 2026 Canvas module asks students to analyse incidents in three parts.

### Incident

Describe what happened using the five Ws:

- What happened?
- Who was involved?
- Where did it happen?
- When did it happen?
- Why did it happen?

### Trigger

State the rule, event, or condition that makes the event a security incident. A trigger may depend on the sensitivity of the asset, the person's authority, the location, or an act such as reading, copying, changing, removing, or sharing it.

### Process

State the controls that should prevent, detect, limit, or help the organisation respond to the event.

The Canvas example concerns a sensitive clinical-trial document left in a coffee room. A contractor reads it and removes it. The event becomes a violation when an unauthorised person reads restricted material, or when a document that must remain on site leaves the premises. Suggested controls include clear labels, document checks, RFID tags, and tracking.

The example also shows the need for layered controls:

- A clear handling policy tells staff what they must do.
- Training helps staff understand labels and reporting steps.
- Physical and technical controls help detect or block removal.
- Response steps define who must act after a document goes missing.

## Information Security Attacks

The course defines an attack as an action in which a threat agent exploits a system vulnerability and creates an impact. The attack is the realised event, while the threat is the ongoing danger.

The lecturer also uses **attack** in a broad security sense for a harmful pattern of events, even when no person intended the harm. A fire, flood, failed provider, or staff mistake may still attack the availability or integrity of an asset. Intent remains important when profiling the cause and predicting what may happen next, but the organisation must still manage the harmful event.

### Attack Replication Vectors in the Course

| Vector | Course description in plain English |
| --- | --- |
| IP scan and attack | An infected system scans addresses, finds known flaws, and attacks exposed systems. |
| Web browsing | An infected system changes website files so that visitors may become infected. |
| Virus | Harmful code copies itself into files on systems it can access. |
| Mass mail | An infected system sends harmful email to contacts and spreads through other users. |
| Simple Network Management Protocol (SNMP) | An attacker uses known or common device-management passwords to gain control; updates have closed many old flaws. |

These examples focus on how harmful code spreads. The 2026 module summary also names malware, social engineering, phishing, ransomware, and insider threats. These threats exploit technical flaws, weak processes, trust, access rights, or human behaviour.

### Testing Technology Before Use

The lecturer used a bank example to show how firms may test software in a separate environment before placing it into live use. He also described using controls from several vendors so that one vendor's weakness or an attacker's knowledge of one product does not expose the full defence. Treat this as a lecture example rather than a verified account of one bank's current practice.

## How Organisations Should Respond

For each risk scenario, managers should:

1. Name the exact asset and why it matters.
2. Identify the threat and likely threat actor.
3. Find the vulnerability and possible attack vector.
4. State the likely attack and its impact on confidentiality, integrity, availability, and the business.
5. Choose formal, informal, technical, and physical controls that match the risk.
6. Define signs that should trigger an incident response.
7. Set ownership, reporting, recovery, and review steps.

A useful answer should link each control to the weakness or stage it addresses. A list of security products does not show why the controls fit the risk.

## Exam and Quiz Use

### Principle of At Least Three

The lecturer recommends giving at least three correct and distinct points or examples when an exam question allows it. One correct example could be chance, and two could be coincidence. Three sound examples give stronger evidence that the student understands the concept and can apply it across cases.

Treat this as an exam-answer guide rather than a formal cybersecurity principle. Each point must still be relevant, correct, and explained where the question requires it. If a question asks for a set number of points, follow that instruction.

For a short case, use this answer structure:

> The main asset is ____. The threat actor is ____, and the ongoing threat is ____. The actor uses ____ as the vector and exploits ____. The attack causes ____ impact, mainly affecting ____. The organisation should use ____ controls because they address ____.

Common errors include:

- Calling the attacker the threat instead of the threat agent.
- Calling a weakness an attack vector.
- Naming malware without explaining the asset, weakness, or impact.
- Treating all threats as external and deliberate.
- Suggesting one technical control without policy, training, ownership, detection, or recovery.

## Admin Note

The old slide deck mentions a Week 3 workshop quiz. The 2026 assessment schedule places Quiz 1 in the Week 4 workshop on Tuesday 18 August 2026. Follow the current Canvas schedule.

## Reference

Whitman, M. E., & Mattord, H. J. (2022). *Principles of information security*. Cengage.
