# Effectiveness of Feedback

**Question:** To be added.

## Overview

This metric is part of the [AI Alignment - Community Aligned Training (Feedback)](metrics-model-ai-alignment-community-aligned-training-feedback.md) metrics model, which measures whether a community can give feedback to a model builder and see its impact, as the means by which alignment with that community increases.

Determine whether or not feedback was effectively resolved to the satisfaction of governance agreement (for community and/or model builder).

Whether feedback was in scope and if so - did it produce an observable change (in model behavior, policy, attribution, compensation, reciprocal contribution, or community-facing tooling), and whether that change persists.

| Indicator | Implementation | Measurable now? |
| --- | --- | --- |
| Model behavior changed | Re-test the behavior against the model; read changelogs, model and system cards | Yes |
| Policy changed | Review provider policy pages, contribution rules, and model-card updates | Yes |
| Community posture changed | Track the community's own policy, bounty, or moderation changes after the outcome | Yes |
| Change persisted | Re-test across later releases to confirm it didn't silently revert | Yes |
| Attribution given | Look for the change credited to community feedback in changelogs or cards | Not yet |
| Compensation | Public records and self-report: grant, contract, sponsorship, or paid time | Not yet |
| Reciprocal contribution | Track provider contributions back to the project (code, fixes, infrastructure, roadmap seat) | Not yet |

Existing CHAOSS metrics to draw on: [Change Request Acceptance Ratio](https://www.chaoss.community/kb/metric-change-request-acceptance-ratio/), [Change Requests Accepted](https://www.chaoss.community/kb/metric-change-requests-accepted/), [Time to Close](https://www.chaoss.community/kb/metric-time-to-close/), [Change Requests Duration](https://www.chaoss.community/kb/metric-change-requests-duration/) and [Review Cycle Duration within a Change Request](https://www.chaoss.community/kb/metric-review-cycle-duration-within-a-change-request/), [Change Request Closure Ratio](https://www.chaoss.community/kb/metric-change-request-closure-ratio/)

## Want to Know More?

### Data Collection Strategies

Known methods (as of this writing) for collecting data related to this metric.

| Attribute | How we'd collect it | Detectable today? |
| --- | --- | --- |
| Model behavior changed | Re-test against the model; read changelogs, model & system cards | Partial. Visible in changelogs and testing; unknown under silent retraining |
| Policy changed | Review provider policy pages, contribution rules, model-card updates | Detectable when public |
| Community governance changed | Track the community's own policy, bounty, or moderation changes | Detectable; it's the community's own record |
| Attribution given | Look for change credited to community feedback in changelogs / cards | Unknown. Providers rarely attribute |
| Compensation | Public records and self-report: grant, contract, sponsorship, paid time | Partial. Public funding detectable; private needs self-report |
| Reciprocal contribution | Track provider contributions back to the project (code, fixes, infra) | Partial. Public detectable; informal unknown |
| Change persisted | Re-test across later releases to confirm no silent revert | Partial. Needs ongoing testing and version disclosure |

### Filters

- **Feedback type:** ◆ quality of contribution, ◆ accuracy / factuality, safety, bias / discriminatory, privacy, ◆ tooling / agent behavior, environmental impact, accessibility, attribution / provenance, licensing / compliance, financial cost
- **Verifiable, re-testable subset (◆):** quality of contribution, accuracy / factuality, tooling / agent behavior
- **Lean:** both care, leans community
- **Tier:** detectable-today core, standards-we're-asking-for
- **Measurable now:** yes, not yet

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
