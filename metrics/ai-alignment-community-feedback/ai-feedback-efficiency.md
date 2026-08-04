# Feedback Channel Efficiency

**Question:** To be added.

## Overview

This metric is part of the [AI Alignment - Community Aligned Training (Feedback)](metric-model-ai-alignment-community-aligned-training-feedback.md) metrics model, which measures whether a community can give feedback to a model builder and see its impact, as the means by which alignment with that community increases.

Measures the cost of the loop to each side. On the community side, the effort to give feedback and the wait for a response. On the model-builder side, the effort and cost to respond and implement. Neither side's time is free.

Capture what the loop costs both communities and builders, so proportionality can be judged. A channel that technically exists but is expensive for a community to use, or slow and costly for a provider to answer, is not a working loop.

|Indicator|Cost to|Implementation|Measurable now?|
|---|---|---|---|
|Effort to give feedback|Identify feedback channel and assign scalar for effort letter|Yes|
|Wait for a response|Timestamps on feedback channel waits|Yes|
|Escalation count|Reopened issues, duplicate issues, reverted statuses  or escalated|Yes|
|Provider effort & cost|Provider|Infer from public timing (time to acknowledgment, time to change, whether it shipped); otherwise provider self-report|Not yet|

Existing CHAOSS metrics to draw on: [Time to First Response](https://www.chaoss.community/kb/metric-time-to-first-response/), [Issue Response Time](https://www.chaoss.community/kb/metric-issue-response-time/), [Labor Investment](https://www.chaoss.community/kb/metric-labor-investment/),  [Collaboration Platform Activity](https://www.chaoss.community/kb/metric-collaboration-platform-activity/)

## Want to Know More?

### Data Collection Strategies

Known methods (as of this writing) for collecting data related to this metric.

| Attribute | How we'd collect it | Detectable today? |
| --- | --- | --- |
| Effort to give feedback | Identify feedback channel and assign scalar for effort | Yes |
| Wait for a response| Timestamps on feedback channel| Yes|
|Escalation count| Reopened issues, duplicate issues, reverted statuses |Yes|

### Filters

- **Effort Level:** low, medium, high, persistent, collective
- **Feedback type:** ◆ quality of contribution, ◆ accuracy / factuality, safety, bias / discriminatory, privacy, ◆ tooling / agent behavior, environmental impact, accessibility, attribution / provenance, licensing / compliance, financial cost
- **Time to response:** never, 1-24 hours, 1-7 days, 1-4 weeks, 1-3 months, 1-4 quarters, 1+ years
- **Escalated:** yes, no
- **Tier:** detectable-today core, standards-we're-asking-for
- **Measurable now:** yes, partly, not yet

### Visualizations

*(model-level visualizations are listed in the metrics model)*

## References

*(see the References section of the metrics model)*

## Contributors

- Emma Irwin
- Coraline Ada Ehmke
- Justin Wheeler
- Adrian Edwards

## Additional Information

To edit this metric please submit a Change Request here: (replace with correct link once metric is added to a focus area repo)

To reference this metric in software or publications please use this stable URL: (replace with permalink once published)
