# Week 05 Lecture

Course: [[Cyber Security Management (ISYS90090)/Course Overview|Cyber Security Management (ISYS90090)]]
Week: 05
Topic: Role of Technological Controls — Defence in Depth

## Source Material

- 2026 Canvas Module 5 pages 5.0, 5.1, 5.2, 5.3, 5.5, and 5.6, plus discussions 5.3.1 and 5.4, viewed on 1 September 2026.
- [[Cyber Security Management (ISYS90090)/Assets/Week 05 - Defence in Depth Slides|Week 05 defence-in-depth slides]], updated 25 August 2026.
- [[Cyber Security Management (ISYS90090)/Assets/Week 05 - Defence in Depth Transcript|Week 05 lecture transcript]].
- Whitman and Mattord (2022), Chapters 8 and 9, pp. 295–383. The prescribed pages are not stored in the workspace, so the textbook descriptions below come from Canvas and the lecture rather than direct review.
- [[Cyber Security Management (ISYS90090)/Week 03/Horizon Case Study|Horizon case study]], especially Scenes 10 and 11.

## Intended Learning Outcomes

- Explain defence in depth and the castle model.
- Match technological controls to the role they play in a layered defence.
- Explain the strengths and limits of firewalls, VPNs, intrusion detection, identity and access controls, encryption, and security testing.
- Explain why cloud computing, artificial intelligence, and distributed workforces change how organisations apply the castle model.
- Design a defence-in-depth response for a stated asset, threat actor, and vulnerability.

## Topic Map

`Risk scenario → separate → observe → mediate → assess → adapt`

1. **Risk scenario:** Name the asset, threat actor, and vulnerability.
2. **Separate:** Place enforced boundaries between the threat and asset.
3. **Observe:** Watch activity at several useful points and raise timely alerts.
4. **Mediate:** Check identity and control each request for access.
5. **Assess:** Find exposed, weak, misconfigured, or leaking parts of the attack surface.
6. **Adapt:** Change the design as assets move to cloud services and staff work from many locations.

The lecture treats technology from a management and strategy view. The main question is not how a product works in full technical detail. It is why a control is needed, where it belongs, which risk it reduces, and how it works with other controls.

## Defence in Depth

**Defence in depth** places several successive and linked controls between a threat actor and an asset. The outer areas are less trusted, while controls become tighter nearer the critical asset.

The design assumes that any single control may fail. A strong defence therefore:

- makes an attacker overcome several different obstacles;
- delays progress towards the asset;
- detects activity while the attack is still under way;
- limits how far an attacker can move after one breach;
- gives defenders time and information to respond;
- keeps protecting the asset if one control fails.

The goal is not to buy many unrelated tools. The controls must reinforce one another and address the stated risk.

### Why the Castle Model Helps

The castle model gives a simple structure for understanding layered controls:

| Castle function | Digital function | Course examples |
| --- | --- | --- |
| Outer boundary | Separate trusted and untrusted zones | Firewalls and network segmentation |
| Gate | Let approved users cross the boundary safely | VPN and secure remote access |
| Guards and watch points | Observe traffic and behaviour | Network and host intrusion detection |
| Inner rooms and locked areas | Limit access near valuable assets | Identity and access management, need-to-know access, encryption |
| Surveying the area | Find paths an attacker can use | Scanners, analysis tools, and penetration testing |
| Traps and false targets | Distract attackers and collect intelligence | Honeypots, honeynets, and padded cell systems |

The castle creates an advantage for defenders by forcing an attacker through narrow, visible, and repeated control points. In digital systems, segmentation and varied controls can produce the same effect.

## Layer One: Separate

Separation creates and enforces a boundary between an asset and a threat. It also divides the internal environment into smaller zones so one breach does not expose every asset.

### Firewalls

A **firewall** regulates network traffic between logical zones. It checks traffic against rules and allows or denies passage.

Key points:

- The firewall does not create the whole perimeter. It controls a passage through the perimeter.
- All relevant traffic must pass through the firewall. Traffic routed around it remains outside its control.
- Every external connection needs suitable boundary control. One protected route does not secure unprotected routes elsewhere.
- Internal firewalls can divide a network into zones and slow movement after an attacker enters.
- Placing valuable assets behind several layers forces the attacker to defeat more than one control.
- Using varied technologies may stop one known flaw or one set of attacker skills from defeating every layer.

Whitman and Mattord identify five firewall types in the set reading:

1. Packet-filtering firewalls.
2. Application gateways.
3. Circuit gateways.
4. MAC-layer firewalls.
5. Hybrid firewalls.

The course does not require detailed recall of every technical feature beyond what supports control selection and strategy.

### Firewall Limits

A firewall cannot:

- inspect traffic that bypasses it;
- remove the need for internal controls;
- stop a trusted user from misusing valid access by itself;
- guarantee that permitted or encrypted traffic is harmless;
- remain effective without correct rules, placement, updates, and monitoring.

Closing all external access may protect confidentiality but stop legitimate work and harm availability. Managers must balance security with the authorised flow of information.

### Virtual Private Networks

A **virtual private network (VPN)** gives an approved remote user a protected route through the logical perimeter. It uses encryption and credentials to make remote traffic act as though it came from an approved internal connection.

A VPN supports safe passage, but it also extends internal access to a remote device and user. The organisation must therefore combine it with strong authentication, suitable access limits, secure endpoints, logging, and monitoring.

## Layer Two: Observe

Boundaries delay and filter attacks, but they do not show everything that happens inside. Observation helps the organisation find attacks, check whether other controls work, and act before the attacker reaches the asset.

### Intrusion Detection and Prevention

An **intrusion detection system (IDS)** watches network or host activity for signs of attack and alerts the responsible staff. A good IDS should identify the suspected attack, its source, and possible action in time to support a response.

An **intrusion detection and prevention system (IDPS)** may also block or stop activity when its rules permit this.

Two broad detection approaches are:

| Approach | How it works | Main limit |
| --- | --- | --- |
| Signature detection | Compares activity with known attack patterns. | May miss a new or changed attack whose pattern is not known. |
| Anomaly or behaviour detection | Builds a view of normal activity and flags unusual behaviour. | Normal behaviour varies, which can create false alerts or missed events. |

Artificial intelligence and machine learning can support richer behaviour analysis, but they do not remove the need for sound data, human judgement, and response processes.

### Vantage Points

No single sensor sees the whole attack. Placement changes what an IDS can observe.

- A sensor outside the firewall sees incoming attempts.
- A sensor inside the firewall shows what passed through and helps test firewall rules.
- Internal sensors show movement between network zones.
- Host agents can inspect activity after encrypted traffic reaches its endpoint and is decrypted.

Several vantage points give a fuller view than one perimeter sensor.

## Layer Three: Mediate

Security must let approved people use assets while stopping excessive or improper use. The lecture calls this **mediation**.

### Identity and Access Management

Identity and access management links a person or system identity to allowed actions and resources.

1. **Authenticate:** Check whether the requester is who they claim to be.
2. **Authorise:** Decide what that identity may do.
3. **Control access:** Enforce which resources and actions are available at the point of use.
4. **Encrypt:** Keep the asset unreadable if earlier access controls fail or the asset leaves its normal environment.

Authentication and authorisation are different. Proving an identity does not give that identity unlimited access. Need-to-know and least-privilege rules limit access to what the role requires.

### Encryption as the Last Inner Layer

Encryption protects the content of an asset even when another control fails. It is most useful when:

- the organisation controls the keys;
- only approved identities can obtain decryption rights;
- access rules apply wherever the data moves;
- the organisation manages keys, recovery, revocation, and logging well.

Encryption does not replace access control. An approved user with valid decryption rights may still misuse the information.

## Knowing the Attack Surface

The **attack surface** is the set of exposed systems, services, ports, devices, paths, information, and other points that a threat actor could target.

The organisation should keep checking:

| Question | Useful controls |
| --- | --- |
| What is exposed? | Port scanners and operating-system detection tools |
| What is misconfigured? | Firewall analysers and vulnerability scanners |
| What is leaking? | Network sniffers, wireless security tools, and reviews of public information |

### Penetration-Testing Limit

A penetration test can reveal long-standing weaknesses that the organisation did not know about. However, it gives a view of the environment at one time.

Its main limits are:

- systems and settings may change soon after the test;
- new services and devices create new weaknesses;
- a technical test may not cover people, work practices, and knowledge leakage;
- fixing the reported findings does not prove that the organisation is now secure.

Penetration testing should support continuing asset discovery, configuration checks, monitoring, and reassessment rather than replace them.

## Deception and Security Intelligence

The Canvas module names three forms of deceptive control:

- **Honeypot:** A decoy system or service intended to attract and study attackers.
- **Honeynet:** A group or network of decoy systems.
- **Padded cell system:** A controlled environment that redirects a suspected attacker away from real assets.

These controls may reveal attacker methods and motives, but the organisation needs skilled design and legal review. A poorly designed decoy may expose the defence or create added risk.

## Why the Old Castle Model Is Weaker Today

The defence-in-depth strategy still matters, but the old idea of one fixed internal safe zone has become less useful. The updated slides name three main forces:

1. **Cloud computing:** The organisation may own the data but not possess or control the infrastructure that stores it.
2. **Distributed workforces:** Data and users operate across homes, mobile devices, suppliers, and many networks.
3. **Artificial intelligence:** Detection is moving from fixed signatures towards richer behaviour analysis and prediction, while attackers also gain new ways to adapt.

These changes make location alone a weak basis for trust. Controls must follow the asset and assess each request.

## Cloud Service Models and Control

Moving an asset to the cloud separates ownership from possession. The organisation remains accountable for the asset, but its direct control changes with the service model.

| Model | Provider supplies | Customer's main control role |
| --- | --- | --- |
| Infrastructure as a service (IaaS) | Base computing infrastructure | Build and manage more of the operating environment, security layers, and asset controls |
| Platform as a service (PaaS) | Infrastructure and a managed platform | Configure applications, identities, access, data, and the controls available within the platform |
| Software as a service (SaaS) | A complete application and supporting stack | Set users, roles, data rules, configuration, and provider requirements within the service's limits |

Contracts and service-level agreements can state required security, but they do not give the customer direct control over every provider action. The customer still needs provider checks, clear ownership, logging, assurance, and a response plan.

## Protection That Travels With the Asset

Modern defence in depth places controls around the data itself:

1. **Encryption travels with the data:** Storage access reveals ciphertext unless the requester can obtain the correct key.
2. **Policy travels with the data:** Classification and access rules remain linked to the asset wherever it moves.
3. **Identity enforces each request:** Access depends on who is asking, their role, context, and location rather than simple presence on an internal network.

The updated slides summarise the wider shifts as:

- **Perimeter to identity:** Multi-factor authentication and behaviour analysis keep checking the requester.
- **Reactive to predictive:** Detection expands from known signatures towards behaviour-based analysis using AI and machine learning.
- **On-premises to cloud-first:** Cloud security posture and provider controls become part of the defence.

## Matching Controls to Risk

Use this sequence when choosing controls:

1. Name the valuable asset or capability.
2. Identify the threat actor, motive, and likely methods.
3. Identify the weakness and the paths to the asset.
4. Add controls that separate the actor from the asset.
5. Add observation at the points that show attempted entry and internal movement.
6. Mediate every approved request through identity, authorisation, access limits, and encryption.
7. Check the attack surface and whether each control still works.
8. Add policy, ownership, staff practices, response, and recovery so the technology forms part of one program.

A control list without this link to risk does not show sound security management.

## Horizon Case Connection

Scene 10 shows that Horizon's key asset is not each finished car or one folder of designs. Its lasting asset is the capability to build valuable hypercars. That capability exists across information, employee knowledge, judgement, work processes, tools, and supplier relationships.

Scene 11 shows why one perimeter firewall is not enough. Horizon has little internal monitoring, relies on a common firewall product, and faces an intelligent actor seeking business capability rather than simple service disruption. Its controls must match that actor and protect knowledge across people, processes, and technology.

See [[Cyber Security Management (ISYS90090)/Week 03/Horizon Case Study#Detailed Analysis: Scenes 10–14|Horizon Scenes 10 and 11 analysis]].

## Exam Use

The lecturer said the prescribed chapters support the lecture. The exam will not test all technical detail from the 88 pages beyond what the lecture requires.

For an applied question:

1. Define defence in depth as several successive, linked control layers.
2. State the asset, threat actor, and vulnerability.
3. Use at least the three functional layers: **separate, observe, and mediate**.
4. Name suitable controls within each layer.
5. Explain how the controls work together to delay, detect, contain, and respond to the actor.
6. Add managerial controls such as ownership, policy, staff practice, monitoring, and review.
7. Address cloud, mobile work, or provider limits if the asset leaves the organisation's own infrastructure.

Useful answer form:

> The organisation should use defence in depth to protect **[asset]** from **[actor and method]**. It should separate the asset using **[boundary and segmentation controls]**, observe activity using **[monitoring controls and vantage points]**, and mediate access using **[identity, authorisation, access, and encryption controls]**. These layers work together because **[explain delay, detection, containment, and response]**. **[Managerial controls]** keep the design aligned with the changing risk.

Common errors include:

- Listing products without naming the asset, threat, or weakness.
- Treating a firewall as the entire perimeter or complete defence.
- Assuming internal or VPN traffic is safe because it crossed the boundary.
- Confusing authentication with authorisation.
- Relying on one IDS sensor or one penetration test.
- Treating encryption as a replacement for identity and access control.
- Assuming a cloud provider removes the organisation's accountability.

## Applied Diataxis Notes

- [[Cyber Security Management (ISYS90090)/Week 05/Defence in Depth - How-to Guide|How to design a defence-in-depth strategy]]
- [[Cyber Security Management (ISYS90090)/Week 03/Horizon Case Study|Horizon Case Study — Reference and Explanation]]

## Reference

Whitman, M. E., & Mattord, H. J. (2022). *Principles of information security*. Cengage.
