# Horizon Question Workbook — Facts and Insights

Course: [[Cyber Security Management (ISYS90090)/Course Overview|Cyber Security Management (ISYS90090)]]
Type: Exam practice reference and how-to
Source case: [[Cyber Security Management (ISYS90090)/Assets/Week 03 - Horizon Teaching Case Complete Canvas.txt|Horizon Teaching Case, Scenes 1–14]] with the Canvas "Text Version with Questions" prompts
Related: [[Cyber Exam Study Guide - Section C]], [[Cyber Security Management (ISYS90090)/Week 03/Horizon Case Study|Horizon Case Study analysis]]

## How to Use This Workbook

1. Read a scene and its question. **Answer from memory first.**
2. Check the **Facts** column: these are things the case writes down.
3. Check the **Insight**: this is what you must infer by linking facts.
4. Rewrite the answer in your own words using the course terms.

The lecturer's rule applies here: **if the case writes it, it is a fact. An insight is derived.** The case has dialogue, so treat character opinions (for example Kurt's claim that this is "not our area") as facts about what he said, not as proven truth.

Questions are quoted in short form. Model points are guides, not a mark scheme.

## Whole-Case Timeline

The exam case may not be in date order. Practise rebuilding order from clues.

| Order | Event | Scene | Timing label in the case |
| ---: | --- | --- | --- |
| 1 | FC Design meets Oliver in Dubai and commissions intelligence on Horizon's next-generation project | 3 | "A few years prior to the present" |
| 2 | Visit by a delegation including FC Design; staff ask detailed questions and take photos | 5 | "a couple of years ago" |
| 3 | Zero-day attack on Swedish firms, with attackers spending most time in Horizon's finance network | 5 | "July 2 years ago" |
| 4 | Jordan researches Horizon, phones staff, gets malware installed, finds the air gap; Oliver proposes recruiting an engineer | 6, 8, 9, 14 | "Recent past" |
| 5 | Emil copies files weeks before leaving for FC Design | 2, 4 | Left "about a year ago" |
| 6 | Horizon loses the contract and starts investigating | 1, 2 | Present (1 March) |
| 7 | Horizon links the events, diagnoses the failures, and appoints a CSO | 5, 7 | Present |

The case does not state how Jordan's "recent past" work lines up against the zero-day attack or against Emil's departure, so treat ordering within rows 3–5 as an **inference from labels**. Scenes 2 and 4 place Emil in R&D, but Scene 10 says the leaver was a manufacturing engineer. This is an inconsistency in the case, so avoid building an argument that depends on which team he was in.

---

## Scene 1 — What Is Going Through Anders' Mind?

**Facts**

- Erik says Horizon will not receive the NextGen order.
- Horizon is the only performance-car maker in the country.
- The new supplier is not a European firm, offers a price Horizon "won't be able to match", and has cars with "a faint resemblance" to Horizon's.
- Anders asks Patrick to investigate FC Design.

**Insight**

A lost contract can be the first visible symptom of a hidden security failure. Anders is moving from "we lost on price" to "someone has obtained our product knowledge".

**Answer points**

- Shock and a sense of threat to market position.
- Suspicion of intellectual property leakage (an inference): a rival with no hypercar history offers a similar-looking product at a price Horizon cannot match.
- Realisation that Horizon did not know it had a competitor.
- Urgency to identify the actor, which is a **threat intelligence** step.

## Scene 2 — What Is Going Through Anders' Mind?

**Facts**

- Photographs show the "spitting image" of a car still under development.
- Only the R&D team and Anders had seen the design.
- FC Design hired an R&D engineer, Emil, about a year earlier.
- Anders asks the IT manager to review R&D logs.

**Insight**

The leak is likely an **insider route**, which technical perimeter defences do not address. Anders is trying to connect a departed employee to the theft, but he is still working from logs rather than a prepared response plan.

**Answer points**

- Anger and disbelief, because the design was held within a small trusted group.
- Hypothesis: Emil took or carried the design.
- Next step: gather evidence from logs. That is **detection after the fact**, which shows weak real-time monitoring.

## Scene 3 — The Meeting in Dubai

**Question set:** What is the meeting about? What can we deduce about Oliver's profession? Describe FC Design's strategy. Why Oliver? Describe and distinguish this category of threat.

**Facts**

- The client uses a pseudonym ("John"), gives a business card with no name, hands over an envelope with a payment figure, and asks for designs, part specifications, supplier names, and raw-material pricing.
- FC Design's incoming CEO wants to compete in the hypercar market in ten years.
- FC Design has finance, factory space, and an engineering workforce but lacks the higher-order hypercar capability.
- Its engineers visited Horizon's manufacturing division and were impressed.
- Oliver reads the payment figure ("Excellent") and commits the card's contact details to memory.

**Insight**

FC Design chose to **buy a shortcut to capability** instead of building it over decades, and used an intermediary to keep deniability and access specialist skills. This is a **sponsored, strategic, patient campaign**, not an opportunistic hack.

**Answer points**

| Question | Strong points |
| --- | --- |
| What is the meeting about? | Commissioning industrial espionage against a named competitor and project. |
| Oliver's profession | Corporate intelligence broker or spy-for-hire who recruits technical operators; works through intermediaries; discreet and mobile. |
| FC Design | Mid-range Asian passenger-vehicle maker with scale, money, and engineering skills, but no hypercar know-how; strategic objective is entry into a high-margin market in ten years. |
| Shift the landscape | Obtain designs and supply-chain data to skip R&D and negotiate lower material costs, then undercut the incumbent. |
| Why Oliver? | Deniability, specialist skills, and distance between FC Design and the crime. |

**Threat category and distinction**

- Category: **espionage or trespass**, with **compromise to intellectual property** as the target (Whitman and Mattord categories, Week 3).
- Actor type: **organised, malicious, strategic** with a **sponsor**. It fits the **advanced persistent threat** pattern: collect intelligence, study controls, enter, maintain access, reach assets, complete the objective.
- How it differs from other threats:

| Threat | Motive | Typical behaviour | Contrast with FC Design |
| --- | --- | --- | --- |
| Opportunistic or ransomware criminals | Quick money | Scan broadly, leave if costly | FC Design does not give up because the objective is strategic |
| Insider with a grievance | Revenge | Ad hoc, internal | FC Design is organised and funded |
| Hacktivist | Ideology | Public disruption | FC Design wants silence and advantage |
| Accident or human error | None | Unplanned | FC Design is deliberate |

Key distinction from Week 3: when the sponsor's aim is strategic, defeating one attacking team does not help because the sponsor can hire another. Defend against the **sponsor's objective**.

**Extra Materials — economic espionage versus trade-secret theft (IP Commission)**

US law distinguishes economic espionage (benefit to a foreign government or agent) from trade-secret theft (benefit to an individual or organisation); the key difference is **who benefits** (Commission on the Theft of American Intellectual Property, 2013, p. 41). Horizon's case is closer to commercial trade-secret theft by a competitor. This is a US legal distinction, so use it only as supporting context.

## Scene 4 — Why Is This Not "Information Security" for Kurt?

**Question set:** Why does Kurt think this is not an information security incident? What is his team's role? Which term best applies? Short-term cost? Long-term cost?

**Facts**

- Emil copied hundreds of files from the NextGen server weeks before leaving.
- Kurt says his team "maintain[s] the availability of IT systems and networks".
- Kurt says IT has no idea what information is stored or sensitive, and there is no need-to-know policy.
- Emil had authority to access the files.
- Asked who secures paper files and phone conversations, Kurt answers "Ummm… everybody", which Anders reads as nobody.
- Kurt says Anders was briefed at the time, but a procurement issue (a key supplier's bankruptcy) distracted them.

**Insight**

Horizon has **equated information security with IT availability and technical controls**. That leaves information, knowledge, paper, and conversations with no owner. Emil's access was *authorised*, so a control framework based on "who is allowed in" could not flag him.

**Answer points**

- Kurt's view: IT security means keeping systems running and protected from technical failure. The files were accessed by an authorised user, and IT does not decide what is sensitive.
- IT's role: infrastructure, availability, perimeter tools, access records. It is one of the four roles of information security (safeguard technology assets), not the whole.
- Anders' counter-point: information security covers information in any form and wherever it moves.

**Which term?**

| Term | What it focuses on | Fit |
| --- | --- | --- |
| Computer security | Protecting computers and networks | Too narrow. Matches Kurt's role, not the loss |
| Information security | Protecting confidentiality, integrity, and availability of information resources in any form | Fits. Paper, spoken, and digital information were all involved |
| Information assurance | Information security managed as a business and risk issue, with assurance that risk and controls stay in balance across the organisation | Best fit for a strategic answer, because the failure was ownership and management, not only controls |

Check this table against your Week 1 slide or textbook definitions. The course notes in the workspace do not define the three terms side by side, so the wording above is a reasoned summary rather than a quoted definition. Lim (2018) frames information assurance as a business and enterprise risk issue first, with IT as a component (see [[Cyber Exam Cheat Sheet#Reading and Expert Opinion Takeaways|expert takeaways]]).

**Short-term cost** (visible, near-term)

- Stated in the case (Scene 7): lost contracts, a new design to build "from the ground-up", no new car for at least a few years, and an immediate financial hit in the hundreds of millions of dollars.
- Likely but not stated (inference): incident investigation, legal work, and recovery effort.

**Long-term cost** (competitive, structural)

- A permanent competitor with similar product capability.
- Lower sales volume, market share, and margin.
- Loss of competitive advantage and pricing power.
- Loss of reputation and customer trust.
- Weaker supplier position, because pricing and supplier data are exposed.

Quick rule: **short term = one-off and visible; long term = the market has changed.**

## Scene 5 — Why Could Horizon Not Stop the Leak When Each Incident Was Reported?

**Question:** Relate your answer to the definition of information security and ideas such as risk perception.

**Facts**

- Emil could not reach supplier or pricing data, which sat on the financial network.
- A zero-day attack two years earlier gave attackers time inside the finance network.
- A delegation including FC Design visited, asked specific questions about suspension and propulsion, and photographed. Phones were confiscated, then returned.
- Kurt only now recalls that the incident response team found the attackers spent most of their time in the finance network, and that he would need to cross-reference logs and addresses to know what was copied.
- Lena only now learns from physical security that the visiting delegation listed FC Design.
- Anders says (Scene 7): "every incident was reported" but Horizon "failed to link the incidents".

**Insight**

Horizon **perceived each incident as a low-level, separate event** because no one defined security as protecting the organisation's competitive knowledge. Without that definition, signals that were visible to different teams did not add up to a risk. Reporting is not the same as **situation awareness**.

**Answer points**

- Information security protects information and knowledge resources against harm to confidentiality, integrity, and availability, across the whole organisation, using formal, informal, and technical controls.
- **Risk perception** depends on knowing the asset's value and the actor's intent. Horizon did not know the crown jewels or who wanted them, so each incident looked minor.
- Silos: IT saw the intrusion, physical security saw the visit, HR saw the departure, the business saw the lost contract.
- No one asked "who is behind these, and what do they want?" That is **threat intelligence**.
- FC Design acted **deliberately, systematically, and patiently** over three to five years (Anders' reading in the case). The attacker's patience beat the organisation's attention span.

## Scene 6 — Jordan's High-Level Game Plan

**Facts**

- Jordan will look for unpatched systems and weak firewalls.
- Alternatives: hijack an executive laptop, use a VPN, create a Wi-Fi access point, exploit a wiring fault, or use a photocopier.
- Worst case: buy a zero-day and build custom malware in small pieces.
- A unique weapon will not match IDS signatures.
- He will install backdoors in many places and then "take the information".
- Buying a zero-day vulnerability is quoted at $5,000 to $250,000.

**Insight**

The attacker has **several independent routes** and can adapt, so closing one vulnerability does not end the risk. Defence must target the **attacker's objective and persistence**, not one weakness.

**Answer: steps to get the information**

1. Reconnaissance: map systems, patch levels, firewalls.
2. Select the easiest entry route (vulnerability, then human or wireless routes, then zero-day).
3. Build or buy the weapon and avoid known signatures.
4. Deliver and exploit.
5. Install multiple backdoors for persistence.
6. Move to the target data and copy it.

Map to the **cyber kill chain**: reconnaissance → weaponisation → delivery → exploitation → installation → command and control → action on objectives.

## Scene 7 — Management Meeting

**Question set:** Respond as IT Director. Why is awareness training ineffective? What qualities does a CSO need, and what remains after appointing one?

**Facts**

- Lisa: Horizon has no leakage-mitigation strategy and has faced court action over leaked contracts, personal-device downloads, and misdirected email.
- Kurt: >90% availability, firewalls, IDS, antivirus, access spreadsheet, incident response team, compliance with best practice.
- Gustav says Horizon does security awareness training; Anders replies that it is only once a year and covers IT scenarios such as virus attack and system malfunction.
- Anders: every incident was reported, but they were not linked. Lisa admits teams rarely compare notes, "certainly not about security issues".
- Anders appoints a Chief Security Officer with enterprise-wide responsibility.

**Insight**

Horizon optimised IT service performance and **compliance** and mistook that for security. The real problem is **strategy, scope, ownership, and coordination**.

### As the Director of IT

Strong response structure:

1. **Accept what IT does well** (availability, standard controls, incident response) but admit it addresses technical threats, not knowledge leakage.
2. **Explain the mandate gap.** IT was never asked to identify sensitive information or govern paper and conversations.
3. **Challenge compliance as proof.** Compliance is a baseline (Week 4). Risk assessment adds context. Horizon needs both.
4. **Ask for what IT needs:** business owners to classify information, authority over access reviews, budget for internal monitoring, and a cross-functional forum.
5. **Position IT as a partner** inside a wider programme, not the sole owner.

Avoid sounding defensive. Concede that "information security" is not the same as "IT security" and ask for enterprise governance.

### Why Awareness Training Is Ineffective

| Fact | What it reveals |
| --- | --- |
| Annual only | Not **sustained** (Week 8 design feature) |
| Covers virus and system malfunction | Not tied to Horizon's top risk scenario (knowledge leakage) |
| No way to report what is not known to be a problem | No culture or channel for reporting early signs |
| Same content for everyone | Not **tailored** by role or skill |
| Run by HR (Gustav) and framed around IT scenarios | Inference: no senior ownership and no link to strategy or the main risk |

Link to Week 8: SETA should target identified risk scenarios, follow the seven steps (scope and goals, trainers, audiences, motivate, administer, maintain, evaluate), study culture first, and ask "what's in it for them?"

### Qualities for a CSO

- Business and strategic understanding; can speak to the CEO and board.
- Authority and reporting line to the top (Week 2 survey: reporting lines matter).
- Risk and knowledge-asset thinking beyond IT.
- Cross-functional communication with HR, legal, R&D, physical security, and IT.
- Ability to build policy, strategy, SETA, and response structures.
- Credibility with technical staff, without being only a technologist (Week 4 CISO roles: strategist, advisor, technologist, guardian).

### What Remains After the Appointment

A CSO is a **structural** fix, not a complete one.

- Culture and behaviour still need to change.
- Information owners must be named and classification must be done.
- Risk assessment, policy, and training still need rewriting.
- Technical controls (internal monitoring, segmentation) still need building.
- The adversary is still patient and adaptive.
- A new leader without authority, budget, and CEO backing will repeat the same silo problem.

## Scene 8 — How Far Up the Kill Chain Is Jordan?

**Facts**

- Jordan mapped systems, software versions, usernames, roles, and access levels, partly using social media.
- He scanned drives for keywords and found financial documents.
- He entered through a fake antivirus update containing a virus.
- He says Horizon does not know he is inside.
- He cannot find NextGen designs and concludes there is an air gap.
- He plans to delete logs and make it look like a big attack.

**Answer**

| Kill-chain stage | Status |
| --- | --- |
| 1. Reconnaissance | Done |
| 2. Weaponisation | Done (malware disguised as an update) |
| 3. Delivery | Done (email as antivirus update) |
| 4. Exploitation | Done (update installed) |
| 5. Installation | Done (malware on a Horizon system) |
| 6. Command and control | Done (remote access, mapping the network) |
| 7. Actions on objectives | **Partly done.** Finance data located. Engineering designs not reached. Clean-up still planned |

**Links remaining:** reaching the air-gapped R&D files, which the case shifts to a human route (Scene 9); exfiltration; and hiding evidence. Expect the attacker to **adapt** at the stage that is blocked.

The kill chain is a **model, not a guarantee**: the case does not say how Jordan will complete step 7, so avoid claiming facts beyond the text.

## Scene 9 — Preventing Employees From Leaving and Taking Information

**Facts**

- Oliver suggests offering Horizon engineers a job and hinting that FC Design is "building something amazing".
- He has profiles on employees and says one is "ripe for the taking".
- Emil, a Horizon engineer, was later hired by FC Design (Scene 2).

**Insight**

When technology blocks the route to an asset, an adaptive adversary shifts to **people**. Knowledge that is tacit lives in heads, so a technology-only defence cannot stop it leaving.

**Answer points (by control type)**

| Type | Measures |
| --- | --- |
| Formal | Confidentiality and intellectual property agreements; conflict-of-interest and secondary-employment rules; clear exit procedures with access removal; need-to-know and classification policy; sanctions that are **certain and severe** |
| Informal | Fair pay, recognition, and career paths; a culture where staff report outside job approaches; leaders who model secure handling; SETA on recruitment and approach tactics |
| Technical | Monitoring unusual copying and printing; data loss prevention; compartmentalising crown-jewel files; logging access to critical designs |
| Knowledge management | Document explicit knowledge; reduce single-person dependence; stage access to sensitive design work |
| Intelligence | Watch competitors' hiring and approaches to staff |

Honest limit: you cannot fully stop tacit knowledge leaving with a person. The aim is to **reduce likelihood, limit what is exposed, and detect warning signs**. Avoid treating every departing employee as malicious.

## Scene 10 — Anders' View Versus Karim's View of the Asset

**Facts**

- Anders: the asset is the cars, each worth over $1.5 million.
- Karim points out that Horizon is "giving the cars away" (selling them), so the car cannot be what sustains advantage. The asset is the **capability to make cars the market will buy at the price Horizon sets**.
- Karim says Horizon cars are predominantly hand crafted, more so than Lamborghini or Ferrari.
- Karim: knowledge is "experience and insight… values and judgment" and is embedded in processes, tools, and techniques.
- The stolen designs help FC Design, but Karim says FC Design would need some Horizon engineers on the factory floor to show Horizon practices.
- Anders says the leaver was a manufacturing engineer (note the inconsistency with Scenes 2 and 4, which place Emil in R&D).

**Insight**

Horizon defined its asset **at the wrong level**. The cars are outputs. The value comes from tacit and explicit **knowledge** spread across people, processes, and technology.

**Answer points**

- Anders sees a tangible product; Karim sees an intangible capability.
- Karim's point: information is only part of knowledge. Information is data in context. **Knowledge** adds experience, judgement, and skill (Week 2: explicit versus tacit; Week 11: data, information, knowledge, wisdom).
- Effect on the security programme:
  - Scope widens from IT systems to **people, process, and technology**.
  - Controls must cover how knowledge moves (conversation, paper, digital flows).
  - Protect the people who hold tacit knowledge, not only their files.
  - Define the asset before choosing controls.

## Scene 11 — Strategy Advice for Kurt

**Facts**

- R&D is segregated, but the rest of the organisation depends on one perimeter firewall.
- Horizon does not monitor internal activity.
- The firewall is a common, off-the-shelf product.
- Standard antivirus and password access control.
- Karim: the adversary is "intelligent" and may know Horizon's routines better than Horizon does.
- Karim: "Everything starts with risk."

**Insight**

Horizon built **a castle with one wall and no guards inside**, designed for non-intelligent threats such as accidents and bots. The adversary wants **capability**, not service disruption.

**Strategy advice**

1. **Start with risk.** Identify the crown jewels and the actor's likely paths.
2. **Use threat intelligence.** Profile FC Design's motive, capability, and tactics, techniques, and procedures.
3. **Defence in depth.** Separate (segment the network, internal firewalls, keep the air gap), observe (monitor internal movement, several vantage points), and mediate (identity, need-to-know, least privilege, encryption).
4. **Assume the perimeter will be breached.** Add detection and response.
5. **Include people and process**, not only technology.
6. **Do not rely on obscurity.** Assume the attacker knows your layout.

**Simplest and most effective advice for an under-resourced IT team**

> Identify the few assets that would hurt most to lose, restrict who can reach them, and watch them closely. Spend the limited effort where the loss would be largest.

This applies the Week 9 strategy rule: coordinate limited resources at **least effort and cost while remaining effective**, and keep spending proportionate to the asset's value.

**Extra Materials — IP Commission on vulnerability mitigation**

The Commission distinguishes opportunistic hackers, who move on when defences are tough, from targeted hackers hired to take specific information. It argues that "vulnerability mitigation" (patches, firewalls, updated tools) works mainly against the opportunistic type and is "largely ineffective" against determined targeted attackers, so organisations should add active monitoring and a response capability (Commission on the Theft of American Intellectual Property, 2013, pp. 79–80). This matches Karim's point that Horizon's one-layer castle fits the wrong adversary.

## Scene 12 — Weaknesses in Horizon's Risk Assessment

**Facts (Carl's answers)**

- Risk assessment done by identifying assets in a workshop with security managers.
- Last official assessment three years ago.
- One asset identified: IT systems.
- Four or five risks: system failure, hacker attack, virus outbreak, natural disasters, and one forgotten.
- Likelihood by "gut-feel"; impact rated low, medium, or high by opinion.
- Relies on a standard IT security audit and best-practice standards.
- No classification of information sensitivity.

**Insight**

The process is **perfunctory, ungrounded, and stale**, and it is blind to Horizon's real asset. It generates a plausible-looking ranking that points effort at the wrong problems.

**Karim's concerns and implications**

| Concern | Link to course |
| --- | --- |
| One broad asset, "IT systems" | Coarse granularity; knowledge neglected (Shedden et al., Week 6) |
| Few generic risks, no scenarios | Perfunctory identification (Webb et al., Week 6) |
| Gut feel without evidence | Weak grounding in the actual situation |
| Three years old, no learning from incidents | Intermittent, non-historical assessment |
| Done with security managers only | Business owners and knowledge holders absent |
| No classification | Cannot rate impact or apply need-to-know |
| Compliance audit as the input | Baseline treated as ceiling (Week 4) |

**Outcome (risk exposure)**

- Horizon cannot see its **real risk profile**. Knowledge-leakage and insider scenarios are missing.
- Spending goes to availability threats, not to the most harmful scenario.
- Leaders have **false confidence**, because a completed assessment looks like assurance.
- High residual risk exists but is unknown, unowned, and unmonitored.
- It was therefore reasonable that a patient adversary operated for years without a matching risk entry.

## Scene 13 — Improving the Information Security Policy

**Facts**

- Karim notices the keyhole of his office appears tampered with, with scuff marks.
- A heavy "Information Security Policy" binder sits on his desk.
- Contents: version history, a motherhood opening statement from Anders, many technical policies (acceptable use, email, telecommuting, malware, patching, and so on).
- Long, technical, "You must…" language.
- Anders and Lena both say Kurt has it; Anders does not know how many copies exist.
- The last version was three years ago.

**Insight**

The policy is a **formal control that exists but has no organisational effect**: it is unreadable, unowned by the business, inaccessible, outdated, and aimed at IT systems rather than Horizon's knowledge risk.

**Advice for Anders (Horizon-specific)**

| Problem in the case | Recommendation | Course link |
| --- | --- | --- |
| Held only by IT | Publish through the intranet and onboarding; business heads co-own sections | Dissemination, owner |
| Technical and unreadable | Replace the main document with a short, plain-language enterprise policy and move detail to standards and procedures | Höne and Eloff: styling; hierarchy |
| Opening statement is generic | A signed CEO statement tied to Horizon's actual risk: protecting engineering knowledge and supplier information | Management commitment |
| Focus on IT assets | Add classification, need-to-know, handling of paper and conversations, departing staff, and visitors | Suitability, completeness |
| Three years old | Set review triggers (new threat, incident, restructure) and a review date | Maintenance |
| No link to training | Pair each policy area with SETA and measure behaviour | Policy supported by SETA |
| Commands and penalties only | Explain why, involve R&D and manufacturing in drafting, and enforce uniformly | Four conditions: read, understand, comply, uniform enforcement |

Use the **four conditions** (dissemination, comprehension, compliance, uniform enforcement) and the **policy to standard to procedure to guideline** hierarchy.

**A hidden fact worth using:** the tampered lock suggests a possible physical probe that nobody has reported. This is a **fact** (Karim noticed marks) and an inference of a physical-security gap, but the case does not confirm a break-in. Say so.

## Scene 14 — Jordan's Strategy and SETA

**Facts**

- Jordan builds an organisation chart with photos, phone numbers, and IP addresses from tools, emails, and social networks.
- He chooses Mikael as "the most trusting" and runs a **denial-of-service** attack on Mikael's address.
- He calls as "Ludwig from TeleFon Services", gets Mikael's name and employee ID.
- He calls IT manager Marcus as Mikael, claims a USB from the car park produced a "Tomb Raider" message, and plants a fake virus notice on bugtraq.
- He calls Marcus as "V-Scan", the antivirus vendor, and emails a "virus update" that is malware.
- The malware opens a remote connection with super-user privileges.

**Insight**

Jordan's strategy is **staged social engineering**: manufacture a believable problem, build trust with each call, and exploit people with **authority** (a privileged IT manager). Each step creates the credibility for the next. Human trust beats technical controls.

**How SETA mitigates the risk**

| Step in the attack | SETA response |
| --- | --- |
| Public information used for profiling | **Awareness:** limit what staff post online; explain how profiles are built |
| Pretext caller asks for name and ID | **Training:** verify callers by calling back on a known number; never give identifiers unprompted |
| Staff use a found USB | **Awareness and policy:** treat unknown media as hostile; report it |
| IT manager accepts a vendor update by phone and email | **Training for privileged staff:** verify updates through a trusted channel; install only from approved sources |
| No suspicion of coincidence (outage then call) | **Education:** teach that attackers can *create* the problem they offer to fix |
| No escalation or reporting | **Awareness:** simple, rewarded reporting route |

**Design points from Week 8**

- Use the **seven steps**. Start by studying the current culture: why did Marcus act as he did? Time pressure? Authority? Helpfulness?
- Tailor to **audiences**: general staff, and **privileged IT staff** need specific training.
- Make it **situated and sustained**: realistic simulated calls and repeat exercises.
- Aim above **compliance**: Kelman's three levels are compliance, identification, internalisation.
- Measure behaviour, not completion.

**Limit:** SETA lowers the chance of success but will not stop every call. Pair it with technical controls such as signed updates, least-privilege admin accounts, and monitoring.

---

## A Model Section C Answer for Horizon

Use this to see the three questions answered as a chain. Write your own version from memory before reading it.

### C1: Five Key Insights

1. **Horizon's real asset is its manufacturing and engineering knowledge, not the cars or files.** *Facts:* the cars are hand crafted and sold, Karim says the "how" of making them matters, and he says FC Design would need Horizon engineers to show its practices. *Why it matters:* the security programme protects the wrong object, so leakage of knowledge is not seen as a security event.
2. **Nobody owns information and knowledge security.** *Facts:* IT says it maintains availability; there is no need-to-know policy; paper and conversations belong to "everybody". *Why it matters:* without an owner, no one classifies, monitors, or reacts to copying by an authorised user.
3. **Separate teams saw separate warnings and never joined them.** *Facts:* the visit, the finance-network intrusion, Emil's copying, and the lost contract were each handled alone; Anders says every incident was reported. *Why it matters:* a patient campaign looks harmless in pieces, so the threat picture never formed.
4. **Controls and management practices were built for the wrong adversary.** *Facts:* one perimeter firewall, no internal monitoring, risk assessment three years old with one asset, annual IT-only training. *Why it matters:* the actor is a funded, adaptive sponsor, so compliance with standards gave false assurance.
5. **Attackers beat technology by using people and trust.** *Facts:* a fake antivirus update from a phone pretext, a recruitment approach to an engineer when the air gap blocked the technical route. *Why it matters:* strong technical layers do not protect the human route, and Horizon has little SETA aimed at it.

### C2: The Critical Risk

- **Asset:** Horizon's specialised hypercar design and manufacturing knowledge, held in R&D files and in the heads of engineers.
- **Threat:** FC Design, a well-funded competitor acting through intermediaries with a long-term strategic aim to build hypercars.
- **Vulnerability:** Horizon applies no classification, need-to-know limits, or departure controls to authorised R&D and manufacturing staff, and has no enterprise owner for knowledge security.
- **Risk:** FC Design recruits or compromises a Horizon engineer who uses authorised access to copy files and carries tacit know-how out, causing loss of confidentiality of Horizon's core capability, loss of competitive advantage, and long-term market erosion.
- **Why this over others:** the finance-network breach and phishing route were serious but produced supplier and pricing data, which can be rebuilt. The knowledge loss cannot be reversed and is the capability FC Design needed. The technical routes are also symptoms of the same missing ownership.

### C3: Five Recommendations

1. **Appoint a CSO reporting to the CEO with authority over knowledge, information, and IT security, and a leakage strategy.** The CSO owns an organisation-wide strategy for protecting capability. *Reduces the risk* by creating the missing owner and a single point that links HR, IT, R&D, legal, and physical security. (Strategic, formal.)
2. **Run a scenario-based risk assessment led by business owners and classify information.** R&D and manufacturing heads name the knowledge assets, rate scenarios with evidence, and classify materials. *Reduces the risk* by showing what is sensitive, so need-to-know and monitoring can target it. Review after each incident. (Strategic or tactical, formal.)
3. **Segment and monitor the crown-jewel environment.** The CSO and IT director keep R&D air-gapped, add internal zones, and use access and behaviour monitoring on copying and printing. *Reduces the risk* by limiting what an authorised insider can reach and flagging unusual copying even when credentials are valid. (Strategic or tactical, technical.)
4. **Issue a short enterprise policy plus a departure-and-recruitment procedure, with HR and legal.** It covers exit access removal, confidentiality agreements, notice of outside approaches, and certain sanctions. *Reduces the risk* by closing the exit route Emil used and giving staff clear rules and reporting. (Tactical, formal.)
5. **Run a role-targeted SETA programme with leadership modelling.** Follow the seven steps, begin with culture, train engineers and privileged IT staff on pretexts and approaches, and measure behaviour. *Reduces the risk* by making the human route harder and encouraging reporting. (Tactical, informal.)

Altitude check: two strategic, three tactical; formal, technical, and informal all appear. Add an incident response and intelligence structure if you have time (Week 10).

## References

Commission on the Theft of American Intellectual Property. (2013). *The IP Commission report*. The National Bureau of Asian Research.

Lim, S. (2018). *Information assurance and enterprise security risk management* [Video file]. University of Melbourne.
