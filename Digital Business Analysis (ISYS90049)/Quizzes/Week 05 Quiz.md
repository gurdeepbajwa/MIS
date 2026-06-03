# Week 05 Quiz

Course: [[Digital Business Analysis (ISYS90049)/Course Overview|Digital Business Analysis (ISYS90049)]]
Source: [[Digital Business Analysis (ISYS90049)/Week 05/Lecture|Week 05 Lecture]]
Linear issue: BAJ-107
Date: 2026-05-11

## Scope

Questions 1-10 are based only on the Week 05 lecture note. These are the questions used for the 80% note-check score.

Questions 11-15 are extension questions. They go beyond the notes and use external research to test transfer, application, and broader professional context. They are not included in the 80% note-check score unless requested.

## Quiz 1

### Note-Based Questions

1. What is the main purpose of problem analysis in business analysis?
   - A. To choose the cheapest technology solution.
   - B. To systematically investigate why a problem exists and what causes it.
   - C. To document every stakeholder request as a requirement.
   - D. To avoid using qualitative evidence.

2. Which term refers to an observable effect of a problem rather than the deeper reason it exists?
   - A. Symptom
   - B. Root cause
   - C. Business need
   - D. Corrective action

3. Explain why jumping to a solution too early can create risk in problem analysis.

4. Which approach is forward-looking and focused on potential problem areas or future opportunities?
   - A. Reactive problem analysis
   - B. Preventive problem analysis
   - C. Post-implementation evaluation
   - D. Transition planning

5. Name three types of evidence that can be used to validate whether a perceived problem is supported by facts.

6. Which item is not one of the key aspects of a problem definition in the Week 05 note?
   - A. Background and context
   - B. Stakeholders
   - C. Potential challenges
   - D. Final software architecture

7. What should a useful problem statement identify?

8. Which limitation of the Five-Why method is described in the Week 05 note?
   - A. It can only be used after a solution is implemented.
   - B. It always produces one objectively correct causal path.
   - C. It is easy to stop at a symptom too early.
   - D. It removes the need for stakeholder involvement.

9. What is the purpose of a fishbone diagram?

10. When is Pareto analysis most useful in problem analysis?
   - A. Before any possible causes have been identified.
   - B. After possible causes have been identified, to prioritise the causes with the greatest frequency or impact.
   - C. Only when no data is available.
   - D. Only for stakeholder attitude analysis.

### Extension Questions

11. ASQ describes Five Whys as a way to drill down into a problem and Five Hows as a way to develop solution detail. In a BA context, why should the analyst usually complete the "why" work before moving into the "how" work?

12. ASQ lists fishbone diagrams and Pareto charts as different cause analysis tools. Which statement best explains their difference?
   - A. Fishbone diagrams organise possible causes into categories, while Pareto charts show which factors are more significant.
   - B. Fishbone diagrams prove the final solution, while Pareto charts replace stakeholder elicitation.
   - C. Fishbone diagrams are only for financial problems, while Pareto charts are only for software problems.
   - D. Fishbone diagrams measure KPIs, while Pareto charts define business needs.

13. IIBA describes root cause analysis as involving problem statement definition, data collection, cause identification, and action identification. What could go wrong if a BA identifies actions before collecting evidence?

14. In a digital business problem, give one example of how operational data and stakeholder interviews might disagree. How should the BA handle that disagreement?

15. A team uses Five Whys and concludes "staff are careless" as the root cause of repeated data-entry errors. What is weak about this conclusion, and what should the BA investigate next?

## Answer Template

Copy this section into your response when you are ready for grading.

```markdown
1.
2.
3.
4.
5.
6.
7.
8.
9.
10.
11.
12.
13.
14.
15.
```

## Grading Notes

- Questions 1-10 are scored out of 10.
- A score of at least 8/10 passes the note-check workflow.
- Questions 11-15 are extension questions and are reviewed separately.
- After grading, weak note-based areas should be used to revise the Week 05 lecture note if needed.

## User Attempt 1

### User Answers

1. B
2. A
3. We could be fixing symptoms of the root cause, meaning the issue is not being found and can continue after a solution is delivered.
4. B
5. Five why, Pareto method and fishbone.
6. D
7. The problem, the affected stakeholders and impact on stakeholders.
8. C
9. Categorise problems into 6 key groups to find the cause of the issue.
10. A
11. We need to understand the why behind a problem before we can move to figuring out how it happens; it helps to speed up finding the how.
12. A
13. The actions may not cover all the problems.
14. Unsure.
15. It assumes the staff are bad at their job. It should instead look at what the staff are doing when they do data entry to find when and where the errors occur, to know if there is a technical issue or bad design that could cause the human to make the error. If multiple staff are facing the issue, then it is likely systemic.

### Note-Based Score

8 / 10 = 80%

Result: Pass. No repeat quiz required.

### Marking

| Question | Mark | Feedback |
| --- | ---: | --- |
| 1 | 1 | Correct. Problem analysis investigates why the problem exists and what causes it. |
| 2 | 1 | Correct. A symptom is the observable effect rather than the deeper cause. |
| 3 | 1 | Correct. You clearly explained the risk of treating symptoms while the underlying issue continues. |
| 4 | 1 | Correct. Preventive problem analysis is forward-looking and proactive. |
| 5 | 0.25 | Mostly incorrect. Five Why, fishbone, and Pareto are techniques, not evidence types. Stronger examples: interviews, workshops, focus groups, surveys, operational data, customer data, employee data, and system reports. |
| 6 | 1 | Correct. Final software architecture is not part of the problem definition. |
| 7 | 1 | Correct. A problem statement should identify the problem, affected stakeholders, and impact. |
| 8 | 1 | Correct. A Five-Why analysis can stop at a symptom too early. |
| 9 | 0.75 | Mostly correct. A fishbone diagram organises possible causes into categories. The 6M categories are common but not mandatory; categories can be adapted to the situation. |
| 10 | 0 | Incorrect. Pareto analysis is most useful after possible causes have been identified, so the analyst can prioritise the causes with the greatest frequency or impact. |

### Extension Review

| Question | Review |
| --- | --- |
| 11 | Partly correct. The stronger point is that "why" identifies the problem/root cause, while "how" develops solution detail. Moving to "how" too early risks designing a solution for the wrong problem. |
| 12 | Correct. Fishbone diagrams organise possible causes; Pareto charts show which factors are more significant. |
| 13 | Correct but brief. A fuller answer would say actions may target assumptions, symptoms, or incomplete causes because they were not grounded in problem definition and evidence. |
| 14 | No answer. Example: interviews may suggest the CRM is slow for everyone, while system logs show the delay only occurs for one team during batch uploads. The BA should investigate the discrepancy, check data quality, segment users, and triangulate with more evidence. |
| 15 | Strong answer. You correctly challenged blame-based reasoning and moved toward system, process, interface, workload, training, and design causes. |

### Weak Areas

- Distinguish evidence sources from analysis techniques. Techniques help analyse the problem; evidence sources provide the information being analysed.
- Pareto analysis does not discover root causes by itself. It is used after possible causes are known, to prioritise the causes with the greatest frequency or impact.
- For extension questions, use a concrete example even when uncertain. A partial example is better than leaving the answer blank.

### Revisions Made

No Week 05 lecture note revisions were required. The weak areas are already covered in the note.

## Extension Sources

- American Society for Quality. (n.d.). _Five whys and five hows_. https://asq.org/quality-resources/five-whys
- American Society for Quality. (n.d.). _Cause analysis tools_. https://asq.org/quality-resources/root-cause-analysis/tools
- International Institute of Business Analysis. (n.d.). _Business analysis tips for avoiding failure rates - Part 2_. https://www.iiba.org/business-analysis-blogs/business-analysis-tips-for-avoiding-failure-rates---part-2/
