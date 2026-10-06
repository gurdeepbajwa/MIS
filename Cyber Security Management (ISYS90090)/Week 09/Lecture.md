# Week 09 — Security Strategy and Defence in Depth

Course: [[Cyber Security Management (ISYS90090)/Course Overview|Cyber Security Management]]

Sources: Week 9 slides and lecture transcript ([[Cyber Security Management (ISYS90090)/Assets/Week 08-10 - Canvas Source Index|source index]]). This is a quick-study distillation. The Canvas D-series module pages and the BioTech exam-practice material are not covered here.

## Start-to-Finish Map

**Triplet model** (asset ← risk ← threat, controls mitigate risk) → **Strategy** decides how controls are chosen and *combined* → built from **nine paradigms** → organised into **strategy / tactics / operations** → expressed as **defence in depth** (the castle) → tested against **three principles** (obscurity, weakest link, shared security).

> Plain version: a strategy is not one control. It is the whole coordinated program of controls against the organisation's risk scenarios.

## 1. What Strategy Is

Three definitions were given. The third is the one to learn:

> The art and science of deciding how best to use appropriate defensive security technologies and measures, deploying them in a **coordinated** way to defend organisational information resources against **internal and external** threats by providing confidentiality, integrity and availability at **least effort and cost** while being **effective**.

Why it is useful: (1) art *and* science, (2) coordinated deployment, (3) efficiency, (4) covers internal and external threats.

- Definitions 1 and 2 are general. Strategy responds to a **challenge**, over the medium to long term, by aligning intentions, environment and resources.
- **Cost matters.** The lecturer's rule of thumb: spending more than about 10% of an asset's value to protect it is a warning sign. This was stated verbally, not as a course formula.
- Security science is not a university discipline in its own right. The lecturer's nine paradigms are the course's attempt to define it.

## 2. The Nine Paradigms

"Paradigm" here means a fundamental approach to thinking about and doing security. They split into two groups.

**Group A: behaviour of attacker and defender (6)**

| Paradigm | Core idea | Memory hook |
| --- | --- | --- |
| Prevention | Block access before an attack; passive and always on | A safe; a shell; outer space; copy-protection codes |
| Detection | Notice a specific violating behaviour so response can follow | An alarm; an intrusion detection system |
| Response | Take corrective action against an identified attack | Guards; shutting down a network segment |
| Deterrence | Disciplinary action to influence behaviour | Works only if sanctions are **certain** and **severe** |
| Surveillance | Systematic, broad monitoring to build situational awareness | CCTV; broad vs detection's narrow |
| Deception | Decoys that waste the attacker's time and remove their leverage | False accounts and decoy documents |

**Group B: structuring the battlefield (3)**

| Paradigm | Core idea | Memory hook |
| --- | --- | --- |
| Perimeter defence | A boundary around a domain with one policy inside | Firewall around an enclave |
| Compartmentalisation | Separate zones, so one breach does not open everything | DMZ; subnets |
| Layering | Multiple complementary barriers that back each other up | Three castle walls; firewalls from three vendors |

Distinctions that are easy to confuse:

- **Surveillance vs detection:** surveillance is broad and aims to understand the environment; detection is narrow and aims to spot a specific behaviour.
- **Prevention vs perimeter:** prevention is any blocking (even software refusing access). Perimeter, compartments and layers are specifically about *structuring the battlefield*, so perimeter is one kind of prevention, but prevention is wider.
- **Deterrence in policy:** "must fire" signals certainty; "will consider" leaves room to avoid the sanction.

### Combining the paradigms (the safe example)

Prevention, detection and response work together. A cheaper safe (for example one rated to resist a professional safecracker for 30 minutes) plus an alarm plus guards who arrive within that time can match the protection of an expensive safe. **Weak prevention means you need better detection and response.** This is the economic logic behind combining paradigms.

### Why deception is powerful

Attackers choose when, where and how to attack, so they hold natural leverage. After the attack, leverage shifts to the defender, who can investigate at leisure. Deception removes the attacker's leverage *before* the attack by making the target unreadable. It works only if the illusion keeps changing, and it takes significant resources. The lecturer mentioned some managed security providers that do this commercially.

## 3. Strategy, Tactics, Operations and the Concept Map

Top to bottom: **strategy → tactics → operations**. These leverage **controls** (formal, informal, technological, and administrative if you add it), which draw their principles from the **paradigms**. Strategy can be a plan *or* a process, achieves a security objective, protects information resources, must complement security culture and reduces risk from the environment.

Learn the relationships, not just the words. The lecturer called the diagram a "dictionary" for the whole course.

## 4. Defence in Depth: The Castle

Place **multiple obstacles** between threat actor and asset, designed to complement each other, so the attacker needs more sophistication, more time and more cost, and may give up and go elsewhere.

- **Concentric network:** every firewall placed on a traffic channel creates another ring. Firewall policy should let traffic pass a zone only if it is meant to.
- **Air gap:** keeps a valuable asset off the network, forcing physical penetration.
- **Proxies** and **IDS / access control** add further layers.
- **Different vendors:** the lecturer's example is a bank buying firewalls from three vendors so an attacker must handle all three.
- **Extra layers can separate skill levels,** which reverses the asymmetric leverage.
- **Rule of thumb:** key assets sit behind as many layers as possible.
- **Castle mapping questions from the slides:** where are the perimeter walls, the drawbridge, the inside of the castle and the king (the asset)?
- **Bull's-eye:** the asset (information) sits in the middle, with the **digital environment** on one side and the **cognitive environment** on the other. The digital side has many layers; the human side has few, mostly training. That is why social engineering usually beats technical attack, and it links back to [[Cyber Security Management (ISYS90090)/Week 08/Lecture|Week 8]].

## 5. Three Principles

**Security through obscurity is not security.** Assume the attacker knows your strategy, assets and organisation. Real security holds even then. Hiding information is still sensible as *part* of a strategy, but you must not *rely* on it. Different attackers differ: hiding details may stop a local thief but does nothing against a government-level attacker.

**Weakest link.** A chain is no stronger than its weakest link, and effort on stronger links is wasted. The weakest link depends on the *attacker*: profile their skills, history, motivation and adaptability. Avoid generic threat actors. An example from the lecture: a bank found its model of protecting key assets failed because attackers went for the weakest-protected systems and moved in from there, so it shifted to shielding the broader environment. Shadow IT (business units buying IT without telling security) hands attackers weak entry points.

**Shared security.** The organisation is a shared security environment, like 100 families each maintaining a section of a common wall. One weak section compromises everyone. Physically the weak section is visible; digitally it is not, so you need continuous monitoring and scanning.

## 6. Exam Cue: Altitude

The lecturer warned that strong-looking technical answers often miss the point of case questions, which are usually about knowledge and capability. Check your *altitude*:

- **Strategic:** organisational design and structure, why teams do not talk, where IP strategy sits.
- **Operational/technical:** add a firewall, add biometrics, change one person's behaviour.

Insights, key risk and recommendations should all be pitched at the strategic layer when the case calls for it.

## Quick Recall

- Recite the third definition's four selling points.
- Name the nine paradigms and say which group each belongs to.
- Why can a cheap safe plus alarm plus guard match an expensive safe?
- What two things make deterrence work?
- Surveillance vs detection? Prevention vs perimeter?
- Why does deception remove attacker leverage, and why must it keep changing?
- Name the three principles and give a one-line example of each.
- Where is the "king" in a network castle, and why does the cognitive side have fewer layers?
