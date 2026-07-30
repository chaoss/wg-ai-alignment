# Misuse

**Question:** To be added.

## Overview

This metric is part of the [AI Alignment - Community Governed AI Use](metric-model-ai-alignment-community-governed-use.md) metrics model, which measures how clear and compliant a project's governance around AI use is.

The presence and rate of AI use that causes harm or violates community norms, independent of whether a formal policy exists yet to violate.

Capture harm and disruption that predates or falls outside written policy, so that communities without an AI policy, or with use that violates the Code of Conduct, can still measure it. This is deliberately separate from [Use Compliance](ai-use-compliance.md): compliance measures use against policy, while misuse measures harm whether or not policy names it.

| Indicator | Implementation | Measurable now? |
| --- | --- | --- |
| Code of Conduct violations involving AI | Code of conduct records where AI use is a factor in the reported harm | Partly |
| Low-quality AI-driven contribution load | Maintainer report and triage records for contributions rejected as AI-generated noise | Partly |
| Social engineering and toxic behavior facilitated by AI | Moderation records (flagging, tagging, hiding, deleting) where AI use is a factor | Partly |
| License laundering | AI regenerating code from training data in a way that strips out copyleft reciprocity requirements. Maintainer or legal self-report | Not yet |
| Wrongful accusation | Contributors who did not use AI being wrongly accused of undisclosed use, including harm produced by retaliation and other motivations. Maintainer self-report, code of conduct records | Not yet |
| Attribution stripped from lifted work | Cases where AI output reproduced another author's code or prose without headers or attribution | Not yet |

**Note on licensing:** license laundering is legally unsettled rather than established fact. Framing it as unresolved lets member projects evaluate the risk without overstating a position courts have not yet decided.

## Want to Know More?

### Data Collection Strategies

Known methods (as of this writing) for collecting data related to this metric.

| Attribute | How we'd collect it | Detectable today? |
| --- | --- | --- |
| Self-disclosed AI use by human contributors | Depends on policy and culture; no technical enforcement | Partial |
| Whether a contribution came from any LLM at all (no disclosure) | No reliable method; text-based AI detectors are unreliable (see MIT Sloan EdTech reference) | Unknown |
| Which specific model produced an undisclosed contribution | No reliable signal currently exists | Unknown |
| Whether an approved model was used vs. an unapproved one in undisclosed contributions | Depends on the above | Unknown |
| License 'laundering' incidents | Maintainer or legal self-report; no reliable automated signal currently exists | Unknown |
| Wrongful accusation incidents | Maintainer self-report, code of conduct records; no reliable automated signal currently exists | Unknown |

**Note**: The "unknown" entries are where CHAOSS and adjacent projects can build, through tooling, partnerships, or formally surfacing the gap as unsolved.

Examples of the failure modes this metric is meant to capture are listed in the [Appendix of the metrics model](metric-model-ai-alignment-community-governed-use.md#failure-modes-examples-of-ai-being-used-in-ways-that-motivate-detection).

### Filters

- **Harm type:** license laundering, wrongful accusation, attribution stripping, low-quality contribution load, social engineering, toxic behavior
- **Policy status:** community has an AI policy, community has no AI policy yet
- **Source of record:** code of conduct records, moderation records, maintainer self-report, legal self-report
- **Usage surface:** pull requests, git commits, issues, content, moderation
- **Project size:** number of active contributors
- **Governance accountable:** single maintainer, foundation, company
- **Measurable now:** partly, not yet

### Visualizations

*(model-level visualizations are listed in the metrics model)*

## References

*(see the References section of the metrics model)*

## Contributors

- Emma Irwin
- Adrian Edwards
- Justin Wheeler
- Coraline Ada Ehmke
- Omkar Petkar
- Andrew Nesbitt

Add your name if you contributed

## Additional Information

To edit this metric please submit a Change Request here: (replace with correct link once metric is added to a focus area repo)

To reference this metric in software or publications please use this stable URL: (replace with permalink once published)
