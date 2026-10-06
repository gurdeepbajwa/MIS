# Week 03 Tutorial

Course: [[Cyber Security Management (ISYS90090)/Course Overview|Cyber Security Management (ISYS90090)]]
Week: 03
Topic: Horizon Teaching Case, Scenes 1–6
Type: Tutorial

## Source Material

- [[Cyber Security Management (ISYS90090)/Assets/Week 03 - Horizon Teaching Case Complete Canvas.txt|Complete 2026 Canvas Horizon teaching case, Scenes 1–14]].
- [[Cyber Security Management (ISYS90090)/Assets/Week 03 - Horizon Teaching Case Canvas.txt|Earlier Canvas extract, Scenes 1–6]].
- [[Cyber Security Management (ISYS90090)/Week 03/Lecture|Week 03 lecture note]].
- [[Cyber Security Management (ISYS90090)/Week 03/Horizon Case Study|Complete Horizon case analysis]].

## Purpose

The Horizon case applies Week 3 threat and attack terms to a long-running information security incident at a hypercar maker. It shows how one target may face linked insider, technical, physical, and management threats over several years.

The lecturer said the workshop would also use parts of a prior exam's Section C questions to practise case analysis. This is study practice, not confirmation that the 2026 exam will repeat the same format.

## Case Overview

FC Design wants to enter the hypercar market but lacks Horizon's designs, supply-chain facts, and production knowledge. It hires Oliver to collect what it needs. The operation uses a former Horizon engineer, cyber intrusion, physical visits, and weak security management at Horizon.

Horizon records several warning signs, but teams treat each event on its own. Leaders do not join the reports into one risk view or act on the long-term campaign.

Scenes 7–14 continue the case through security governance, knowledge protection, defence strategy, risk assessment, policy, and the full social-engineering attack sequence. See [[Cyber Security Management (ISYS90090)/Week 03/Horizon Case Study|Complete Horizon case analysis]].

## Scene Guide

### Scene 1: The Business Warning

Horizon loses a major order to FC Design, which offers a similar car at a lower price.

Anders is likely to suspect that:

- A competitor gained access to Horizon's protected designs or knowledge.
- The product match is too close to result from normal competition alone.
- Horizon may face a larger leak than one copied file.

The first sign of a security incident appears as a business event: lost sales and a new competitor. This is why security teams need business context as well as system alerts.

### Scene 2: The Insider Link

Horizon learns that Emil, a former R&D engineer who joined FC Design, accessed and copied NextGen files before leaving.

Threat analysis:

- **Asset:** NextGen designs and R&D knowledge.
- **Threat actor:** Emil, with FC Design as a possible sponsor or beneficiary.
- **Threat:** Intellectual-property compromise, theft, and espionage.
- **Vulnerability:** Emil kept broad authorised access and could copy many files without an effective response.
- **Vector:** Legitimate staff access and file copying.
- **Attack:** Copying and transferring protected R&D material.
- **Impact:** Loss of confidentiality and competitive advantage.

The key point is that authorised access does not make every use of the information authorised.

### Scene 3: Planned Espionage

FC Design hires Oliver to collect Horizon's designs, specifications, suppliers, and prices. Oliver appears to arrange or manage corporate espionage.

FC Design has money, factories, and skilled staff, but it lacks the higher-level capability needed to build a hypercar. It seeks Horizon's information and knowledge to reduce the time, cost, and uncertainty involved in entering the market.

This differs from a random attack because FC Design has:

- A named target.
- A clear business aim.
- Long-term funding.
- A need for several types of information and knowledge.
- A planned campaign using several actors and methods.

### Scene 4: Information Security Is Broader Than IT Security

Kurt's team maintains systems and networks. It does not decide which business information is sensitive, manage paper records, monitor staff conversations, or set need-to-know rules.

The best term for Horizon's problem is **information security** because the firm must protect information and knowledge across systems, paper, people, conversations, and work practices. **IT security** covers the technology part but does not cover the full incident.

Horizon lacks:

- Clear information ownership.
- Sensitivity labels.
- Need-to-know access rules.
- Control of paper and verbal information.
- Clear duties across R&D, IT, physical security, and leaders.
- A process that turns a warning into action.

Short-term costs may include an investigation, legal advice, control changes, lost orders, and staff time. Long-term costs may include lower prices, lost market share, weaker profit, loss of research value, and a new competitor able to copy future work.

### Scene 5: A Campaign Hidden Across Separate Incidents

Horizon discovers that FC Design may have used several routes:

- Emil copied R&D files before leaving.
- Attackers used a zero-day flaw to spend time in the finance network.
- A visiting group asked detailed technical questions and took photographs.
- Supplier, price, material, and design information came from separate systems and people.

Horizon reported the events but did not link them. The firm failed to see that one actor might run a patient campaign across several years.

This reflects weak risk perception. Each team saw only its own event, while no owner assessed the combined business threat. Reports did not lead to shared analysis, stronger controls, or limits on FC Design's access.

### Scene 6: The Technical Attack Plan

Jordan's high-level plan follows these stages:

1. **Reconnaissance:** Study Horizon's firewalls, servers, devices, remote access, and patch state.
2. **Find a weakness:** Look for unpatched systems, poor wiring, weak wireless access, exposed devices, or a user laptop that can provide entry.
3. **Gain access:** Exploit a known flaw, hijack an executive laptop, enter through a wireless point or device, or buy a zero-day flaw.
4. **Avoid detection:** Use custom malware that signature-based tools may not recognise.
5. **Create persistence:** Install several backdoors so Horizon cannot end access by closing one route.
6. **Move through the environment:** Reach systems that store the desired information.
7. **Remove information:** Copy the target files and knowledge without permission.

The scene shows that a capable attacker changes methods when one route fails. Defence must therefore include patching, device and network design, access limits, behaviour monitoring, incident response, and information controls.

## Information and Knowledge

The stolen R&D files give FC Design explicit information, such as blueprints and specifications. They do not provide all of Horizon's knowledge.

FC Design also needs:

- Supplier relationships and prices.
- Material choices.
- Production methods.
- Engineering judgement.
- Staff experience.
- An understanding of how the parts work together.

This explains the mixed campaign. One copied folder cannot give FC Design every skill, relationship, or fact required to compete.

## Threat Map

| Case event | Threat category | Main control gap |
| --- | --- | --- |
| Emil copies NextGen files | Intellectual-property compromise, theft, insider threat, and espionage | Broad access, weak exit checks, and poor monitoring |
| Oliver plans the operation | Espionage and information theft | Weak threat intelligence and third-party awareness |
| Zero-day attack reaches finance | Software attack and espionage | Detection, response, network separation, and follow-up gaps |
| Visitors take photos and ask detailed questions | Trespass and espionage | Weak visitor rules, escort, device control, and reporting links |
| Teams fail to join the reports | Weak policy, planning, and ownership | No shared risk view or senior owner |
| Jordan seeks several entry routes | Software attack and unauthorised access | Patch, identity, endpoint, network, device, and monitoring gaps |

## Incident–Trigger–Process Practice

### Incident

Emil used valid R&D access to copy hundreds of NextGen files shortly before leaving Horizon for FC Design.

### Trigger

The event becomes a security incident when Emil copies protected files without a work need, moves them outside approved storage, or transfers them to an unauthorised party. His valid login does not authorise those uses.

### Process

- Classify and label R&D information.
- Apply need-to-know access and block bulk copying where suitable.
- Alert on unusual downloads and removable-media use.
- Review access when staff resign or change roles.
- Run a formal departure process across HR, management, legal, IT, and physical security.
- Preserve logs and investigate suspicious activity.
- Join cyber, physical, staff, and business reports under one incident owner.

## Workshop Tasks

Prepare to give:

1. Three key insights from scenes 1–6.
2. One precise asset–threat pair from the case.
3. A case answer that names the asset, actor, weakness, vector, attack, impact, and matching control.

One sound asset–threat pair is:

- **Asset:** Horizon's NextGen designs and related production knowledge.
- **Threat:** A competitor-sponsored operation that uses insiders, cyber intrusion, and physical access to copy the capability.

The full risk statement should go further than the pair by naming each actor and weakness involved.

## Main Lessons

- Information security covers information and knowledge in all forms, not only IT systems.
- A trusted insider or partner can become a threat actor.
- One campaign may use people, systems, devices, visitors, and business ties.
- A logged event has little value if no one assesses its business meaning or acts on it.
- Valid access can still support an attack when a person uses it for an unauthorised purpose.
- Managers need a joined view of assets, actors, motives, warning signs, and control gaps.

## Live Tutorial Notes — Expand Later

- Mintzberg's 5 Ps.

### Group Workshop Scenario

- **Industry:** Construction
- **Threat category:** Espionage
- [ ] Define the exact asset, threat actor, motive, weakness, vector, attack sequence, and business impact.

### Quiz Scope and Difficulty

There is a scope conflict:

- **Official written notice:** Each quiz covers all prior weeks and excludes the current teaching week.
- **Tutor's spoken guidance:** Quizzes 2–4 cover only the teaching block since the prior quiz, while Quiz 5 covers all content.

The official notice gives this cumulative scope:

| Quiz week | Confirmed cumulative scope | Notes |
| --- | --- | --- |
| Week 04 | Weeks 01–03 | Does not include Week 04 content; intended as the simplest quiz |
| Week 06 | Weeks 01–05 | Does not include Week 06 content |
| Week 08 | Weeks 01–07 | Does not include Week 08 content |
| Week 10 | Weeks 01–09 | Does not include Week 10 content |
| Week 11 | Weeks 01–10 | Does not include Week 11 content; final and most difficult quiz |

The tutor instead stated:

- Week 06: Weeks 04–05.
- Week 08: Weeks 06–07.
- Week 10: Weeks 08–09.
- Week 11: All content.

Both sources agree that Week 04 covers Weeks 01–03. The conflict begins with Week 06 and needs written clarification. Cumulative review remains the safer plan until the teaching team resolves it.

**Personal preparation plan:** Bias Quizzes 2–4 toward the new block already named by the tutor, while retaining a smaller delayed-review set from earlier weeks. Use roughly 75% new-block questions and 25% earlier-week questions. Treat Quiz 5 as fully cumulative.

- The quizzes become harder as students build knowledge and skill through the term.
- Each quiz has 10 multiple-choice questions.
- The tutor displays one question at a time for a set period.
- Students mark a hardcopy bubble sheet with a pen and must bring their own pen.
- The total duration and time per question remain unconfirmed.

### Exam Case-Analysis Preparation

- The case used for tutorial practice will differ from the case given in the exam.
- Prior students found the exam case hard because they did not know how to analyse an unfamiliar case under exam conditions.
- The Horizon case will unfold through the semester. Each week, relevant scenes should show how the week's course ideas appear in a realistic case.
- From next week or the following week, the tutor plans to use short cases and explain what a good case analysis must contain.
- Weekly case work should build the skill needed to analyse the unseen exam case rather than encourage memorising Horizon's facts.
- The exam carries 50% and has a pass hurdle, so case-analysis practice is a high study priority.
- The stated size of the exam case was unclear in the live notes and needs confirmation before recording an exact length.
- See [[Cyber Security Management (ISYS90090)/Exam/Case Analysis Preparation|Case Analysis Preparation]].

### Case Facts Versus Insights

| Case element | Meaning | Use in analysis |
| --- | --- | --- |
| Fact | Something the case directly states or shows; often a visible symptom | Cite it as evidence |
| Insight | An inferred problem, pattern, or root cause that explains one or more facts | State and defend it with linked case evidence |

- Repeating a fact does not diagnose the case problem.
- Strong analysis connects several facts, reads beyond the stated events, and explains the underlying cause.
- Recommendations should address the root cause revealed by the insight, not only the visible symptom.
- This distinction will matter for both the unseen exam case and the Week 05 presentation.

**Horizon example:**

- **Facts:** Emil copied files, attackers entered the finance network, visitors took photographs, and separate teams recorded the events.
- **Insight:** Horizon lacked joined information-security ownership and failed to combine separate warnings into one view of a long-term espionage campaign.

### Assignment 2: Problem Before Solution

- The group must describe and support the underlying problem before presenting its innovation.
- Start with the visible symptoms and evidence, then explain the root cause or problem they reveal.
- A solution has little value if the group cannot show that it understands the problem or why the solution fits it.
- Propose recommendations and controls only after defining the problem clearly.
- The required order is: `symptoms and evidence → problem or root cause → impact → solution → matching controls`.

#### Draft Event: Confidential Construction Rates

- **Asset:** The confidential bill of quantities, including material quantities, supply costs, unit rates, supplier discounts, cost models, profit margins, and tender calculations. Only four or five authorised staff members know or can access this information.
- **Threat actor:** A rival construction firm working with a malicious insider from the small authorised group.
- **Motive:** Obtain the bill of quantities, learn the firm's true supply costs and planned margin, and underbid it on a major tender.
- **Weakness:** A trusted estimator can export or copy the data through valid access, so multiple passwords alone do not stop misuse by that authorised person.
- **Vector:** The insider's valid account and an unauthorised export to a personal account, cloud drive, or removable device.
- **Event:** Before a major tender closes, the rival pays a senior estimator to copy the firm's current rates, supplier terms, and pricing model and transfer them outside the firm.
- **Attack:** Covert collection and disclosure of protected commercial information for competitive espionage.
- **Impact:** Loss of confidentiality, lost tender, weaker negotiating power, reduced profit, investigation costs, and loss of trust.

#### Accidental Disclosure Variant

- **Event:** A supplier intends to email confidential material prices and project rates to the construction firm but selects a similar contact name and sends them to a rival company.
- **Immediate threat category:** Human error or failure by an external supplier.
- **Asset:** Confidential supplier prices and bill-of-quantities inputs.
- **Vector:** Misdirected email attachment.
- **Impact:** Loss of confidentiality and possible loss of tender advantage.
- If the rival knowingly keeps and uses the information to gain an advantage, its later conduct may form part of competitive espionage. Keep the supplier's mistake and the rival's deliberate use as two linked events with different actors and intent.

### Threat Intelligence and Incident Context

- Treat an incident as a sequence of linked events, not one isolated event.
- Each observed event may reveal part of an adversary's wider operation.
- Knowing **who** the threat actor is and **why** they target the organisation gives the response team context and situational awareness.
- Study the actor's **TTPs: tactics, techniques, and procedures**. These help link separate signs to a known pattern of behaviour.
- Assess the actor's sophistication, funding, commitment, and persistence to judge whether current controls are enough.
- Distinguish a committed, targeted actor from an opportunistic actor who may move to an easier target.
- Organisations have limited money, time, staff, and controls. Threat knowledge helps them direct those resources toward the most relevant risks.
- The aim is a security program guided by threat intelligence and aligned with the organisation's actual risk.
- **Tutor's closing point:** Understanding the threat actors the organisation truly faces helps it place limited resources where they will make its defence more efficient and effective.
- **Specificity rule:** Describe each event, cyber threat, attack, and risk as precisely as possible. Name the exact actor, asset, weakness, vector, action, and impact where the evidence allows it. Broad labels lead to weak analysis and controls that may not fit the real risk.

### Nation-State and Organised-Crime Actors

- Nation-state actors usually pursue political, military, strategic, or national-interest aims. Their exact goals vary by state and operation.
- Western security sources often focus on China, Russia, Iran, and North Korea as a "Big Four". This framing reflects a Western view; other states may identify the United States, United Kingdom, Australia, or other countries as major state threats.
- Every state may conduct or support cyber operations, but the structure and details of these programs often remain secret.
- Organised-crime groups mainly seek profit. They may have strong funding, skills, planning, and persistence.
- Extortion is a common profit method: the group steals or controls data and demands payment to restore access or prevent disclosure.
- Some criminal groups operate on their own, while others receive support from or maintain ties to a nation-state.
- Attribution should therefore consider both the team carrying out an attack and any sponsor directing or funding it.

### Hacktivism and Cyberterrorism

- Hacktivists act in support of an ideological or political cause, such as an environmental campaign.
- The tutor distinguished activism from cyberterrorism by the result of the digital action.
- In the tutor's framing, an ideological cyber action moves from activism to cyberterrorism when it causes damage or harm.
- When using this distinction in assessed work, state the harm, intended outcome, target, and method rather than relying only on the actor's claimed cause.

### Independent and Opportunistic Actors

- Independent actors may gain access to attack tools without belonging to a larger group.
- They often scan the internet for targets of opportunity rather than pursue one fixed target.
- They may leave enough signs for investigators to track them.
- Motives may include financial gain, curiosity, challenge, thrill, or excitement.
- Do not assume one motive from the actor category alone; use the observed target, conduct, and TTPs.

### Insider Actors

- The tutor identifies three insider-threat types:

| Type | Position and intent | Possible conduct |
| --- | --- | --- |
| Negligent insider | A legitimate worker causes exposure without intending harm. | Mistakes, unsafe handling, weak security practice, or failure to follow a process |
| Malicious insider | A legitimate worker intends to misuse access or cause harm. | Fraud, sabotage, disruption, theft, extortion, or personal gain |
| Credentialed external actor | An outside actor gains valid credentials and acts as an insider. | Espionage, theft, disruption, or movement through internal systems |

- **Intent** separates a negligent insider from a malicious insider.
- An outside actor can create an insider threat once they gain valid access and appear to act as an authorised user.

The tutor groups insider impact into two broad forms:

1. **System manipulation:** Fraud, sabotage, disruption, ransomware, or other harmful changes to systems and operations.
2. **Data theft:** Removal or misuse of data for extortion, espionage, financial gain, personal gain, or personal use.

The same case may involve both forms. The organisation should identify the actor type, intent, access used, asset affected, and resulting impact before choosing controls.

### Follow-Up

- [ ] Confirm how the tutor applied Mintzberg's 5 Ps in this workshop.
- [ ] Expand the five terms, purpose, and link to the relevant course or assignment topic after the tutorial.
- [ ] Link the tutor's TTP discussion to the Horizon attack sequence and later risk-management material.
- [ ] Add a clear comparison of nation-state, independent organised-crime, and state-linked organised-crime actors.
- [ ] Check the set reading's definitions of hacktivism and cyberterrorism before using the tutor's harm threshold as a formal definition.
- [ ] Link each insider type to suitable preventive, detective, and response controls.
