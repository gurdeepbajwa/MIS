# Appendix B source: Luna literature review response

- Model: GPT-5.6 Luna (`gpt-5.6-luna`)
- Reasoning effort: Medium
- Date: 13 September 2026
- Context: A fresh sub-agent context without the proposal draft or the preceding conversation.
- Capture: The full final response appears below, unchanged. Its claims and references have not been checked as part of this capture. Apparent errors are retained for comparison.

## Exact prompt

Review the research literature relevant to this question: “How do the number and quality of business requirement changes differ between developers working with and without an AI coding agent within two hours?” Discuss productivity, code quality, developer understanding and work across repositories. Include references and identify a research gap.

## Full AI response — unedited

Literature synthesis for Appendix B

The question is best framed as a gap between established AI-assisted programming research and requirements-engineering research. Existing studies usually measure coding speed, task completion, accepted suggestions, commits, defects, or benchmark success. They rarely measure how developers revise business requirements during a fixed work period.

Productivity findings are mixed and depend on task and developer context. Peng et al. (2023) reported that developers with GitHub Copilot completed a JavaScript HTTP-server task 55.8% faster than the control group. A larger field-experiment paper by Cui et al. (2024) combined three randomised trials involving 4,867 developers and found a 26.08% increase in completed tasks for developers given access to generative AI. These results support a possible increase in the number of implemented changes within two hours.

However, controlled evidence does not show a universal gain. METR’s randomised trial of 16 experienced open-source developers completing 246 real tasks on repositories they knew well found that early-2025 AI tools increased completion time by approximately 19%. Developers spent less time writing and searching, but more time prompting, waiting, reviewing, and correcting generated output. This is directly relevant to a two-hour comparison because the agent may increase the volume of proposed changes while reducing the number of verified, business-valid changes completed.

Code quality is also multidimensional. Imai (2022) found that Copilot increased lines of code added but produced more subsequent deletions than human pair programming, suggesting that apparent output volume may conceal rework. Nguyen and Nadi (2022) evaluated Copilot suggestions across 33 LeetCode problems and four languages. Correctness varied substantially by language, with Java suggestions scoring highest at 57% and JavaScript lowest at 27%; they also identified unnecessary complexity and undefined helper methods. Pearce et al. (2022) found that Copilot could generate security-vulnerable code in scenarios where vulnerabilities were possible. These studies suggest that “quality” should include correctness against acceptance criteria, requirement coverage, maintainability, security, and the amount of rework—not only lines changed or number of commits.

Developer understanding is a likely mechanism behind differences in requirement-change quality. Barke et al. (2023) identified two interaction modes: “acceleration,” where the developer already knows the solution and uses AI to implement it faster, and “exploration,” where the developer uses AI to investigate possible solutions. Exploration may help developers generate more alternatives and expose missing requirements, but it can also produce plausible code that the developer does not fully understand. Vaithilingam et al. (2022), in a within-subject study of 24 programmers, found that Copilot often supplied a useful starting point and reduced web searching, but participants had difficulty understanding, editing, and debugging longer generated snippets. This supports measuring developer understanding directly, for example through post-task explanations, confidence calibration, or the ability to identify defects and explain how each change satisfies a business requirement.

Repository context is important. SWE-bench (Jimenez et al., 2024) evaluates agents on real GitHub issues at repository level, using tests to assess whether a patch resolves the issue. SWE-agent (Yang et al., 2024) similarly treats software engineering as an agent interaction with a repository rather than isolated code generation. More recent work on SWE-Explore separates repository exploration, context retrieval, code localisation, and diagnosis from final patch success. These studies show that repository-wide work requires navigation, dependency reasoning, and integration. They do not, however, examine whether human developers make better business decisions when an agent can inspect one or more repositories. The multi-repository setting may increase the agent’s access to context but also increase review burden, cross-repository inconsistency, and the risk of importing unsuitable patterns.

Requirements-engineering research provides the conceptual basis for the dependent variable. Requirements volatility refers to the number, direction, and impact of requirement changes over time. Empirical studies associate poorly controlled requirement changes with rework, delay, increased complexity, and quality degradation. A change-count measure alone is therefore insufficient: a high number may indicate productive refinement, or it may indicate misunderstanding and churn. The study should classify changes as, for example, clarification, addition, deletion, modification, or reversal, and assess quality using criteria such as clarity, consistency, completeness, traceability to business goals, feasibility, and stakeholder acceptance.

A clear research gap remains:

> There is little controlled evidence comparing developers with and without an AI coding agent on the number and quality of business-requirement changes produced within the same short time window, especially when the task requires work across repositories. Existing AI studies focus mainly on code output and speed, while requirements-volatility studies generally do not isolate AI assistance. The relationship between developer understanding, repository context, code quality, and requirement-change quality is therefore unresolved.

A suitable study contribution would be to compare both conditions within two hours and record:

- number of requirement changes proposed and accepted;
- change type and scope;
- requirement quality scores from blinded reviewers;
- code correctness and test results;
- rework, rejected changes, and defects;
- developer understanding and confidence;
- repository navigation and cross-repository integration effort.

Potential hypotheses should remain cautious:

- AI access may increase the number of proposed requirement changes.
- AI access may increase the number of implemented changes only when repository context is clear and tasks are familiar.
- AI access may reduce average requirement quality when developers accept generated solutions without sufficient review.
- Developer understanding and review effort may mediate the relationship between AI access and change quality.
- Multi-repository tasks may reduce or reverse productivity gains because context gathering and integration increase.

References

Barke, S., James, M. B., & Polikarpova, N. (2023). Grounded Copilot: How programmers interact with code-generating models. *Proceedings of the ACM on Programming Languages, 7*(OOPSLA1). https://arxiv.org/abs/2206.15000

Cui, C., Demirer, M., Jaffe, S., Musolff, L., Peng, S., & Salz, T. (2024). The effects of generative AI on high-skilled work: Evidence from three field experiments with software developers. https://mit-genai.pubpub.org/pub/v5iixksv

Imai, S. (2022). Is GitHub Copilot a substitute for human pair-programming? An empirical study. *2022 IEEE/ACM  b19th International Conference on Software Engineering: Companion Proceedings*, 384–386. https://doi.org/10.1109/ICSE-Companion55297.2022.9793778

Jimenez, C. E., Yang, J., Wettig, A., Yao, S., Pei, K., Press, O., & Narasimhan, K. (2024). SWE-bench: Can language models resolve real-world GitHub issues? *International Conference on Learning Representations*. https://arxiv.org/abs/2310.06770

Model Evaluation & Threat Research. (2025). *Measuring the impact of early-2025 AI on experienced open-source developer productivity*. https://metr.org/Early_2025_AI_Experienced_OS_Devs_Study-paper.pdf

Nguyen, N., & Nadi, S. (2022). An empirical evaluation of GitHub Copilot’s code suggestions. *2022 IEEE/ACM 19th International Conference on Mining Software Repositories*, 1–11. https://doi.org/10.1145/3524842.3528470

Pearce, H., Ahmad, B., Tan, B., Dolan-Gavitt, B., & Karri, R. (2022). Asleep at the keyboard? Assessing the security of GitHub Copilot’s code contributions. *Communications of the ACM, 65*(12), าส  - 70–73. https://doi.org/10.1145/3610721

Peng, S., Kalliamvakou, E., Cihon, P., & Demirer, M. (2023). The impact of AI on developer productivity: Evidence from GitHub Copilot. *arXiv*. https://arxiv.org/abs/2302.06590

Vaithilingam, P., Zhang, T., & Glassman, E. L. (2022). Expectation vs. experience: Evaluating the usability of code generation tools powered by large language models. *CHI Conference on Human Factors in Computing Systems Extended Abstracts*, 1–7. https://doi.org/10.1145/3491101.3519665

Yang, J., Jimenez, C. E., Wettig, A., Yao, S., Press, O., & Narasimhan, K. (2024). SWE-agent: Agent-computer interfaces enable automated software engineering. *Advances in Neural Information Processing Systems, 37*. https://arxiv.org/abs/2405.15793
