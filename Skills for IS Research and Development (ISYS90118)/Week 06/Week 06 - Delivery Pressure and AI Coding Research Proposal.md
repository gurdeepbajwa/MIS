# Week 06 Research Proposal: Delivery Pressure and AI Coding in Unfamiliar Repositories

- Course: Skills for IS Research and Development (ISYS90118)
- Updated: 8 September 2026
- Status: Current working direction; literature section drafted, full proposal and research gap still under development.
- Earlier exploration: [[Week 04 - Product Requirement Prompt Research Question]]
- Related tutorial: [[Week 06 - Research Proposal Tutorial]]
- Official brief and rubric: [Research Proposal on Canvas](https://canvas.lms.unimelb.edu.au/courses/237538/assignments/663896), inspected in Safari on 7 September 2026.
- Drafting support: Codex assisted with source searches, comparison, and this draft; the author should read the selected papers and revise the argument before submission.

## Current Research Question

> How does delivery pressure affect developers’ ability to implement business requirement changes in an unfamiliar repository using an AI coding agent?

Define ability through the final system's fit with the revised requirements and its preservation of valid existing behaviour. This measures performance on the study task, rather than a person's general competence.

## Research Motivation

The author's experience motivates the problem: working across more repositories, using agents to explain unfamiliar code, mapping business changes onto systems that are only partly understood, and reviewing increasingly large generated changes. This is a starting observation, not evidence that all developers share the experience or that agents cause employers to increase demands.

The proposed study examines one requirement change in one unfamiliar repository. Work across multiple projects and growing expectations explain the practical concern but are not additional experimental factors.

## Draft Literature Review: Delivery Pressure, Understanding, and Agent Context

Research update: [[Week 06 - AI Coding Proposal Research Gap Check]] identifies closer studies than those in this initial draft, including a controlled pressure comparison, repository-change experiments, and a late-requirement study. The question remains unchanged, but the final review must integrate this evidence. Do not claim that pressure in AI-assisted coding or AI-supported requirement changes is unstudied.

### Delivery pressure and quality before coding agents

Earlier research provides a basis for examining how deadline demands affect software work. Austin (2001) models developers who value quality but may take shortcuts when they fear the consequences of missed deadlines. His explanation concerns competing incentives, rather than a lack of concern for quality. It also predicts that the relationship depends on deadline-setting policies; it does not establish a universal rule that tighter deadlines produce worse software. Kuutila et al. (2020) reviewed 102 papers and found that most high-quality studies reported higher productivity and lower quality under time pressure. However, the review also identified conflicting findings and called for closer attention to study settings. These sources justify studying pressure while leaving its effect in a specific agent-supported task open to testing.

### Automation changes the work people must oversee

The possibility that automation creates new demands on people predates generative AI. Bainbridge (1983) explains how automating industrial processes can leave human operators responsible for difficult or abnormal situations. Applying that argument to coding agents suggests that producing code and judging its suitability require distinct forms of work. This application is a proposed explanation, since Bainbridge did not study software agents. Early evidence from coding assistants also shows that assistance serves different purposes. Barke et al. (2023), observing 20 programmers, distinguished using Copilot to accelerate a known approach from using it to explore an unfamiliar task. Agent explanations may therefore help developers form an understanding, while code generation alone may leave that understanding incomplete.

### Evidence about understanding and context

Recent research examines this concern more directly. Shen and Tamkin (2026) studied 52 developers learning an unfamiliar Python library. AI assistance reduced subsequent mastery scores, while the average improvement in completion time was not statistically significant. Their analysis also identified interaction patterns associated with stronger learning, including seeking explanations. Those patterns were not randomly assigned, so they do not establish that a particular prompting style causes better understanding. The study used a chat assistant and short library tasks, which limits direct transfer to repository-level coding agents.

Ahmad (2026) provides complementary evidence from 621 reflective diaries written by 207 students over eight weeks. The study describes accepting generated code without understanding it, mismatches between suggestions and project context, and weak verification. It also describes students using AI to build understanding. These accounts show that AI use can support or hinder comprehension, but self-reports from student projects do not isolate the effect of delivery pressure. Jiang and Nam (2026) examine the information developers make available to coding assistants through an analysis of rule files in 401 repositories. Their categories include project information, conventions, guidelines, model directives, and examples. This identifies context provision as a concrete activity, without proving that adding rules improves outcomes or that pressure reduces their quality.

### A possible shift in the sources of risk

Storey (2026) offers a conceptual account that connects these findings. Her model distinguishes problems in code, gaps in a team's shared understanding, and missing records of goals, constraints, and design reasons. It suggests that code quality alone cannot capture all risks when people and agents change a system. The model is an emerging conceptual framework, not an experimental demonstration of effects, and its team-level concepts should not be treated as established measures of an individual's performance. It nevertheless helps explain why an agent can produce a plausible change that a developer cannot adequately assess against the business need.

Together, these sources motivate a specific question about delivery pressure during changes to an unfamiliar system. The proposed explanation is that pressure may affect time spent understanding existing logic, updating relevant context, and checking the generated result. Agents might also offset pressure by explaining dependencies or helping test affected rules. The studies reviewed here do not directly establish which effect dominates when both groups use the same agent to implement a revised business requirement. This is the candidate gap for the proposal, subject to further searching in requirements-change and repository-comprehension research. The study would test pressure within agent-supported work; it would not establish a historical shift from human coding to agent supervision without a further comparison.

## Source Roles and Limits

| Source | Role in the argument | Evidence and caution |
| --- | --- | --- |
| Austin (2001) | Deadline incentives and quality choices | Published formal model; do not describe it as a field experiment. |
| Kuutila et al. (2020) | Historical evidence on pressure | Published systematic review; findings vary by task and setting. |
| Bainbridge (1983) | Why supervision remains demanding | Published conceptual paper on industrial automation; its application here needs justification. |
| Barke et al. (2023) | Assistance for known versus unfamiliar work | Published observational study of early Copilot, not current autonomous agents. |
| Shen and Tamkin (2026) | Learning and oversight skills | Research preprint; randomised AI access, not randomised delivery pressure. |
| Ahmad (2026) | Project understanding and verification | Author manuscript with an EASE Companion venue listed; student diary evidence, not a causal test. |
| Jiang and Nam (2026) | Context supplied to coding assistants | MSR paper; describes context content rather than testing its effectiveness. |
| Storey (2026) | Links code, understanding, and recorded intent | Conceptual preprint; useful framework, not a validated causal model. |

The most recent sources make the topic less novel at the broad level: gaps in understanding and business intent already appear in research. The value must come from the precise pressure comparison, task, and measures, not a claim that no one has noticed these risks.

## Proposed Study Outline

- Randomly assign developers to a shorter or an adequate time allowance after the same setup and initial familiarisation.
- Give both groups the same unfamiliar working repository, original requirements, initial agent context, and business change request.
- Keep model version, tools, repository access, instructions, and starting conversation state consistent; allow normal agent exploration and follow-up questions in both groups.
- Pilot the task to set credible time allowances and check participants' perceived pressure. Record model latency and number of runs because time limits also constrain opportunities to use the agent.
- Score final behaviour with researcher-prepared acceptance checks covering new rules, replacement of obsolete rules, and preservation of valid rules. Use scoring without group labels where feasible.
- Record context corrections, requests for explanations, and observed review or testing. These are supporting process measures, not components of the final behaviour score.
- Consider a short assessment after the task in which participants explain an affected rule or predict its behaviour without AI assistance. Treat this as task understanding, not proof of long-term skill loss.
- Compare outcomes and uncertainty between groups. Use process records to explore possible explanations; associations alone cannot prove that comprehension or context mediates the effect.

This is primarily a quantitative comparison. Coding session events into categories does not automatically make it mixed methods; a separate qualitative analysis would need its own purpose and justification. Participant numbers, recruitment, scoring details, and the exact change remain to be settled.

## Assignment Fit and Word Plan

The rubric allocates 30 marks to the problem, 40 to research synthesis and the question, 15 to initial method justification, and 15 to structure and flow. The main text is 2,000 words, with a 10% allowance; references and compulsory appendices do not count. This working note includes planning material that will not all go into the submission.

| Proposed section | Target words |
| --- | ---: |
| Background and research problem | 350 |
| Literature review, useful theory, and gap | 800 |
| Research question and aims | 100 |
| Research approach and justification | 450 |
| Possible contributions and limits | 300 |
| Total | 2,000 |

Required appendices: RIOT certificate; ChatGPT prompt and selected literature-review output; comparison with the author's review. The Canvas page requests a 100-word discussion, while the [AI guide](https://canvas.lms.unimelb.edu.au/courses/237538/files/27964345?wrap=1) allows about 100–200 words. A 100-word critique meets both. The author must make that comparison against the actual saved response, rather than inventing an AI interaction or a personal critique.

## Next Research Checks

1. Read the full selected papers before finalising the synthesis. This draft uses verified abstracts and selected method, result, discussion, and limitation sections; it is not a completed systematic review.
2. A targeted search is recorded in [[Week 06 - AI Coding Proposal Research Gap Check]], including direct pressure evidence and a maintenance null result. Follow with university database searches and integrate the closest studies before finalising the gap.
3. Add a well-matched source on how developers understand unfamiliar repositories and identify the impact of changed requirements.
4. Verify the final publication records for manuscripts; distinguish peer-reviewed findings, conceptual arguments, and preprints in the submission.
5. Retain one main outcome and a small set of supporting measures so the proposal remains feasible.

## References

Ahmad, M. O. (2026). *Comprehension debt in GenAI-assisted software engineering projects* [Preprint]. arXiv. https://arxiv.org/abs/2604.13277

Austin, R. D. (2001). The effects of time pressure on quality in software development: An agency model. *Information Systems Research, 12*(2), 195–207. https://doi.org/10.1287/isre.12.2.195.9699

Bainbridge, L. (1983). Ironies of automation. *Automatica, 19*(6), 775–779. https://doi.org/10.1016/0005-1098(83)90046-8

Barke, S., James, M. B., & Polikarpova, N. (2023). Grounded Copilot: How programmers interact with code-generating models. *Proceedings of the ACM on Programming Languages, 7*(OOPSLA1), Article 78. https://doi.org/10.1145/3586030

Jiang, S., & Nam, D. (2026). Beyond the prompt: An empirical study of Cursor rules. In *Proceedings of the 23rd International Conference on Mining Software Repositories* (pp. 397–409). Association for Computing Machinery. https://doi.org/10.1145/3793302.3793367

Kuutila, M., Mäntylä, M., Farooq, U., & Claes, M. (2020). Time pressure in software engineering: A systematic review. *Information and Software Technology, 121*, Article 106257. https://doi.org/10.1016/j.infsof.2020.106257

Shen, J. H., & Tamkin, A. (2026). *How AI impacts skill formation* [Preprint]. arXiv. https://arxiv.org/abs/2601.20245

Storey, M.-A. (2026). *From technical debt to cognitive and intent debt: Rethinking software health in the age of AI* [Preprint]. arXiv. https://arxiv.org/abs/2603.22106
