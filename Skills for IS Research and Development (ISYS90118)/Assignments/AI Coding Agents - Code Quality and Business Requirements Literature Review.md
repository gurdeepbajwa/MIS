# Code quality and business-requirement fit with and without AI coding agents

## Research question

How does the quality of code changes made to meet business requirements differ between developers working with and without an AI coding agent?

## Executive conclusion

The literature does not yet support a simple claim that AI coding agents produce either better or worse code changes overall. The strongest causal evidence concerns AI coding assistants, such as GitHub Copilot and Cursor, rather than newer autonomous agents that can plan, edit files, run tools, and iterate with limited developer input.

Across controlled studies, AI access often improves short-term functional success, task speed, or developers' perception of quality. However, other controlled evidence finds no clear downstream maintainability advantage, and a security-focused experiment found that participants with an AI assistant produced less secure code. Large field studies also show that individual productivity gains do not always become better delivery outcomes.

For business requirements, the most defensible conclusion is conditional: AI can improve the implementation of clear, local, testable requirements, but it does not reliably improve the interpretation of ambiguous requirements, the selection of suitable trade-offs, or the fit between a code change and wider business rules. Human expertise, requirement clarity, tests, review, repository context, and governance appear to moderate the result.

## Scope and terms

“AI coding agent” is used here as an umbrella term. The literature contains at least three different tool types:

1. **Completion assistants** suggest lines or functions in an editor.
2. **Chat-based coding assistants** answer questions, generate code, and help debug or refactor.
3. **Coding agents** plan and carry out multi-step repository work, often using a shell, tests, search, and version-control tools.

Most peer-reviewed evidence compares developers with and without the first two types. Direct evidence about autonomous coding agents in ordinary business software teams remains limited. Results from assistant studies should therefore be treated as related evidence, not direct proof about current agent workflows.

“Code quality” is also multi-dimensional. This review separates:

- **Requirement satisfaction:** whether the change implements the stated functional and non-functional requirements.
- **Internal quality:** readability, complexity, maintainability, test coverage, and security.
- **Delivery quality:** review approval, rework, change failure, incidents, and stability after release.

Passing a unit test is evidence for part of requirement satisfaction. It is not evidence that the requirement was complete, correctly interpreted, secure, usable, or aligned with a wider business process.

## Evidence base

| Study | Design and setting | Main quality or outcome measure | Finding relevant to the question |
|---|---|---|---|
| Peng et al. (2023) | Randomised experiment; 95 professional programmers; JavaScript HTTP-server task | Task success and completion time | Copilot users who completed the task were 55.8% faster. The task-success difference was not statistically significant. This supports speed on a bounded task, not broader business fit. |
| GitHub (2024/2025) | Randomised experiment; 202 developers with at least five years' experience; API endpoints for a web server | Unit tests and blind expert review | Copilot access increased the likelihood of passing all tests by 53.2%. Blind reviewers found better readability, reliability, maintainability, conciseness, and approval likelihood. The study was vendor-led and used one bounded task. |
| Perry et al. (2023) | Controlled user study of security-related programming tasks | Correctness and security-vulnerability classification | Participants with an AI assistant wrote less secure code on most tasks and were more likely to believe their code was secure. Lower trust and more careful prompting were linked to fewer vulnerabilities. |
| Paradis et al. (2024/2025) | Randomised trial; 96 full-time Google engineers; complex enterprise task using internal AI features | Time on task | AI significantly shortened task time by an estimated 21%. The study did not establish that the resulting change better met business requirements or had better long-term quality. |
| Butler et al. (2025) | Mixed-methods workplace study; RCT, telemetry, surveys, and three-week diaries in a multinational company | Usage, perceived usefulness, trust, and work practice | Developers reported positive work changes, but trust in AI-generated code did not improve. Telemetry did not show statistically significant differences in the main productivity comparison. Direct code-quality evidence was limited. |
| Borg et al. (2025 preprint; 2026 journal publication) | Preregistered two-phase experiment; 151 participants, 95% professionals; feature development followed by hand-off and evolution without AI | Completion time, CodeHealth, test coverage, downstream evolution | No significant downstream difference in evolution time or code quality. Bayesian analysis suggested, at most, a small and uncertain CodeHealth benefit for habitual AI users. Developer proficiency mattered more than AI use in some outcomes. |
| Becker et al. (2025) | Randomised field-like experiment; 16 experienced open-source developers; 246 real tasks in familiar mature repositories | Completion time | Early-2025 AI tools increased completion time by 19% despite developers expecting a reduction. This is not a direct quality result, but it shows that AI can add review, prompting, and integration work in complex repositories. |
| DORA (2024) | Large survey of software professionals and organisations | Self-reported code quality and delivery performance | AI adoption correlated with higher reported code quality, but also with lower delivery throughput and stability. The observational design cannot show that AI caused either result. |

## Findings by quality dimension

### 1. Functional requirement satisfaction

The clearest positive result comes from GitHub’s controlled study. Developers with Copilot access were more likely to pass all ten unit tests, and blind reviewers rated their submissions more favourably across several code-quality dimensions. This indicates that an assistant can help developers translate a bounded specification into working code, especially when the task has visible tests and a familiar technical shape.

Peng et al. also found a large completion-time advantage on a standard HTTP-server task, but the difference in task success was not statistically significant. The result therefore supports faster implementation more strongly than higher correctness.

These studies have limited reach for business requirements. Their tasks provide a short, explicit specification and a fixed test suite. Real requirements often include incomplete rules, stakeholder disagreement, legacy constraints, data ownership, approval rules, service-level targets, and exceptions that do not appear in visible tests. A model can produce code that passes the available tests while implementing the wrong interpretation of the business need.

The literature therefore supports this narrower proposition: AI assistance can raise the probability of satisfying a well-specified, locally testable requirement. It does not yet establish a general gain in requirements traceability or business acceptance.

### 2. Readability, maintainability, and technical debt

The GitHub study reports small but statistically significant improvements in readability, reliability, maintainability, and conciseness, together with a higher approval rate. These results are useful, but they come from one task and from a study run by the tool provider. They measure the submitted artifact soon after creation rather than the cost of maintaining a growing system.

Borg and colleagues provide the most relevant counterweight. Their two-phase design handed code from one developer to another, then asked the second developer to extend it without AI assistance. The study found no significant difference in downstream completion time, code quality, or test coverage between code first developed with and without AI. The authors found a small, uncertain positive maintainability signal for habitual AI users, but Java proficiency had a stronger influence on outcomes.

This suggests that AI-generated code is not automatically harder to maintain, but neither does AI use reliably create maintainability gains. The study also identifies a system-level risk: low-cost code generation can increase code volume, duplicated logic, and architectural clutter even if individual files look clean. This risk matters for business systems because maintainability depends on the whole service, its data flows, and its rules, not only on the local quality of a changed file.

### 3. Security and non-functional requirements

Security is a major weakness in the evidence for unqualified AI adoption. Perry et al. found that participants with an AI assistant produced less secure code on most security tasks. They were also more likely to think their code was secure. The result suggests an automation-bias problem: an answer that looks complete can reduce the developer’s search for security flaws.

Security requirements are often implicit or cross-cutting. They include access control, input validation, secrets handling, privacy, auditability, safe defaults, and abuse resistance. These requirements may not appear in the prompt or the test suite. An agent that optimises for the stated feature can therefore satisfy the visible function while missing the risk boundary around it.

The practical implication is that security checks must remain independent of the agent. Static analysis, dependency checks, threat-focused tests, code review by a suitably skilled person, and production monitoring should not be replaced by the agent’s own claim that the change is safe.

### 4. Review quality and delivery outcomes

The evidence is mixed because faster code production can move the bottleneck to review, testing, integration, or release. GitHub’s study found a 5% higher likelihood that reviewers would approve Copilot-authored code. DORA’s 2024 survey found positive associations between AI adoption and reported code quality, but negative associations with software delivery throughput and stability.

The DORA result is not a causal test: teams that adopt AI may differ from teams that do not, and adoption may coincide with other process changes. Still, it is important because it measures the delivery system rather than an isolated coding task. It implies that better local code production does not guarantee better product outcomes.

METR’s 2025 randomised study reaches a related conclusion from a different setting. Experienced maintainers working in repositories they knew well took 19% longer with early-2025 AI tools. The study did not show that the final code was worse, but it demonstrates that an agent can impose context-loading, prompting, verification, and rework costs. Those costs are likely to be higher when the business requirement is ambiguous or the repository contains rules that are not well represented in the available context.

## Why findings differ

The variation across studies is not surprising. The treatment is not one stable technology, and the task is not one stable kind of work. Important moderators include:

- **Requirement clarity:** explicit acceptance criteria favour AI; ambiguous or conflicting requirements favour experienced human judgement.
- **Task locality:** a self-contained endpoint or refactor is easier for an assistant than a cross-service change with hidden dependencies.
- **Repository familiarity:** AI may help with unfamiliar code, but experienced maintainers may already hold a better mental model than the agent can recover from files and prompts.
- **Developer skill and AI skill:** developers need enough technical knowledge to test, challenge, and revise suggestions. The maintainability study found human language proficiency and AI proficiency both mattered, with human technical proficiency often stronger.
- **Verification strength:** visible tests, static analysis, review, and staged release reduce the chance that plausible but wrong code reaches production.
- **Tool mode:** autocomplete, chat, and autonomous agents create different amounts of generated code, context loss, and human oversight.
- **Outcome horizon:** immediate test success may improve while long-term complexity, security exposure, or rework worsens.

The central causal model supported by the evidence is not “AI causes quality.” It is closer to:

> AI changes the distribution of developer effort. It can reduce typing and search effort, while increasing effort for requirement translation, checking, integration, and review. The net quality result depends on which of those activities the workflow supports and measures.

## Assessment of the research gap

The specific question about code changes made to meet business requirements remains under-tested. Current studies commonly use one of four substitutes:

1. a fixed programming task;
2. unit-test or benchmark success;
3. static quality measures such as complexity or maintainability; or
4. developer perception and delivery telemetry.

Few studies connect all of the following in one design: a real business requirement, traceability from requirement to acceptance criteria, implementation by developers with and without an agent, independent review, security and maintainability analysis, and post-release business outcomes. Autonomous coding agents are especially under-represented. The maintainability study explicitly calls for work on third-generation agents and for longitudinal studies.

## Recommended research design for this question

An informative study should use a randomised or well-matched comparison of developers working on equivalent, real requirements. It should record the tool and model version, developer experience, prompt and interaction patterns, repository context, and the amount of generated code that remains after review.

The outcome should be a quality vector rather than one score:

| Outcome | Suggested measure |
|---|---|
| Requirement fit | Blind business-owner rating against acceptance criteria; traceability matrix; missed and invented requirements |
| Functional correctness | Hidden tests, boundary cases, and scenario-based acceptance tests |
| Non-functional fit | Security, privacy, performance, accessibility, reliability, and compliance checks relevant to the domain |
| Internal quality | Independent review, CodeHealth or equivalent, complexity, duplication, test quality, and documentation |
| Change sustainability | Time and defects when a second developer changes the code later |
| Delivery quality | Review iterations, rework, rollback, escaped defects, incident rate, and lead time |
| Human factors | Developer confidence calibration, understanding of the change, cognitive load, and ability to explain design choices |

The study should stratify by task type: routine local change, cross-component feature, ambiguous requirement, security-sensitive change, and legacy-system change. It should also compare an agent with a defined verification workflow against an agent used without such controls, because the workflow is part of the treatment in real organisations.

## Overall answer

Developers working with an AI coding agent may produce code changes that are more functional, readable, or quickly completed when the business requirement is clear, local, and well covered by tests. The evidence does not show a stable advantage across all code-quality dimensions. Maintainability results are mostly null or small and uncertain; security results raise a material risk; and production studies show that local productivity gains can fail to improve delivery stability.

The best current answer is therefore: **AI agents appear to improve some forms of implementation quality under strong specification and verification, but they do not reliably improve business-requirement fit. Their effect shifts from positive to neutral or negative as requirements become ambiguous, cross-cutting, security-sensitive, or dependent on deep repository and domain knowledge.**

## Sources

Becker, J., Rush, N., Barnes, E., & Rein, D. (2025). *Measuring the impact of early-2025 AI on experienced open-source developer productivity*. arXiv. https://arxiv.org/abs/2507.09089

Borg, M., Hewett, D., Hagatulah, N., Couderc, N., Söderberg, E., Graham, D., Kini, U., & Farley, D. (2026). Echoes of AI: Investigating the downstream effects of AI assistants on software maintainability. *Empirical Software Engineering, 31*, Article 161. https://doi.org/10.1007/s10664-026-10889-1

Butler, J., Suh, J., Haniyur, S., & Hadley, C. (2025). Dear diary: A randomized controlled trial of generative AI coding tools in the workplace. In *2025 IEEE/ACM 47th International Conference on Software Engineering: Software Engineering in Practice*. https://www.microsoft.com/en-us/research/publication/dear-diary-a-randomized-controlled-trial-of-generative-ai-coding-tools-in-the-workplace/

DORA. (2024). *Accelerate State of DevOps report 2024*. Google Cloud. https://dora.dev/research/2024/dora-report/

GitHub. (2025, February 6). *Does GitHub Copilot improve code quality? Here’s what the data says*. https://github.blog/news-insights/research/does-github-copilot-improve-code-quality-heres-what-the-data-says/

Paradis, E., Grey, K., Madison, Q., Nam, D., Macvean, A., Meimand, V., Zhang, N., Ferrari-Church, B., & Chandra, S. (2024). *How much does AI impact development speed? An enterprise-based randomized controlled trial*. arXiv. https://arxiv.org/abs/2410.12944

Peng, S., Kalliamvakou, E., Cihon, P., & Demirer, M. (2023). The impact of AI on developer productivity: Evidence from GitHub Copilot. arXiv. https://arxiv.org/abs/2302.06590

Perry, N., Srivastava, M., Kumar, D., & Boneh, D. (2023). Do users write more insecure code with AI assistants? In *Proceedings of the 2023 ACM SIGSAC Conference on Computer and Communications Security*. https://doi.org/10.1145/3576915.3623157
