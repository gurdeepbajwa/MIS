# Horizon Scenes 04–09 — Quick Reference

Course: [[Cyber Security Management (ISYS90090)/Course Overview|Cyber Security Management (ISYS90090)]]
Source: [[Cyber Security Management (ISYS90090)/Week 03/Horizon Case Study|Complete Horizon Case Study]]
Type: Tutorial and exam quick reference

## Six-Scene Map

`authorised insider theft → linked espionage campaign → adaptable attack plan → management diagnosis → social-engineering entry → shift from systems to people`

## Scene Distillation

| Scene | Key fact | Root insight | Main concepts |
| ---: | --- | --- | --- |
| 4 | Emil copied hundreds of R&D files through valid access. Horizon had no need-to-know policy, and IT did not know which information was sensitive. | Horizon confused IT security with information security and lacked clear ownership of information and knowledge. | Insider threat, authorised-access misuse, information versus IT security, governance |
| 5 | Horizon links Emil, a finance-network intrusion, and FC Design visitors who took photographs and asked detailed questions. | Separate reports were parts of one long-term espionage campaign, but siloed teams failed to connect them. | Threat intelligence, TTPs, incident sequence, cross-team awareness |
| 6 | Jordan plans several entry routes, custom malware, several backdoors, persistence, and information theft. | A funded and persistent actor will change methods when one route fails; blocking one vector does not end the threat. | Attack vectors, advanced persistent threat, attacker–defender imbalance, defence in depth |
| 7 | Horizon has strong IT availability and standard controls but no leakage strategy, broad ownership, useful training, or cross-team review. | Compliance and technical controls gave false assurance because they did not address Horizon's main business risk: loss of competitive capability. | Strategy, governance, CSO or CISO, SETA, business alignment |
| 8 | Jordan maps the firm through public and technical data, enters through a fake antivirus update, reaches finance, but cannot cross the R&D air gap. | Social engineering and trust bypassed the perimeter. The air gap limited technical access but did not protect people or knowledge. | Reconnaissance, phishing, malware, social engineering, network separation |
| 9 | Oliver responds to the air gap by advising FC Design to recruit a Horizon engineer and targets a suitable employee. | When systems block access, an adaptable actor may target a person who holds or can recreate the missing knowledge. | Insider recruitment, tacit knowledge, adaptive adversary, people risk |

## Overall Insight

Horizon's central failure was not the absence of all security technology. It failed to identify its competitive knowledge as the key asset, understand FC Design as a strategic threat actor, connect warning signs across teams, and build a security strategy that covered people, processes, information, and technology.

## Three Strong Exam Points

1. **Valid access can still support an attack.** Emil's authority to open R&D files did not authorise copying them for a competitor.
2. **An incident may form one part of a wider sequence.** The insider, cyber intrusion, visitor activity, and recruitment effort support the same strategic objective.
3. **Controls must match an adaptive actor.** FC Design moved between technical, physical, relationship, and human routes as barriers appeared.

## Short Answer Template

> The case states **[two facts]**. Together, they show **[root insight]** because **[reasoning]**. This exposes **[asset]** to **[actor and threat]** through **[weakness and vector]**. Horizon should address the cause through **[management response]** and support it with **[matching controls]**.
