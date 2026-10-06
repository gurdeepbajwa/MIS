# Final Research Proposal Pitch: Mock Audience Questions

- Course: Skills for IS Research and Development (ISYS90118)
- Assessment: Final Research Proposal Pitch (25%, due Friday 23 October 2026 at 8:00 pm)
- Purpose: Rehearse likely questions from an academic audience (IS researchers) after the pitch.
- Sources: Submitted `Research-Proposal.docx` / `.pdf`, [[Week 06 - Delivery Pressure and AI Coding Research Proposal]], [[Week 06 - AI Coding Proposal Research Gap Check]], [[Appendix B - Luna Literature Review Response]].
- Status: Question bank with suggested answer directions. Answers are drafted from our own documents only. Check each against the final pitch before using it, and do not claim anything the proposal does not support.
- Format source gap: the pitch brief, length and delivery rules are not yet in the workspace. Add them to [[Assignments Overview]] when found.

## Decide Before Rehearsing

The submitted proposal compares **AI vs no AI** across four repositories in two hours. The Week 06 working notes settled on **delivery pressure** (shorter vs adequate deadline, everyone using the agent). The proposal itself says it "will not isolate the effect of tighter deadlines." Choose which framing the pitch uses, because several questions below depend on that choice. If the pitch moves to the pressure framing, state that it is a refinement and why (see Q2 and Q7).

## Priority Questions (Most Likely)

| # | Question | Why they would ask |
| --- | --- | --- |
| 1 | Your question asks about *quality*, but your main measure is accepted tasks per developer. Which is it? | Question and primary measure do not match |
| 2 | Becker et al., Balepur et al. and Chen et al. already compare AI with no AI. What is new here? | Gap is narrow and the gap check admits no confirmed first study |
| 3 | Ten participants, five per group. What can you claim? | Sample size |
| 4 | Why a between-groups design rather than a crossover? | Chen et al. counterbalanced tool order within participants |
| 5 | How do you know your tests measure business-requirement quality and not just test-passing? | Researcher-written acceptance checks |
| 6 | What is your theory, and what does it do in the study? | Pennington used only to interpret interviews |
| 7 | Is this a pressure study or an AI study? | Mismatch between lit review and design |
| 8 | What do you expect to find, and what would change your mind? | No stated hypotheses |

## 1. Problem and Motivation

**Q1. Your motivation is a workplace expectation of faster delivery, but it rests on one interview study. How strong is that evidence?**
- Source: Miller et al. (2025), 54 developers in 27 teams at one company; arXiv preprint (the ICSE 2026 listing links to the 2025 manuscript).
- Answer direction: Agree it is one setting and a preprint. It motivates the practical question and is not evidence that expectations rise everywhere. The study tests delivered work, not management behaviour. Avoid saying AI "causes" higher demands (gap-check note).

**Q2. You say the problem is changing expectations. How does comparing AI and no-AI speak to that?**
- Answer direction: It tests whether the extra output is acceptable output. Link back to the intro claim: workload expectations should rest on work that passes quality checks, not submission counts.

**Q3. Your motivation is partly personal experience. How do you manage bias?**
- Source: Week 06 note says the experience is "a starting observation, not evidence."
- Answer direction: Neutral outcomes are stated up front ("limited gains, poorer quality or inconclusive differences"), scoring is blinded where feasible, and tests are fixed before data collection. Name your position as a working developer openly.

## 2. Literature and Gap

**Q4. Becker et al. (2025) found AI made experienced developers 19% slower. Why would your result differ, and why does it matter if it doesn't?**
- Source: Becker et al. (2025) used 16 developers on 246 tasks in repositories they knew well; Becker et al. (2026) reported selection problems.
- Answer direction: Your setting is unfamiliar repositories and multiple switches, so familiarity is the key difference. A null or negative result is still reportable. Do not claim your study will replicate or refute theirs.

**Q5. Balepur et al. found agent users did better initially but understood less. Your study seems to repeat that.**
- Source: Balepur et al. (2026), 54 students; the follow-on extension task removed agent support.
- Answer direction: Their participants were students building and extending one application. Yours are professionals in unfamiliar repositories with a delivered-change outcome. Say what you add, not that nobody has studied understanding.

**Q6. Padmakumar et al. already varied time limits with AI. Doesn't that cover your gap?**
- Source: One-hour vs four-hour limits, 40 freelance developers, a model-derived reliance score.
- Answer direction: They varied time on new web-app tasks and measured reliance, not preservation of existing business rules in an inherited repository. This is a bounded-search claim, not "first."

**Q7. Your literature review spends a section on time pressure, then you say you won't isolate deadlines. Why is it there?**
- Answer direction: Pressure is the delivery context (the shared two-hour limit), not the manipulated variable. If the pitch has adopted the pressure framing, say the review now matches the design.

**Q8. How did you search? Is this a systematic review?**
- Source: Gap-check note: 23 web queries in the follow-up, domain-filtered, not Scopus, Web of Science, ACM or IEEE searches. No screening count.
- Answer direction: Be honest: a targeted scoping search, followed by citation tracing, with a library-database search planned. Never call it systematic.

**Q9. A large share of your references are 2026 arXiv preprints. How reliable are they?**
- Source: Balepur, Shen (EvoCode-Bench), Jiang, Padmakumar, Chen and others are preprints. Borg et al. is published.
- Answer direction: Preprints are labelled as such. Use them for design and recency, not as settled findings. EvoCode-Bench is used for the evaluation distinction (new vs obsolete rules), not its leaderboard numbers (its repository reports withdrawn results).

**Q10. You used an AI model to produce a comparison review. What did it add, and what did it get wrong?**
- Source: Appendix B. The "Luna" review omitted the agent studies and implied AI worsens as requirements become ambiguous without a direct test.
- Answer direction: Quote your own comparison: useful quality dimensions (correctness, maintainability, security), but weaker on delivery pressure, understanding and mid-task requirement changes. Admit apparent errors were kept deliberately, and name at least one you checked.

## 3. Theory and Conceptual Framework

**Q11. Pennington (1987) is about how experts comprehend programs. How does it apply to an agent-assisted study?**
- Source: Proposal uses Pennington's program-model vs domain-model distinction to guide interviews only.
- Answer direction: It structures what you ask developers: how a program runs vs what it is for. It is not tested. Concede it predates agents and that the application is a proposed interpretation.

**Q12. You want to study understanding, but you have no direct measure of understanding. Why not?**
- Source: The Week 06 note considered a no-AI post-task explanation. The proposal uses interviews instead and says it won't sit a knowledge test.
- Answer direction: Interviews are about reasoning and decisions, not scoring. Say a short post-task prediction exercise is a possible extension and would measure task understanding, not long-term skill.

**Q13. Why not use cognitive load, Bainbridge's ironies of automation, or Storey's cognitive and intent debt?**
- Source: Bainbridge and Storey appear in the Week 06 working draft, not the submission.
- Answer direction: One main theory keeps a small proposal feasible. Be ready to say what you would gain from each.

## 4. Research Design

**Q14. Why five per group? Could you detect any difference?**
- Source: Limitations: "individual experience may strongly affect results", findings are "exploratory estimates."
- Answer direction: The study is exploratory and reports individual results, averages and ranges. No significance claims. Planned balancing by experience. It reports a pattern, not an effect size.

**Q15. Why not have each developer do both conditions (within-subject)?**
- Source: Chen et al. (2025) counterbalanced tool order across 20 participants.
- Answer direction: Learning and familiarity carry over between conditions in repositories. State the trade-off: crossover gives power but contaminates. If you cannot defend it, say you would consider a crossover with different repositories in each condition.

**Q16. Four repositories in two hours: does switching confound your result?**
- Source: Proposal allows familiarity to grow through return visits; limitations say faster participants may revisit more often.
- Answer direction: Switching is the studied condition, not noise. A pilot checks comparable effort and that the pool cannot be exhausted. Sequences are balanced for difficulty and order. Admit return visits are partly outcome-dependent.

**Q17. The no-AI group has no AI but the AI group has an agent. Isn't it a comparison of two different jobs?**
- Answer direction: Yes. The study compares working practices, not isolated tools. Both groups get the same documentation and tools apart from AI. State that results apply to this configuration.

**Q18. Participants practise both approaches on unrelated code. Does that bias toward AI-fluent developers?**
- Source: Recruitment needs regular AI-tool experience; eligibility is meant to depend on skills, not opinions; attitudes are recorded.
- Answer direction: Practice reduces first-use effects. Recruiting AI users limits generalisation to AI-experienced professionals. Say so.

**Q19. How do you handle people who submit nothing?**
- Source: Acceptance rates are undefined, not zero, for developers with no submissions.
- Answer direction: Report accepted tasks as the main measure so zero is a valid result, then show acceptance rate only where defined. Keep partial progress separate.

**Q20. What agent, which model version, and what happens when the model changes next month?**
- Source: Fixed agent setup; gap-check notes a rapidly changing evidence base.
- Answer direction: Pin and record the version. The finding is bound to that setup. The method is the transferable contribution.

## 5. Measurement and Analysis

**Q21. Who decides what counts as an acceptable change?**
- Source: Researcher-controlled end-to-end tests (new rules work, replaced rules stop applying, following EvoCode-Bench), unit tests, a quality engineer and a reviewer using a predefined checklist.
- Answer direction: Define checks before data collection and pilot them. Name the three components (new, obsolete, unchanged behaviour) and report each, so one cannot hide another.

**Q22. Is the reviewer really blind? AI-generated code often looks different.**
- Source: "Reviewers will not see group labels where feasible."
- Answer direction: Concede blinding is partial. Tests are automatic, so only the checklist and edge-case review are exposed. Reviewers are not told group membership.

**Q23. Inter-rater reliability for the quality engineer and reviewer?**
- Gap: The proposal does not describe agreement checks. Say what you would add, for example independent scoring of a subset and reporting agreement.

**Q24. You call this mixed-method. What does the qualitative strand add, and how are the strands integrated?**
- Source: Week 06 note warned that coding events into categories does not automatically make a study mixed method.
- Answer direction: Interviews and observation explain outcomes and test whether stated reasoning matches behaviour. Differences between account and outcome are retained, not resolved. Be ready to say what each strand answers.

**Q25. Observation and screen recording: will participants behave naturally?**
- Source: Limitations: "Observation may affect behaviour, and interviews rely on recall."
- Answer direction: Acknowledge a Hawthorne effect. The researcher does not coach. Recordings support later recall.

**Q26. Where does the "three- to fourfold productivity gain" come from?**
- Source: Limitations paragraph says findings are not proof of a general three- to fourfold gain, but the submission does not cite where that figure comes from. Check this before the pitch. If it is not sourced, remove it or cite it. An unsourced number invites a challenge.

## 6. Ethics, Feasibility, Contribution

**Q27. What are the ethics risks, and where is the approval?**
- Source: Informed consent, recordings, AI-provider data handling, withdrawal limits, private GitHub repositories, participant codes, university-approved storage. Required approval is obtained before data collection. RIOT certificate is in Appendix A.
- Answer direction: It is a proposal, so approval is a planned step. Be specific about what participants are told about AI-provider data handling and limits on withdrawing data.

**Q28. The repositories are adapted from real projects. Any confidentiality or licence issues?**
- Source: Preparation includes removing confidential material from adapted repositories.
- Answer direction: Only use material the team owns or that is licensed for reuse, and say how that is checked.

**Q29. Is it feasible to recruit professional developers who are regular AI users, outside your workplace?**
- Source: Recruitment outside the researcher's workplace; about 20 developer-hours plus interviews.
- Answer direction: Name a recruitment route and the risk of volunteers being unrepresentative. Have a fallback such as fewer repositories or tasks.

**Q30. If AI wins, are you saying employers should expect more output?**
- Source: Expected contribution says accepted-work gains "would support higher output expectations within the study's setting."
- Answer direction: Keep the claim bounded: setting, tasks and tool only. The study does not justify workforce reductions (it says so itself). A larger output expectation also needs a view of review burden and understanding costs.

**Q31. So what? Who uses this result?**
- Answer direction: Managers planning workload and onboarding across repositories; researchers who need a measure of accepted change rather than submission counts.

## 7. Challenge Questions

- If you could keep only one outcome measure, which and why?
- If AI users score worse, is that a tool problem or a training problem?
- What would you drop first if recruitment gave you only six developers?
- What is the weakest part of your proposal?
- What did you change after reading the closest studies, and what stayed the same?
- Is this a Gregor Type I description of differences, or do you aim to explain them?
- How would your design change with a longer study over weeks?

## Weak Spots to Fix or Rehearse

1. Question wording (quality) vs main measure (accepted tasks per developer).
2. The unsourced "three- to fourfold" figure.
3. Whether pressure is a variable or only a context.
4. Pennington as theory vs the missing direct measure of understanding.
5. Between-groups design vs the Chen et al. crossover precedent.
6. Reviewer agreement and blinding.
7. Literature search method and preprint reliance.
8. Confidentiality and recruitment routes.

## Practice Method

1. Answer each priority question aloud in about 45 seconds.
2. Start with a direct answer, give the evidence, then state the limit.
3. Never claim "first", "proves" or "shows AI causes." Use "bounded search" and "exploratory."
4. Record the questions you could not answer and update the proposal or pitch notes.
