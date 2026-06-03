# Lecture

Course: [[Digital Business Analysis (ISYS90049)/Course Overview|Digital Business Analysis (ISYS90049)]]
Week: 11
Topic: Solution Evaluation

## Topic

Solution Evaluation

## Key Concepts

### Purpose

Solution evaluation assesses the performance of and value delivered by an existing or implemented solution. It also recommends actions to remove barriers or constraints that prevent full value realisation.

Solution evaluation is not the same as checking whether a project was delivered on time and budget. The business analysis focus is whether the solution creates the intended business value.

The lecture frames solution evaluation as work that occurs after a solution is ready, delivered, implemented, or actively used. The business analyst is usually not responsible for building the solution, but returns to evaluate whether it performs as intended and whether the envisioned future state is being achieved.

Evaluation can continue while the solution remains active. In some organisations the business analyst keeps monitoring value over time; in others, ongoing measurement may be handed to operational owners after the evaluation approach and metrics are established.

### Solution Evaluation Tasks

| Task | Purpose |
| --- | --- |
| Measure solution performance | Define performance measures and use data to evaluate solution effectiveness. |
| Analyse performance measures | Interpret performance data and compare actual performance with expected value. |
| Assess solution limitations | Identify factors internal to the solution that restrict value realisation. |
| Assess enterprise limitations | Identify external organisational factors that restrict value realisation. |
| Recommend actions to increase solution value | Recommend actions to close the gap between potential value and actual value. |

### Measure Solution Performance

Measuring solution performance involves defining and collecting relevant measures.

The analyst should:

- Define accurate and relevant performance measures.
- Validate that measures are suitable.
- Collect performance data.
- Consider data volume or sample size.
- Consider frequency and timing of data collection.
- Consider whether the data is current enough to support evaluation.

Measures can be qualitative or quantitative.

Performance measures should ideally be considered before the solution evaluation stage. Measures are often identified during strategy analysis, future state definition, or requirements analysis, because the analyst needs to know what value the solution is expected to produce before implementation.

Digital solutions can generate large amounts of data, but not all available data is useful. The analyst needs to choose measures that represent the business value expected from the solution. Timing also matters: a measure collected during an unusual seasonal period, a short sample window, or before enough users have adopted the solution may misrepresent actual performance.

### Analyse Performance Measures

Performance analysis asks whether the solution is delivering the desired value.

The analyst should consider:

- Actual solution performance compared with desired value.
- Risks to solution performance.
- Trends in the data.
- Accuracy of performance measures.
- Performance variances between expected and actual results.
- Whether root cause analysis is needed to explain variance.

The lecture emphasises the comparison between expected and actual performance. A gap between the two does not automatically mean the solution has failed. If the solution is new, benefits may appear gradually. An upward trend may justify continued monitoring, while flat or declining performance after several intervals may indicate a limitation that needs action.

### Assess Solution Limitations

Solution limitations are internal factors that prevent the solution from fully realising value.

This may involve:

- Identifying internal dependencies between solution components.
- Investigating solution problems.
- Assessing the severity of problems.
- Assessing probability of recurrence.
- Assessing business impact.
- Assessing whether problems should be resolved, mitigated, or accepted.

A solution may underperform because one component limits the performance of the whole solution.

The transcript distinguishes solution limitations from enterprise limitations. Solution limitations are problems inside the solution itself, such as missing features, weak design, poor integration, incorrect data, a weak component, or a holistic fit problem. Once identified, changes normally need to be reported, assessed, and approved before the solution is altered.

### Assess Enterprise Limitations

Enterprise limitations are organisational factors outside the solution that restrict value realisation.

Examples include:

- Enterprise culture.
- Stakeholder impact.
- Organisational structure.
- Policies and procedures.
- Processes and capabilities.
- Human resources.
- Tools and technology.
- Operational readiness.

The solution itself may be technically sound, but the enterprise may not be able to adapt to or use it effectively.

The lecture treats enterprise limitations as socio-technical problems. A technically working system can still fail to create value if people do not understand it, do not trust it, are not trained to use it, or if organisational culture and processes do not support adoption. Further elicitation may be needed to understand user experience and stakeholder resistance. Training, change management, or process changes may be more appropriate than technical changes.

### Recommend Actions to Increase Value

Recommendations should address the cause of the value gap.

Possible recommendations include:

- Adjust solution performance measures.
- Do nothing where change has low value or high risk.
- Make organisational changes.
- Reduce interface complexity.
- Eliminate redundancy.
- Avoid waste.
- Add missing capabilities.
- Retire the solution.

The goal is to align actual value with potential or intended value.

Recommendations can include changing a feature, adding a feature, changing a policy, improving training, changing a process, doing nothing for the moment, or retiring the solution if it no longer creates value. Solution evaluation is therefore connected to future improvement cycles, not only post-implementation review.

### Continuous Monitoring

Solution evaluation is not a one-off event. Metrics should be evaluated at appropriate intervals, such as weekly or monthly, depending on the solution and context.

Possible monitoring outcomes:

| Situation | Analyst response |
| --- | --- |
| No improvement after one or two intervals | Identify whether there is delay, missing capability, ineffective implementation, or another barrier. |
| Progress as expected | Look for ways to improve benefits or speed up value realisation. |
| Progress better than expected | Investigate success factors so they can be reinforced or reused. |

Continuous monitoring can also start the next improvement initiative.

Monitoring intervals should be chosen deliberately. If there is no improvement after the first interval, the cause may be delayed adoption rather than failure. If expected value is reached, the analyst can still look for further improvement. If value is higher than expected, the analyst should identify success factors so they can be reinforced or reused in future initiatives.

Dashboards and analytics tools can support monitoring, but the dashboard should be customised around meaningful measures rather than filled with whatever data is easiest to display.

### Measures and Metrics

| Concept | Meaning | Example |
| --- | --- | --- |
| Measure | A fundamental or unit-specific value. | Number of customers; number of customers leaving per month. |
| Metric | A value derived from one or more measures. | Churn rate; customer lifetime value. |
| KPI | A key metric that shows how effectively the organisation is achieving important business objectives. | Inventory waste reduction rate; customer retention rate. |

Metrics help answer:

1. How are we doing right now?
2. How do we know this?
3. Where do we want to improve?

Metrics can be used across the BA value spectrum:

- Strategy analysis: assess current state and define target outcomes.
- Requirements analysis and design: define evaluation criteria and requirement quality.
- Solution evaluation: measure actual solution performance and value.

A measure is usually a direct count or value, such as number of customers, website visitors, successful deliveries, or customers leaving in a month. A metric relates measures to time, another measure, or a formula, such as churn rate, conversion rate, average delivery time, percentage of refunded orders, customer lifetime value, or customer acquisition cost.

Customer lifetime value is useful only when interpreted with other metrics. For example, if the cost of acquiring a customer is higher than that customer's lifetime value, the business is not creating profitable customer growth.

### Good Metrics

Good business metrics should be:

| Characteristic | Meaning |
| --- | --- |
| Clear | Precise and unambiguous. |
| Relevant | Aligned with the concern or purpose being measured. |
| Economical | Available at a reasonable cost and effort. |
| Adequate | Provides enough basis to assess performance. |
| Quantifiable | Can be independently validated. |
| Trustworthy and credible | Based on evidence and research. |

Pre-defined metrics can be useful, but they may not fit the organisation's strategy, culture, context, processes, capabilities, or terminology. Analysts may need to adapt or develop metrics.

Metrics can come from customer behaviour, known problems, business objectives, or expected solution value. Where no suitable pre-defined metric exists, the analyst may need to define the data points, formula, tracking interval, and reporting method. The important discipline is to start from the problem, objective, and expected value rather than from the data that happens to be easiest to collect.

### A/B Testing

A/B testing compares two variants of a solution element to see which performs better against a chosen metric. For example, two versions of a checkout button, page layout, message, or process step can be shown to different user groups and compared using conversion, completion, or error metrics.

The better-performing version can then become the baseline for another test. A/B testing is most useful when there is enough traffic or usage volume to produce reliable results. Low sample sizes can make results misleading.

### Metrics and KPIs

Metrics are broad. KPIs are narrower and more strategically important.

The relationship can be understood as:

Goals and objectives -> critical success factors -> KPIs -> metrics -> measures.

A KPI is a measurable value that demonstrates how effectively an organisation is achieving key business objectives. Not every metric is a KPI.

The lecture explains this as a selection process: measures provide raw data, metrics interpret the data, and KPIs are the metrics promoted as key because they directly align with the organisation's goals, objectives, or needs. The same metric may be a KPI in one context and a secondary metric in another.

Business objectives and KPIs are related but not identical. An objective defines the desired target, such as increasing annual recurring revenue by a specified percentage. The KPI is the metric monitored after the solution is live to assess whether progress toward that target is actually occurring.

#### Extra Materials

- [What is a Key Performance Indicator (KPI)?](https://www.youtube.com/watch?v=jvdPM6RZ3Xc) - Balanced Scorecard Institute. Reinforces the difference between measures, metrics, and KPIs when evaluating solution performance and value.
- [The Balanced Scorecard - Measures that Drive Performance](https://hbr.org/1992/01/the-balanced-scorecard-measures-that-drive-performance-2) - Harvard Business Review. Adds the history behind strategic measurement: Kaplan and Norton argued that managers needed more than financial measures, which helps explain why KPIs should connect to customers, internal processes, learning, and business outcomes.
- [Goodhart's law: when waiting times became a target, they stopped being a good measure](https://pubmed.ncbi.nlm.nih.gov/29180439/) - PubMed. Useful caution for solution evaluation: metrics can distort behaviour when people optimise the target instead of the underlying value.
- [History of Benchmarking](https://www.globalbenchmarking.org/index.php/whats-benchmarking/development-of-benchmarking/) - Global Benchmarking Network. Adds background on benchmarking's connection to Xerox and quality improvement, explaining why benchmarking compares performance to practices outside the immediate team.

### Cautions About Metrics and KPIs

Common mistakes include:

- Measuring the wrong element, producing irrelevant KPIs.
- Building dashboards from available data rather than useful data.
- Focusing on data instead of improvement.
- Measuring workers rather than improving processes or solutions.
- Brainstorming KPIs without linking them to goals.

Metrics should support decisions and improvement, not create measurement noise.

The transcript also warns that measurement can distort behaviour. When people are evaluated against a visible metric, they may optimise the metric rather than the underlying value. Metrics about individual work performance can also create privacy, fairness, surveillance, and bias problems if they are used without careful governance.

### Benchmarking

Metrics alone do not show how an organisation compares with others. Benchmarking compares performance against internal units, competitors, industry peers, or world-class performers.

Benchmarking helps establish what "good" performance means when the organisation does not yet have a clear target. It can compare performance against another department, another system, competitors, industry averages, or recognised leaders.

Common benchmarking steps:

1. Choose a process or aspect to compare.
2. Identify relevant comparison candidates.
3. Collect information.
4. Conduct the analysis.
5. Measure gaps and propose improvements.

Benchmarking categories:

| Category | Meaning |
| --- | --- |
| Internal | Compare similar processes within the same organisation. |
| Competitive | Compare with competitors, often through shared or anonymised data. |
| Collaborative | Share quantitative data through industry associations or similar arrangements. |
| Shadow | Use publicly available competitor data. |
| Functional | Compare similar processes outside the industry. |
| World class | Compare processes across industries against leading performers. |

Shadow benchmarking relies on public information, so it can be useful when direct competitor data is unavailable, but it may be incomplete or inaccurate.

## Textbook Connections

Milani Chapter 19 connects directly to solution evaluation. Milani frames evaluation as assessing the business value delivered by the solution, not simply whether the implementation finished.

### Evaluation and Value

Milani explains that a solution has little value if it does not produce the gains that justified the investment. Evaluation asks whether and to what extent objectives have been fulfilled.

The current state, future state, and metrics defined earlier are key inputs. This connects Week 11 back to Week 8 and Week 9 because the ability to evaluate depends on having defined needs, objectives, target value, and measures earlier.

### Data Collection

Milani stresses that performance measures should be planned before evaluation. If the analyst does not consider data collection early, the required data may not be available later.

Important considerations include:

- Sample size and data volume.
- Timing and frequency.
- Seasonal or contextual variation.
- Currency of data.
- Whether the measure is relevant to strategic objectives and business goals.

### Solution and Enterprise Limitations

Milani distinguishes limitations inside the solution from limitations in the enterprise. A solution may not deliver value because of weak internal components, poor integration, lack of functionality, poor usability, inadequate training, organisational resistance, or process misalignment.

This aligns with the lecture's distinction between solution limitations and enterprise limitations.

### Continuous Monitoring

Milani explains that evaluation should happen regularly, not only at the end of a time period. Ongoing monitoring helps the analyst respond when benefits are delayed, missing, progressing as expected, or exceeding expectations.

### Metrics

Milani Chapter 10 connects to the lecture's metrics and KPI material. Milani explains that metrics quantify the current state and help identify where improvement is needed. Metrics should answer how the business is performing, how that is known, and where improvement should occur.

Milani also distinguishes measures, metrics, and KPIs. KPIs are tied to strategic performance, while many metrics may simply track ordinary business processes.

## Summary

- Solution evaluation assesses whether a solution delivers intended business value.
- Evaluation includes measuring performance, analysing results, assessing solution and enterprise limitations, and recommending value-improving actions.
- Metrics should be relevant, clear, economical, adequate, quantifiable, trustworthy, and tied to goals.
- KPIs are strategically important metrics that show progress toward key business objectives.
- Useful KPIs depend on the objective. The same metric can be critical in one context and secondary in another.
- Continuous monitoring helps detect delayed benefits, missing value, and opportunities for further improvement.
- Benchmarking and A/B testing help compare performance and identify practical improvement targets.
- Poorly chosen metrics can distort behaviour, create privacy concerns, or distract from the value the solution was meant to deliver.

## Notes

Reading: Milani Chapters 10 and 19.

References:

- IIBA. (2015). _A guide to the Business Analysis Body of Knowledge_ (3rd ed.).
- Milani, F. (2019). _Digital business analysis_. Springer. https://doi.org/10.1007/978-3-030-05719-0
