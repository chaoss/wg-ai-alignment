# Feedback Channel Effectiveness

**Question:** To be added.

## Overview

This metric is part of the [AI Alignment - Community Aligned Training (Feedback)](metric-model-ai-alignment-community-aligned-training-feedback.md) metrics model, which measures whether a community can give feedback to a model builder and see its impact, as the means by which alignment with that community increases.

Determine whether or not feedback was effectively resolved to the satisfaction of governance agreement (for community and/or model builder).

Determine whether feedback was in scope, and if so, whether it produced an observable change (in model behavior, policy, attribution, compensation, reciprocal contribution, or community-facing tooling), and whether that change persists.

| Indicator | Implementation | Measurable now? |
| --- | --- | --- |
| Model behavior changed | Re-test the behavior against the model; read changelogs, model and system cards | Yes |
| Policy changed | Review provider policy pages, contribution rules, and model-card updates | Yes |
| Community posture changed | Track the community’s own policy, bounty, or moderation changes after the outcome | Yes |
| Change persisted | Re-test across later releases to confirm it didn’t silently revert | Yes |
| Attribution given | Look for the change credited to community feedback in changelogs or cards | Not yet |
| Compensation | Public records and self-report: grant, contract, sponsorship, or paid time | Not yet |
| Reciprocal contribution   | Track provider contributions back to the project (code, fixes, infrastructure, roadmap seat) | Not yet |

Existing CHAOSS metrics to draw on: [Change Request Acceptance Ratio](https://www.chaoss.community/kb/metric-change-request-acceptance-ratio/), [Change Requests Accepted](https://www.chaoss.community/kb/metric-change-requests-accepted/), [Time to Close](https://www.chaoss.community/kb/metric-time-to-close/), [Change Requests Duration](https://www.chaoss.community/kb/metric-change-requests-duration/), [Review Cycle Duration within a Change Request](https://www.chaoss.community/kb/metric-review-cycle-duration-within-a-change-request/), [Change Request Closure Ratio](https://www.chaoss.community/kb/metric-change-request-closure-ratio/)

## Want to Know More?

### Data Collection Strategies

Known methods (as of this writing) for collecting data related to this metric.

| Attribute | How we'd collect it | Detectable today? |
| --- | --- | --- |
| Model behavior changed | Community self-report, model and system cards | Yes |
| Policy changed | Provider changelogs, model-card updates | Yes |
| Community posture changed | Detect change in community AI usage  and moderation policies | Yes |
| Change persisted | Community self-report, provider changelogs, model-card updates | Yes |

### Filters

- **Channel type:** provider intake, community channel, foundation liaison, none documented
- **Change type:** accuracy / factuality, safety, bias / discriminatory, privacy, agent behavior, environmental impact, accessibility, attribution / provenance, licensing / compliance, financial cost (keep in sync with [Metric: AI Alignment Feedback](https://github.com/chaoss/wg-ai-alignment/blob/main/metrics/ai-alignment-community-feedback/ai-feedback-channel-quality.md))
- **Outcome** change  
- **Persistence** temporary, current, deprecated, removed
- **Lean:** both care, leans community, leans provider
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

Add your name if you contributed

## Additional Information

To edit this metric please submit a Change Request here: (replace with correct link once metric is added to a focus area repo)

To reference this metric in software or publications please use this stable URL: (replace with permalink once published)
