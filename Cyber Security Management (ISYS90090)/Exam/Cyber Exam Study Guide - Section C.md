# Cyber Exam Study Guide — Section C (Case Study)

Course: [[Cyber Security Management (ISYS90090)/Course Overview|Cyber Security Management (ISYS90090)]]
Type: Exam how-to guide
Companions: [[Cyber Exam Cheat Sheet]], [[Horizon Question Workbook - Facts and Insights]], [[Cyber Flashcard Deck]]

## Why This Guide Exists

Your lecturer said the second half of the exam is where most students "fall off a cliff". Multiple choice and short answer are forgiving. The case study is worth half the marks, and most students had little to say on it. This guide trains one skill: **read an unseen case, then answer the same three questions every time**.

Plain version: the case is a story in which an organisation has been hurt. Your job is to act like a consultant who explains what the story really means (C1), names the one danger that matters most (C2), and tells the organisation what to change (C3).

## Exam Format (Lecturer's Description, Week 9 Lecture)

| Part | Share | What it is |
| --- | ---: | --- |
| Multiple choice | about 20 questions | Recall and recognition across the subject |
| Short answer | about 30% of the exam | Deliberately easier, per the lecturer |
| Case study (Section C) | 50% | One unseen case, three fixed questions |

Source: Week 9 lecture transcript and the [[Cyber Security Management (ISYS90090)/Assets/Week 09 - BioTech Exam Practice.pdf|BioTech exam rehearsal slides]]. The exam is closed-book and two hours. The lecturer described the format verbally, so confirm marks and timing in the official exam notice.

### The Three Section C Questions

| Question | Marks | Task | Marks per item |
| --- | ---: | --- | --- |
| C1 Key insights | 15 | Identify **five** insights critical to understanding the case's security challenges and explain why each matters. | 3 each |
| C2 Critical risk | 10 | Use the **triplet model** to identify the **single most critical risk**. Name the asset, the threat, and the vulnerability a threat actor exploits. Say why it outranks the risks you rejected. | one risk |
| C3 Recommendations | 25 | Develop **five** recommendations for managing the C2 risk, drawing on concepts across the subject. Explain how each helps treat the risk. | 5 each |

C3 is the largest question. It depends on C2, and C2 depends on C1. Treat the three as one chain.

### Time Plan (Two-Hour Exam)

The tutor run sheet gave students about half the exam time for the whole of Section C rehearsal, so a full-exam allocation is a judgement, not an official rule.

| Step | Suggested time | Note |
| --- | ---: | --- |
| Read the case once, marking facts | 8 min | Mark dates, because incidents may not be in date order |
| C1 five insights | 18 min | Write in full sentences if time allows |
| C2 triplet | 10 min | One asset, one threat actor, one specific weakness |
| C3 five recommendations | 28 min | Full sentences. This is the biggest mark pool |
| Multiple choice and short answer | remaining time | Do these quickly. They are the easier marks |

## The Core Skill: Facts Versus Insights

**Your rule:** if the case writes it down, it is a **fact**. An **insight** is something you derive from several facts.

| | Fact | Insight |
| --- | --- | --- |
| Where it comes from | Stated or shown in the case | Inferred by linking facts |
| Example (Horizon) | "Kurt said there is no need-to-know policy." | "Horizon has no enterprise owner for knowledge security." |
| Test | Can you point to the sentence? | Does it explain *why* several facts happened together? |
| Marks | None on its own | The marks |

How to write one insight (3 marks):

> The case states **[fact A]** and **[fact B]**. Together these show **[root cause]** because **[one-line reasoning]**. This matters because it **[enables the attack, hides it, or lets it repeat]**.

Intuition: a fact is a symptom the doctor can see. An insight is the diagnosis.

### Altitude Check (Lecturer's Main Warning)

The lecturer will immediately see **what kind** of insight you wrote. Operational answers lose marks when the case needs strategic ones.

| Altitude | Sounds like | Case question it answers |
| --- | --- | --- |
| Strategic | Organisation design, ownership, why teams do not talk, where IP strategy sits, what leaders value | Why did the organisation allow this? |
| Tactical | Programs, issue-specific policy, monitoring, SETA | How is security run day to day? |
| Operational | Add a firewall, add biometrics, correct one person's behaviour | What single fix applies to one incident? |

If all five insights or all five recommendations sit at the operational level, you have written an IT work plan, not a security analysis.

## Where Insights Come From (Insight Prompts)

Run through these quickly while reading. Each prompt usually produces one strong insight.

| Prompt | Look for in the case | Course link |
| --- | --- | --- |
| What is the real asset? | Capability, rare knowledge, trade secrets, or people rather than "IT" or a finished product | Week 2 asset types; Week 11 knowledge |
| Who owns security? | "Everybody", "not my area", IT as the only owner | Week 2 CISO; Week 4 management practices |
| Who is the adversary and what do they want? | Sponsor, motive, patience, several channels | Week 3 threat actors and APT pattern |
| Why were warnings missed? | Incidents reported separately and never linked | Week 3, Week 10 response and intelligence |
| Which management practice is weak? | Old risk assessment, unread policy, generic training | Weeks 4, 6, 7, 8 |
| Are controls matched to the threat? | One perimeter, no internal monitoring, compliance as proof | Weeks 4, 5, 9 |
| Where do people create the opening? | Trust, authority, pretexts, departing staff | Week 8 SETA; Week 3 vectors |
| Does the response bring in the right people? | Experts or leaders absent from the decision | Week 10 findings |
| Can the organisation tell what is sensitive? | No classification, copies everywhere | Week 11 sensitive information |

### Quick Insight Menu (Recurring Root Causes)

Most cases in this course share a small set of root causes. Use these as a self-check after reading, then **prove each with case facts**. Do not copy the label without evidence.

1. **Wrong asset or scope.** The organisation protects systems while the loss is knowledge, information, or capability.
2. **No owner.** Security sits with IT by default while the damaged asset belongs to the business.
3. **Silos.** HR, IT, legal, physical security, and the business each see a piece and no one sees the pattern.
4. **Controls built for the wrong adversary.** Standard controls meet a non-intelligent threat, but the real actor is purposeful and adaptive.
5. **Formal management without effect.** The policy, risk assessment, or training exists but does not change behaviour.
6. **People route beats technology route.** The attacker bypasses strong technology through trust, access, or recruitment.
7. **Detection and response structure is weak.** The organisation notices late, or the right people are not in the room.
8. **Compliance mistaken for security.** Standards were met, so leaders believed the organisation was safe.

## C2: The Triplet Risk

### The Triplet Model

`Asset ← Risk ← Threat`, with `Controls` mitigating the risk. A risk scenario exists only when a **specific threat actor** exploits a **specific vulnerability** in a **specific asset** and causes a **specific impact**.

### C2 Template

> **Asset:** [exact asset, with why it has value].
> **Threat:** [threat actor, motive, capability].
> **Vulnerability:** [one specific weakness the actor can exploit].
> **Risk:** [Actor] exploits [vulnerability] affecting [asset], causing [CIA loss] and [business consequence].
> **Why this one:** It outranks [rejected risk 1] and [rejected risk 2] because [impact is larger, likelihood is higher, harm is long-lasting, or the other risks are symptoms of this one].

### C2 Tests Before You Move On

- Is the asset exact? "IT" fails. "Specialised hypercar manufacturing knowledge held by engineers and R&D files" passes.
- Is the threat a **who**, not a type of malware?
- Is the vulnerability something the organisation could fix, rather than an event?
- Did you pick **one** risk? The question says the single most critical risk.
- Did you explain why you rejected the others? The BioTech slide asks for this directly.

Common error: calling the attacker the vulnerability, or writing "hackers could steal data" with no asset and no weakness.

## C3: Five Recommendations

### The Marking Test

The tutor run sheet states one rule to enforce: **each recommendation must say how it reduces the risk you named in C2**. A list of products earns very little.

| Recommendation quality | Mark range (slide example) | What it looks like |
| --- | --- | --- |
| Weak | 0–1 of 5 | Names a control and stops: "Run phishing awareness training." |
| Strong | 4–5 of 5 | States what changes, which weakness it fixes, how it reduces the risk, and who owns it |

The slide's strong example works because it says: who must do what, which single point of failure it removes, and why it works even when the attack looks genuine.

### The Three-Part Test for Every Recommendation

1. **What changes?** (a rule, structure, control, or practice)
2. **How does that reduce the C2 risk?** (name the weakness it closes)
3. **Who owns it?** (a role, not "the organisation")

### C3 Sentence Template

> **[Owner]** should **[specific change]**. The risk arises because **[weakness from C2]**. This reduces the risk by **[mechanism: prevents, detects, limits, or recovers]**, even if **[likely failure of another control]**.

### Spread Your Five Across the Altitude Grid

From the Week 10 slides. Aim for at least two strategic, at least one formal, one technical, and one informal item.

| | Formal | Technical | Informal |
| --- | --- | --- | --- |
| **Strategic** | Enterprise security policy; where security reports | Security architecture: what is kept apart from what | What leaders visibly value and reward |
| **Tactical** | Issue-specific policy; the SETA programme | Monitoring and threat hunting | How a team treats its sensitive work |
| **Operational** | System-specific policy; procedures | Firewall rules; device encryption | Individual habits on the day |

### Pull Recommendations From Across the Subject

The question says to draw on strategy, risk management, policy, SETA, and technology. A balanced set might use:

| Subject area | Typical strong recommendation shape |
| --- | --- |
| Governance and CISO (Week 2, 4) | Give a senior security leader enterprise-wide authority and a direct line to the CEO or board |
| Risk management (Week 6) | Run a scenario-based assessment on the named asset, use evidence for likelihood and impact, assign an owner, and review on a schedule |
| Policy (Week 7) | Write a short, owned, enforced policy for the specific risk and link standards and procedures beneath it |
| SETA (Week 8) | Target the exact roles at risk, follow the seven steps, study the culture first, measure behaviour |
| Strategy and defence in depth (Week 5, 9) | Separate, observe, and mediate around the crown jewels; combine prevention, detection, response, and deception |
| Incident response (Week 10) | Put decision makers, intelligence, and technical experts in one structure, with authority to act within the hour |
| Knowledge leakage (Week 11) | Classify sensitive information, track flows between people, paper, and digital containers, and control exit points |

### Anti-Patterns That Cost Marks

- A product list with no link to the risk.
- Five operational items that are all technical.
- Recommending the same idea five times with different wording.
- "Train staff" with no audience, content, or method.
- Fixing the symptom the case mentions rather than the root cause.
- Ignoring cost and feasibility. The lecturer's cost warning: spending far more than the asset is worth is a red flag.

## Building a Full Answer: Start-to-Finish Map

`Read → mark facts → find root causes → write five insights → choose one risk → write triplet → design five recommendations → check altitude and ownership`

1. **Read** once for the story and once for facts. Note timeline order.
2. **Mark facts.** Underline sentences that show who did what, who did not know, and what failed.
3. **Group facts** into patterns. Each pattern is a candidate insight.
4. **Pick the five** with the strongest evidence and widest effect. At least two should be strategic.
5. **Choose the single risk** that links most of those insights.
6. **Write the triplet** and defend the choice against rejected risks.
7. **Design five recommendations** that each attack a different part of the risk, then check the altitude grid and the three-part test.

## Self-Marking Checklist

Use this after every practice attempt.

| Check | Yes / No |
| --- | --- |
| Each insight cites at least two case facts? | |
| No insight is only a restated fact? | |
| At least two insights are strategic? | |
| C2 names one asset, one actor, one specific weakness, and one impact? | |
| C2 explains why other risks were rejected? | |
| Every recommendation links to the C2 weakness? | |
| Every recommendation names an owner? | |
| Recommendations cover more than one control type and more than one altitude? | |

## Extra Materials

Supplemental, not from the core lectures. Use for depth.

### Why Altitude Matters (Intuition)

An operational fix treats the last incident. A strategic fix changes the conditions that produced it. A hospital that repeatedly stitches the same wound is not helped by a better needle. It needs to know why the injuries keep occurring.

### Real Case Echo: Departing Engineer

The IP Commission report describes a Ford employee who copied about 4,000 documents just before leaving and took them to a new job at a Chinese automaker. The case resembles Horizon's Emil and shows that the departure-and-copy pattern is a real recurring route, not only a teaching device (Commission on the Theft of American Intellectual Property, 2013, pp. 41–42). See [[Cyber Exam Cheat Sheet#Reading and Expert Opinion Takeaways|reading takeaways]].

## Practice Cases

- [[Cyber Security Management (ISYS90090)/Exam/Practice Case 01 - Confidential Briefing|Practice Case 01 — The Confidential Briefing]]
- [[Cyber Security Management (ISYS90090)/Assets/Week 09 - BioTech Innovations Case Study.pdf|BioTech Innovations case]] and [[Cyber Security Management (ISYS90090)/Assets/Week 09 - BioTech Exam Practice.pdf|exam rehearsal slides]]. Attempt this under timed conditions before reading any model answer.
- [[Horizon Question Workbook - Facts and Insights]] for the full Horizon scene questions.

## Reference

Commission on the Theft of American Intellectual Property. (2013). *The IP Commission report*. The National Bureau of Asian Research.
