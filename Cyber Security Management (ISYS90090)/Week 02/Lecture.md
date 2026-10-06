# Lecture

Course: [[Cyber Security Management (ISYS90090)/Course Overview|Cyber Security Management (ISYS90090)]]
Week: 02
Topic: Why Organisations Need Cybersecurity

## Source Material

- Week 02 Canvas Module 2 content supplied on 4 August 2026.
- [[Cyber Security Management (ISYS90090)/Assets/Week 02 - Why Organisations Need Cybersecurity Transcript.vtt|Week 02 lecture transcript]] supplied on 8 August 2026.
- [[Cyber Security Management (ISYS90090)/Assets/Week 02 - Why Organisations Need Cybersecurity Slides.pdf|Week 02 slides]]
- [[Cyber Security Management (ISYS90090)/Assets/Week 02 - Global CISO Survey Reading.pdf|2022 Global CISO Survey]]
- [[Cyber Security Management (ISYS90090)/Assets/Week 02 - CISO Responsibilities Mind Map.png|CISO responsibilities mind map]]
- [[Cyber Security Management (ISYS90090)/Week 02/Tutorial|CEO, CIO, and CISO tutorial]]

## Topic

The Cybersecurity Triplet Model, the role of information security in organisations, and the role of the CISO

## Intended Learning Outcomes

- Explain why the Cybersecurity Triplet Model matters when addressing cybersecurity problems.
- Identify and describe how information security protects organisational information resources.
- Explain the main duties and functions of a Chief Information Security Officer.

## Video Study Route

Use [[../Weeks 01-02 - Video Study Guide|Weeks 01–02 — Video Study Guide]] for a video-first pass on risk management, the CIA attributes, and the CISO role. Return to this lecture note for the exact course terms and detail.

## Key Concepts

### Business Information System Security Triplet

The triplet model represents information security as a relationship between three constructs:

- **Information resources:** Assets of value that require protection.
- **Threats:** Factors that may harm the confidentiality, integrity, or availability of an asset.
- **Controls:** Measures used to reduce exposure to threats.

A **vulnerability** is a weakness or susceptibility in an asset that allows a threat to harm it. Each asset-threat-vulnerability combination forms a distinct risk because a different asset, threat, or weakness can change the likely impact and the controls needed.

The model's basic relationship is:

1. A threat can act against an information resource.
2. A vulnerability gives the threat a path to harm the resource.
3. A control limits that path or reduces the resulting harm.

The model helps managers start with the asset and risk rather than a preferred tool. The question is not simply, "Which security product should we buy?" It is, "Which asset faces which threat through which weakness, and what control will reduce that risk?"

The course diagram adapts Baskerville's business information system security triplet, in which safeguards protect an information-resource object from a threat subject.

#### Risk Profile, Controls, and Risk Appetite

The lecturer described the triplet model as the main model for the subject. It forces precise analysis:

- A security problem needs both an asset with value and a threat capable of harming it.
- A risk scenario arises when a specific threat exploits a specific vulnerability in a specific asset and creates an impact.
- Broad labels such as "IT" are too vague to serve as useful assets. An email service, database service, web service, sensitive document, or person with rare expertise is specific enough for analysis.
- The organisation's **risk profile** is the collection of risk across all identified scenarios.
- Controls reduce risk exposure, but no organisation can remove every risk or spend without limit.
- **Risk appetite** is the amount of risk the organisation accepts after choosing how to use its resources.

Security management therefore involves prioritising scenarios and spending limited resources where they produce the most useful risk reduction. This differs from responding to each incident without a risk-based plan.

### Three Categories of Information Assets

The transcript expands the course's definition of information resources into three categories.

#### Digital Platforms

Digital platforms include specific systems and services such as email, databases, web services, e-commerce services, devices, and infrastructure. Managers should name the exact service or system rather than treating all IT as one asset.

#### Data and Information

Information may sit in systems, messages, documents, social media, printed pages, or other media. The management task is not to protect every item equally. It is to identify which information carries value, sensitivity, or duties that justify protection.

#### Knowledge

Knowledge forms when people combine information with experience, judgement, and skill to create value. It can be:

- **Explicit knowledge:** Knowledge that can be written, recorded, or explained.
- **Tacit knowledge:** Experience and judgement bound to a person and difficult to transfer in full.

Rare expertise, trade secrets, recipes, research methods, production skills, and quality practices may determine whether a firm can compete. In pharmaceutical, advanced-manufacturing, and similar firms, losing this knowledge may cause more harm than a temporary system outage.

This broader asset view explains why security must cover systems, information, paper records, people, and business capability.

### Strategic Lesson from Huawei and T-Mobile

The Week 2 lecture returned to the Tappy case from Week 1. T-Mobile already had guards, access controls, cameras, staff training, and rules around the secure laboratory. The lecturer argued that adding more operational controls would not solve the central problem because T-Mobile had not analysed Huawei's changing strategic intent.

The proposed management response was:

1. Examine the partner's record, motives, capabilities, and competitive plans before granting access.
2. Create a team that monitors behaviour across the relationship.
3. Identify what knowledge or components the partner would need to reproduce the protected capability.
4. Define warning signs that show a partner may be acting as a competitor or threat.
5. Trigger a security response, including restricting access, when those signs appear.

This is an example of **threat intelligence** applied to a business partner. The course treats partners, suppliers, and other trusted parties as possible future threat actors. Technology can help detect behaviour only after managers decide which behaviour matters.

For case and exam answers, the lecturer expects analysis of assets, motives, relationships, warning signs, and management action. A list of tools such as encryption or biometrics does not address a strategic problem on its own.

### Organisational Impact of a Cyber Incident

The transcript distinguishes visible response costs from wider and longer-term effects.

Expected or visible effects may include:

- Technical investigation.
- Customer notification and support.
- Post-breach protection.
- Legal advice and litigation.
- Media response.
- Security improvements.
- Regulatory work.

Less visible effects may include:

- Higher insurance premiums.
- Higher borrowing costs.
- Long operational disruption and recovery.
- Loss of trust.
- Damage to the organisation's name and market value.

The lecturer stated that many costs remain unexpected and that recovery from a major breach can take years. The exact percentages used in the lecture came from a slide not stored with the supplied deck, so treat them as lecture claims rather than independently verified figures. The main course point is that impact analysis must extend beyond the first technical response.

### Confidentiality, Integrity, and Availability

| Attribute | Course definition | Simple meaning |
| --- | --- | --- |
| Confidentiality | Information resources can be read only by authorised parties. | Keep information from people who should not see it. |
| Integrity | Information resources can be changed only by authorised parties. | Prevent improper or unauthorised changes. |
| Availability | Information resources remain available to authorised parties when needed. | Keep information and services usable. |

"Information resources" covers information and information technology. The CIA attributes therefore apply both to the content an organisation values and to the systems that store, process, or move it.

For example, a customer database may suffer:

- A confidentiality loss if records are copied.
- An integrity loss if account details are changed.
- An availability loss if the service becomes unreachable.

### Categories of Information Security Controls

| Control category | Main nature | Examples | Main effect |
| --- | --- | --- | --- |
| Formal | Prescriptive | Policies, standards, procedures, audit findings, and penalties | States what people must do and what follows from non-compliance |
| Informal | Suggestive and cultural | Education, training, awareness, leadership example, and team norms | Shapes understanding and routine behaviour |
| Technological | Restrictive | Firewalls, intrusion detection, access controls, and other security tools | Limits, detects, or blocks actions through technology |

The categories depend on each other. A firewall may enforce a rule, but management must first decide the rule through policy and risk work. Staff must also understand the rule and avoid bypassing it. An effective security strategy therefore uses formal, informal, and technological controls together.

### Four Roles of Information Security

Whitman and Mattord identify four roles for information security in organisations.

#### Role 1: Protect the Organisation's Ability to Function

Information security supports business continuity by reducing risks that could stop or harm operations. This role shows why cybersecurity is also a management issue. Policy, risk work, training, strategy, accountability, and technology all shape whether the organisation can continue operating.

#### Role 2: Enable the Safe Operation of Applications

Organisations rely on systems, networks, and applications from outside suppliers. These products may contain flaws that harm the product or the wider environment.

The organisation must:

- Protect applications from unauthorised access and interference.
- Protect the organisation from threats within or introduced through applications.
- Set a secure operating environment for third-party technology.
- Keep senior leaders accountable rather than treating secure operation as an IT-only task.

#### Role 3: Protect Data, Information, and Knowledge

Information security protects resources both **at rest** and **in motion**. These resources may include:

- Intellectual property and trade secrets.
- Research and development information.
- Marketing plans and pricing.
- Customer and supplier lists.
- Payroll and staff data.
- Business knowledge held in documents, systems, processes, and people.

This role matters because a leak may remove both information and the knowledge needed to use it.

#### Role 4: Safeguard Technology Assets

Systems and networks support routine work and need protection in their own right. Controls may include encryption, firewalls, intrusion detection, access control, patching, secure settings, and monitoring.

This is one part of information security, not its whole scope. Technology cannot replace sound ownership, policy, culture, risk decisions, or management.

### The CISO

The CISO is the senior leader responsible for guiding the organisation's information security program. The role connects business goals, security risk, policy, culture, technology, incident response, and outside duties.

Main responsibilities include:

- Develop security strategy and policy.
- Align security with business aims.
- Build and maintain a security-aware culture.
- Lead risk management and advise leaders on risk choices.
- Oversee threat prevention, detection, and incident response.
- Support secure projects, systems, cloud use, mobile technology, and business change.
- Manage identity, access, architecture, and security operations.
- Coordinate with legal, human resources, audit, compliance, and regulators.
- Build security cases, budgets, measures, reports, teams, and supplier relationships.
- Lead response and recovery during major incidents.

The CISO mind map groups this work into several linked domains:

- Business enablement.
- Internal support for information security.
- Governance.
- Security operations.
- Identity management.
- Risk management.
- Legal and human resources.
- Compliance and audits.
- Security architecture.
- Budget and business cases.
- Project delivery.

The role is broad because security decisions affect most parts of the organisation.

## 2022 Global CISO Survey

### Method and Limits

Heidrick & Struggles surveyed 327 CISOs and other senior information-security leaders in Spring 2022. Respondents came from the United States, Europe, and Asia Pacific. The data was self-reported, country sample sizes varied, and respondents came mainly from large firms and the United States.

The results describe this sample and should not be treated as a full count of every CISO or sector.

### Lecture Interpretation of the CISO Evidence

The lecture used the survey to make four management points:

- Large and highly regulated organisations, such as banks and telecommunications firms, are more likely to employ CISOs than small firms and some less regulated sectors.
- A technical or engineering career may prepare a CISO for security operations but may not provide the business, strategy, or management skills needed at senior level.
- Reporting lines indicate authority. Each extra level between the CISO and CEO can weaken access to decisions, funds, and senior attention.
- Stress and burnout are organisational issues because they can weaken judgement, succession, staff retention, and security leadership.

These are the lecturer's interpretations of the survey. They should be distinguished from the survey's reported percentages and sample limits.

### Which Industries Have CISOs?

| Current employer category | Respondents |
| --- | ---: |
| Financial services or fintech | 33% |
| Technology and telecommunications | 24% |
| Industrial, manufacturing, or energy | 17% |
| Consumer, retail, or media | 11% |
| Healthcare, biotechnology, or life sciences | 6% |
| Other | 9% |

Public-sector, education or not-for-profit, and business or professional-services employers do not appear as separate categories in the current-employer chart. They may fall within "Other," so the survey does not prove that these sectors had no CISOs.

The sample also leans toward large firms: more than two-thirds of respondents worked for companies with annual revenue of at least US$5 billion.

### Career Path Into and Beyond the CISO Role

- IT was the main career function for 71% of respondents.
- Software engineering was the main function for 10%.
- Fifty-three percent came from another CISO role.
- When people already doing CISO work without the title are included, 70% moved laterally into the current role.
- A majority wanted a future role other than CISO.
- Board membership was the strongest next-role preference: 56% in the Americas, 44% in Asia Pacific and the Middle East, and 40% in Europe.
- Other paths included chief security officer, CIO, entrepreneur or consultant, chief risk officer, private-equity executive, and CEO.

The survey presents the CISO role as important but without one clear next step. Board work offers a non-technical path, but companies often want prior board experience. Almost half of the sample had advisory-board experience, while only 14% sat on a corporate board or both a corporate and advisory board.

### What CISOs Do

The five most common functions reporting to the CISO were:

| Function | Respondents |
| --- | ---: |
| Security operations | 88% |
| Governance, risk, and compliance | 87% |
| Penetration testing | 87% |
| Security architecture | 86% |
| Product or application security | 79% |

Other areas included business continuity and disaster recovery, trust, crisis management, fraud, physical security, privacy, and safety.

These results support the course view that the CISO does more than operate security tools. The role covers governance, assurance, design, operations, resilience, and business coordination.

### Most Significant Cyber Risks

| Risk | Respondents |
| --- | ---: |
| Ransomware attacks | 67% |
| Insider threats | 32% |
| Nation-state attacks | 31% |
| Malware attacks | 21% |
| Malware-free attacks | 3% |
| Other | 7% |

The report links these risks to security becoming part of software development and business processes through a security-by-design approach.

### CISO Reporting Lines

| Reports to | Respondents |
| --- | ---: |
| CIO | 38% |
| CTO or senior engineering executive | 15% |
| COO or CAO | 9% |
| Global CISO | 8% |
| CEO | 8% |
| Chief risk officer or senior regulatory executive | 4% |
| General counsel | 3% |
| Other | 15% |

Nearly two-thirds reported to someone other than the CIO, but only 8% reported to the CEO. Reporting structures varied by region and industry. Financial-services CISOs often sat under the CIO or CTO, while some security functions sat within risk as a second-line function. Some CISOs also used direct and indirect reporting links, such as a formal manager plus access to an audit committee.

Reporting lines matter because they affect:

- Access to business and risk decisions.
- Independence from the teams being reviewed.
- Authority over budget, policy, and response.
- How clearly security issues reach senior leaders and the board.

Board access was stronger than direct CEO reporting: 88% reported to the full board or a committee, based on 288 responses to that question.

### Personal Risks Faced by CISOs

| Personal concern | Respondents |
| --- | ---: |
| Stress linked to the role | 59% |
| Burnout | 48% |
| Higher turnover caused by a strong hiring market | 33% |
| Job loss after a breach | 25% |
| Feeling underpaid | 21% |
| Team distraction caused by the hiring market | 20% |
| Difficulty keeping up with changing threats | 19% |

The role brings broad accountability and high pressure. This makes succession, staff depth, clear authority, and realistic workloads part of security management.

## Prescribed Reading

- Whitman and Mattord (2022), Chapter 2, "Need for Information Security," pp. 27-34.
- The textbook supports the module but is not yet stored in the workspace assets.

## Questions

- How does the triplet model stop control-first decision making?
- Why does each asset-threat-vulnerability combination form a separate risk?
- How do formal, informal, and technological controls depend on one another?
- How do the four roles of information security extend beyond IT security?
- Why does the CISO need both technical knowledge and business authority?
- Which survey findings suggest that the CISO role remains tied to IT?
- What could a CISO gain or lose by reporting to the CIO, CEO, or chief risk officer?
- How can threat intelligence detect when a trusted partner begins acting as a competitor or threat?
- What are the three categories of information assets, and why does each need a different protection approach?
- How do risk profile and risk appetite guide the use of a limited security budget?
- How could stress and burnout weaken an organisation's security capability?

## Applied Diataxis Notes

- [[Cyber Security Management (ISYS90090)/Week 02/Tutorial|Tutorial - CEO, CIO, and CISO Role Play]]

## Summary

- The triplet model links information resources, threats, vulnerabilities, risks, and controls.
- A risk profile combines the organisation's scenarios, while risk appetite states how much remaining risk it will accept.
- Information assets include digital platforms, data and information, and explicit and tacit knowledge.
- Strategic threat intelligence should examine trusted partners as well as known attackers.
- Confidentiality, integrity, and availability state the main protection goals.
- Formal, informal, and technological controls must work as a set.
- Information security protects operations, applications, information and knowledge, and technology assets.
- The CISO leads a broad program that joins governance, risk, operations, culture, technology, compliance, and incident response.
- The 2022 survey shows that CISOs often retain strong links to IT while gaining wider board access and business duties.
- Strong security depends on clear authority, reporting, resources, and cooperation across senior roles.

## References

Aiello, M., Thompson, S., Reventlow, C., Shaul, G., Randria, M., & Vaughan, A. (2022). *2022 global chief information security officer (CISO) survey*. Heidrick & Struggles. https://canvas.lms.unimelb.edu.au/courses/237535/files/28186968?wrap=1

In-text citation: (Aiello et al., 2022) or Aiello et al. (2022).

Rehman, R. (2015). *CISO mind map: An overview of the responsibilities and ever-expanding role of the CISO* [Infographic]. https://rafeeqrehman.com/

In-text citation: (Rehman, 2015) or Rehman (2015).
