# Week 06 AI Coding Proposal: Research Gap Check

- Course: Skills for IS Research and Development (ISYS90118)
- Checked: 7–8 September 2026; follow-up on 10 September 2026 (see below)
- Parent: [[Week 06 - Delivery Pressure and AI Coding Research Proposal]]
- Status: Targeted scoping check, not a systematic review or proof that no matching study exists.
- Reading depth: Checked primary-source abstracts and selected study designs, task descriptions, results, limitations, and references. Not every paper or appendix has been read in full. Kong et al. was accessible through publisher abstracts and section extracts only.
- Drafting support: Codex searched, compared sources, and drafted this working record. The author should inspect the priority papers before using the synthesis in the assignment.

## Follow-up Check — 10 September 2026

### Verdict

The proposed question remains plausible as a focused empirical extension, not a confirmed first study. The wider literature already covers AI-supported changes, developer understanding, timed programming, and regression checks across changing specifications. The contribution should concern the effect of shorter deadlines on final change correctness while a human developer continues to work with an agent.

The earlier 7–8 September check above did exist. The later chat statement that we had not searched beyond the selected papers understated that work. This follow-up expands it; neither check amounts to a systematic review.

### Closest Additional Evidence

| Study | Design and overlap | What it does not answer |
| --- | --- | --- |
| [Balepur et al. (2026), *(Im)Paired Programming*](https://arxiv.org/html/2607.26375v1), Sections 3–4 | 54 students built a website with an agent or restricted chatbot, then extended their own code with the chatbot. Initial and extension limits were 50 and 20 minutes for everyone. Agent users had weaker comprehension; overall extension accuracy was similar, with results depending on initial code quality and comprehension. | Varies initial AI support, not deadline length. The later task removes agent support. Do not claim agent users simply failed more extensions, or that the extension used no AI. |
| [Shen et al. (2026), *EvoCode-Bench*](https://arxiv.org/html/2605.24110v1), Sections 3.4 and 4.3; Appendix B.5 | Automated agent evaluation across evolving requirements. It checks new and still-active requirements and identifies stale superseded behaviour. | No human deadline comparison. Our new/obsolete/unchanged-rule scoring is an adaptation of existing evaluation ideas, not a novel measure. |
| [Shastry et al. (2026), *Beyond Isolated Tasks*](https://arxiv.org/html/2604.03035v1) | SWE-STEPS evaluates dependent repository changes, including tests of new functionality and regression tests. | Automated agent benchmark, not an experiment on developers under different time allowances. |
| [Gardella et al. (2026), *Relationships Between Trust, Compliance, and Performance*](https://arxiv.org/html/2604.18948v1), Section 2 | 27 novices used Copilot for timed Python function tasks. The analysis relates trust, suggestion acceptance and performance. | All analysed blocks had 20-minute limits. It does not vary pressure or test business changes in an inherited repository. Data came from 2023–2024 tools. |
| [Joshi (2026), *Modeling Learner-AI Interaction in Time-Constrained Programming Tasks*](https://educationaldatamining.org/edm2026/proceedings/2026.EDM.doctoral-consortium-papers.459/index.html), Sections 5–6 | Doctoral-consortium proposal for timed/untimed algorithmic programming, interaction logs and correctness. It cites preliminary studies. | This is planned research, not completed evidence for the proposed pressure comparison. It also shows that pressure and correctness are not an untouched research direction. |
| [Ye et al. (2026), *Coding with “Enemy”*](https://arxiv.org/html/2606.05647v1), Sections 3–4 | Human participants worked with agents on sequential tasks in an existing system for about five hours. The study tested deliberate sabotage and a monitor condition. | It varies model/monitor conditions, not deadlines. Deliberately malicious changes differ from ordinary requirement errors. Do not infer a pressure effect from its discussion. |

Balepur, Shen, Shastry, Gardella and Ye are cited here as preprints, not as verified final peer-reviewed publications. The Joshi item is a conference doctoral proposal.

### Other Leads and Access Limits

- [Joshi et al. (2025), competitive programming](https://link.springer.com/chapter/10.1007/978-3-031-99261-2_17): followed from Joshi (2026), reference 9. Publisher abstract describes contests and 18 participants. Full chapter was subscription-only; no claim of a verified deadline manipulation.
- [Kong et al. (2025)](https://www.sciencedirect.com/science/article/pii/S092054892500042X): the indexed publisher record again supports the existence of AI-supported requirements-change work. Direct full-page access returned 403. Retain the earlier access limit; do not treat a title or abstract as a full methods check.
- [SWE-EVO](https://arxiv.org/abs/2512.18470) and [SlopCodeBench](https://arxiv.org/abs/2603.24755): screened as further evidence that evolving specifications and maintenance already have benchmark research. Abstract-level screening only in this pass; no numerical claims adopted.
- [Agent instruction maintenance](https://arxiv.org/abs/2606.25257): screened as adjacent work on context-file evolution, not direct evidence about human deadline effects.
- [Hackathon interviews](https://arxiv.org/abs/2607.29178): abstract screened; relevant to verification under time and knowledge limits, but not a controlled pressure experiment.

Version caution: the EvoCode-Bench authors' [repository](https://github.com/UniPat-AI/EvoCodeBench) reports corrected evaluation releases, including withdrawn results affected by verifier access. This note and the proposal use the evaluation design, not leaderboard percentages. Pin and recheck the paper/code release before adopting any numerical result.

### Citation Tracing Actually Completed

- Forward connection: Balepur et al. cites Shen and Tamkin (2026) in its related work and contrasts skill learning with understanding one's own code. This provides a closer extension-task study than the learning paper alone.
- Backward connection: Joshi (2026), reference 9, led to the 2025 Springer competitive-programming chapter. Its abstract and source record were checked, but the full chapter was not accessible.
- Related-work checks: inspected the related-work sections of Balepur and EvoCode-Bench and screened nearby software-evolution benchmarks.
- Exact-title/identifier searches for Offloading Score and the earlier agent-workflow paper provided limited further leads. No complete forward-citation export was obtained.

This is selected citation tracing, not exhaustive snowballing.

### Search Coverage

The follow-up used 23 web-search queries, plus primary-source openings, targeted section checks and reference tracing. Selected queries used domain filters for arXiv, ACM, IEEE and Springer. These were web searches, not authenticated searches within Scopus, Web of Science, ACM Digital Library or IEEE Xplore. Search rankings and missing indexed text limit what absence can establish. No complete deduplicated screening count is claimed.

Queries run in this follow-up:

1. AI coding agents time pressure requirements changes experiment developer understanding
2. AI assisted programming maintenance requirement changes time pressure experiment
3. coding agents requirements evolution regression developer study
4. "coding" "time pressure" "AI" study deadline developer
5. "program comprehension" "AI" "time pressure"
6. "EvoCode-Bench" arxiv
7. "SlopCodeBench" arxiv
8. "AI" "deadline" "requirements" "controlled experiment" developers
9. "coding agents" "time pressure" -site:reddit.com -site:linkedin.com
10. "Collaboration with Generative AI to improve Requirements Change"
11. "EvoCode-Bench" "arxiv.org/abs"
12. "Offloading Score" "time" "coding" -site:reddit.com -site:codex.danielvaughan.com
13. "Code with Me or for Me" "pressure"
14. "Collaboration with generative AI to improve requirements change" Kong Zhang
15. "AI Coding Assistants in Competitive Programming" Joshi
16. "Coding With" "Enemy" "Sabotage" study
17. "AI" "time pressure" "maintenance" study
18. "AI-assisted" "requirement changes" "time pressure"
19. "coding agent" "deadline" "experiment" developers requirements
20. "coding" "time pressure" "correctness" experiment AI
21. "2605.29392" -site:reddit.com -site:codex.danielvaughan.com
22. "2507.08149" "2607.26375"
23. "Requirements after the first edit" "time pressure"

### What Changes in the Proposal

- Keep the main question and two-group deadline design.
- Revise the gap to acknowledge changing-requirement benchmarks and human extension-task studies.
- Do not claim novelty for correctness testing or the three rule categories.
- Test the total effect of a deadline on human–agent work. A longer allowance also permits more agent execution; it does not isolate a purely human loss of understanding.
- Keep initial context and familiarisation equal. Do not make the rushed group start with less information.
- Preserve a neutral prediction: agents might help users finish within less time, or reduced time might weaken checking. The study must allow either result.
- Keep incorrect and incomplete submissions as outcomes, with separate rules for technical failures.
- Before submission, run a library-database search and obtain the closest paywalled methods. A direct replication or careful extension can still be worthwhile; an exact unmatched combination is not enough.

The document's gap now cites the two closest additions. The literature review itself has not been broadly rewritten; its next pass should introduce these sources in place of less central detail, rather than keep adding words.

### New References Added to the Proposal

Balepur, N., Baumler, C., Chen, V., Choi, E., Rudinger, R., & Boyd-Graber, J. (2026). *(Im)Paired programming: Coding agents improve productivity but harm understanding* [Preprint]. arXiv. https://arxiv.org/abs/2607.26375

Shen, H., Chen, X., Xu, W., Ma, Y., Chen, L., & Li, K. (2026). *EvoCode-Bench: Evaluating coding agents in multi-turn iterative interactions* [Preprint]. arXiv. https://arxiv.org/abs/2605.24110

These identify the versions checked. Other new leads above have direct primary-source links for follow-up; verify full publication metadata before adding them to the final reference list.

## Decision from the Initial Check

The broad gap does not hold: research already examines pressure in AI-assisted programming, agent-supported repository changes, and changing requirements. The current question can remain as a focused extension, but its contribution must concern the correctness of changes to an existing system under pressure—not simply whether developers use AI more when rushed.

> How does delivery pressure affect developers’ ability to implement business requirement changes in an unfamiliar repository using an AI coding agent?

No directly matching study was identified in this search. That is a bounded search result, not a claim of being first.

## Closest Studies

| Source | What it studies | Why our proposed comparison differs |
| --- | --- | --- |
| Padmakumar et al. (2026), *Offloading Score* | Random assignment of 40 retained freelance developers to one- or four-hour limits for four new web-app tasks, with tools of their choice. A model-derived reliance score was higher under the shorter limit; system recall was also assessed. | Direct pressure overlap. It does not test a fixed agent adapting an inherited repository while preserving existing business rules. Read Sections 4–5 and Appendix E. |
| Chen et al. (2025), *Code with Me or for Me?* | Twenty participants used OpenHands and Copilot for 40 minutes each, with counterbalanced tool order. Tasks included repository bug fixes and feature additions; the study assessed correctness and user experience. | Repository work and correctness already have precedents. The experiment changes the tool, not the time allowance. Read Sections 3–4 and task appendices. |
| Jiang et al. (2026), *Requirements After the First Edit* | A September 2 preprint analyses 3,553 eligible agent sessions. Its reconstructed event sample links late requirements with code replacement. Agent experiments vary disclosure timing and advance warning; final tests supplement the rework measure. | It tests requirement timing/anticipation, not human delivery pressure. Its observed line deletion is not itself proof of a defect or requirement-caused rework. Read Sections 4.2–4.3 and 6. |
| Kong et al. (2025), *Collaboration with Generative AI to improve Requirements Change* | A published method uses ChatGPT-3.5 for modelling, locating affected components, modifying code, and checking properties, illustrated with a real Java system. | AI-supported requirement changes are not new. The accessible material describes a method and application cases, not a controlled developer-pressure comparison. Full methods still need reading. |
| Borg et al. (2026), *Echoes of AI* | A published, preregistered two-phase study reports 151 participants. In its second phase, new developers manually evolve code produced with or without AI. It finds no significant time or code-quality differences in that phase. | A relevant null result and maintenance design. AI provenance is the comparison; pressure is not. Data collection in late 2024 predates widespread coding agents. Read Sections 3, 6, and Appendix A. |
| Miller et al. (2025 manuscript; ICSE 2026 listing) | Interviews with 54 developers in 27 teams at one company describe higher output expectations, tighter deadlines, and limited learning support. | Supports the organisational problem, not a causal test of final business-rule correctness. Read Sections 3, 5.2–5.4, and 6.1. |
| Gardella et al. (2026), *Fast and Forgettable* | Twenty-two novices complete Python tasks with a human partner and with Copilot, for 20 minutes per condition, with a later retest. | A timed study is not necessarily a pressure experiment: this comparison changes the programming partner, not the deadline. Read Section 3. |

Links and APA 7 source records appear below. Preprints remain labelled as such even where their findings closely match the proposal.

## Critical Reading Notes

- **Reliance is not harm.** Padmakumar et al.'s overall reliance–recall correlation is weak (−0.145); it becomes stronger after excluding a high-reliance/high-recall cluster. The score depends on model-generated estimates of human-only work. Do not treat it as a direct measure of thought, or its exploratory threshold as a validated safety limit.
- **Do not discard unsuccessful submissions.** Borg et al. exclude solutions that fail acceptance tests. That suits parts of their maintenance analysis, but would remove a key outcome in our pressure study. Score incomplete and incorrect attempts under a rule set before collecting data; handle technical failures separately.
- **Do not turn rework into a quality score.** A correct requirement change can require deleting many lines. Our primary score should test behaviour, not reward a small patch.
- **Do not infer organisational causes from a task experiment.** A deadline comparison cannot establish that leadership's concern about AI spending caused the pressure, or that engineers personally cared about token costs.
- **Do not equate extra output with extra pressure.** Optional, low-stakes exploration differs from required delivery. Keep task stakes, scope, and choice consistent between experimental groups.

## Defensible Gap and Contribution

The comparison still worth proposing is whether reduced time changes the reliability of a business-rule update when developers and an agent must work within an existing system. In this task, success requires identifying what must change and what must remain valid. Generating more code or recalling its implementation is not the same outcome.

Working gap statement:

> Existing studies examine AI reliance under time limits, developer interaction with coding agents, and software changes. The studies checked here do not directly test whether delivery pressure affects developers' successful adaptation of business rules in an unfamiliar existing repository while preserving valid behaviour. This study proposes a controlled extension focused on that outcome.

This is a modest, focused extension—not a new general theory or a claim that AI creates a wholly new quality problem. An exact combination of factors alone does not justify a study; the business reason is that a change can satisfy the new rule while breaking another rule the organisation still needs.

## Implications for the Proposed Method

1. Keep the original repository, requirements, change request, task stakes, agent version, and tools the same between groups.
2. Vary the time allowance, pilot the difference, and check perceived pressure. A deadline manipulation is one form of delivery pressure, not the whole concept.
3. Assess new rules, obsolete rules that must stop applying, and unchanged rules that must remain valid. Report these components alongside the overall task score so one does not conceal another.
4. Keep process observations secondary: requests for explanations, corrections to context, and review/testing actions. Do not assume more prompting is better or fewer prompts mean less thought.
5. Record agent latency and usage. Extra time also permits more computation; the experiment estimates the total effect of the deadline unless a further design separates these mechanisms.
6. Allow worse, similar, or better final outcomes under the shorter allowance. Do not frame the study as demonstrating harm in advance.

## Search Record and Limits

Searched the web for scholarly sources using combinations of coding agents/AI-assisted programming/Copilot, time or deadline pressure, requirement changes, unfamiliar repositories, maintenance, and controlled experiments. Inspected primary pages from arXiv, publishers, Microsoft Research, and conference records. Followed relevant references from the reliance study. Blog and social-media results served only as leads, not evidence of academic findings.

Representative queries used:

- `"coding agents" "time pressure" study`
- `"AI-assisted" "requirements changes" experiment`
- `"generative AI" developers "deadline" experiment repository`
- `"AI" "software maintenance" "time pressure" study`
- `"developers" "time pressure" "Copilot" experiment`
- `"coding" "time pressure" "LLM" experiment human`
- `"AI-assisted" "change impact" study developers`
- `"programming" "time pressure" "AI" experiment site:arxiv.org`
- `"requirements change" "developers" "LLM" study`
- `"requirement changes" "coding agents" study`
- `"deadline pressure" "Copilot" study experiment`
- `"coding agent" "unfamiliar" "controlled study"`
- `"AI-assisted" "maintenance" "controlled experiment" developers`
- `"coding" "time pressure" "requirement" "experiment" site:dl.acm.org`
- `"AI-assisted" "business requirements" "experiment"`

This was not a structured search inside Scopus, Web of Science, ACM Digital Library, or IEEE Xplore. Domain-filtered web queries do not replace database searches. Search rankings and incomplete indexing can miss relevant studies. No exhaustive screening count or systematic-review label is warranted.

Additional leads screened but not used to establish the gap:

- [Feng et al., junior/senior agent use](https://arxiv.org/abs/2602.00496): junior debugging and senior review; inspected task details showing a common 30-minute task, not a pressure-level comparison.
- [Haduong and Smith, performance pressure](https://arxiv.org/abs/2410.16560): pressure manipulation in spam-review classification, not software changes. Useful method lead; abstract screened.
- [Shen and Tamkin, skill formation](https://arxiv.org/abs/2601.20245): already in the parent note; AI access comparison rather than pressure manipulation.

Before submission: search university research databases with the same concepts, inspect the final versions of priority papers, and rerun the narrow search. Start with Padmakumar et al., Chen et al., and Borg et al.; use the very recent Jiang et al. preprint as emerging evidence rather than the sole basis of the gap.

## References

Borg, M., Hewett, D., Hagatulah, N., Couderc, N., Söderberg, E., Graham, D., Kini, U., & Farley, D. (2026). Echoes of AI: Investigating the downstream effects of AI assistants on software maintainability. *Empirical Software Engineering, 31*, Article 161. https://doi.org/10.1007/s10664-026-10889-1

Chen, V., Talwalkar, A., Brennan, R., & Neubig, G. (2025). *Code with me or for me? How increasing AI automation transforms developer workflows* [Preprint]. arXiv. https://arxiv.org/abs/2507.08149

Gardella, N., Prather, J., Leinonen, J., Denny, P., Pettit, R., & Riggs, S. L. (2026). *Fast and forgettable: A controlled study of novices' performance, learning, workload, and emotion in AI-assisted and human pair programming paradigms* [Preprint]. arXiv. https://arxiv.org/abs/2604.18538

Jiang, B., Cheng, H., Fu, Y., Koziolek, A., Li, J., & Zhang, W. (2026). *Requirements after the first edit: Mining late requirement emergence and rework in real-world coding-agent sessions* [Preprint]. arXiv. https://arxiv.org/abs/2609.03028

Kong, Y., Zhang, N., Duan, Z., & Yu, B. (2025). Collaboration with generative AI to improve requirements change. *Computer Standards & Interfaces, 94*, Article 104013. https://doi.org/10.1016/j.csi.2025.104013

Miller, C., Choudhuri, R., Ulloa, M., Haniyur, S., DeLine, R., Storey, M.-A., Murphy-Hill, E., Bird, C., & Butler, J. L. (2025). *“Maybe we need some more examples:” Individual and team drivers of developer GenAI tool use* [Preprint]. arXiv. https://arxiv.org/abs/2507.21280

Padmakumar, V., Ibrahim, L., Wang, Z. Z., Wang, J., Liao, Q. V., & Yang, D. (2026). *Offloading score: Measuring AI reliance through counterfactual workflows* [Preprint]. arXiv. https://arxiv.org/abs/2605.29392

Version note: Miller et al.'s [Microsoft Research record](https://www.microsoft.com/en-us/research/publication/maybe-we-need-some-more-examples-individual-and-team-drivers-of-developer-genai-tool-use/) lists ICSE 2026 but links to the 2025 arXiv manuscript, including through its DOI link. The reference above identifies the version inspected; verify the proceedings record before citing a final publication. Other preprint labels likewise identify the versions used, not a claim that no later publication exists.
