# Use Compliance

**Question:** To be added.

## Overview

This metric is part of the [AI Alignment - Community Governed AI Use](metric-model-ai-alignment-community-governed-use.md) metrics model, which measures how clear and compliant a project's governance around AI use is.

Whether actual or disclosed AI use matches what current policy permits.

Check disclosed or detected use (per [Use Composition](ai-use-composition.md)) against the specificity and supervision level set for that domain (per [Consent Policy Specificity](ai-use-consent-policy-specificity.md)). Compliance can only be assessed where policy is specific enough to be checked against, so a low score here may reflect a silent policy rather than a non-compliant community.

| Indicator | Implementation | Measurable now? |
| --- | --- | --- |
| Disclosure present where required | Where policy requires disclosure, check whether contributions carry it (commit trailers, PR text, issue comments) | Yes |
| Bot / agent use within permitted domains | Match identified bots and agents (account identity, signed commits, workflow YAML, integration manifests) against the domains policy permits | Yes |
| Supervision level met | Compare the supervision level evident in the contribution against the level policy sets for that domain | Partly |
| Scope or volume limit respected | Compare contribution length or quantity against any stated limit | Partly |
| Accountability holder identified | Check whether the person accountable for the AI-assisted contribution is named where policy requires it | Partly |
| Approved model vs. unapproved model used | Compare the model in use against any policy-approved list | Not yet |
| Complete disclosure of every model used | Check whether all models used were disclosed, not just some | Not yet |
| Proportionality threshold met | Compare resource use against any stated resource-to-community-size limit | Not yet |

## Want to Know More?

### Data Collection Strategies

Known methods (as of this writing) for collecting data related to this metric.

| Attribute | How we'd collect it | Detectable today? |
| --- | --- | --- |
| Bot / agent identity in workflows | Account identity, signed commits, workflow YAML, integration manifests | Yes |
| Self-disclosed AI use by human contributors | Depends on policy and culture; no technical enforcement | Partial |
| Policy provision to check against | Manual audit of CONTRIBUTING files, governance repos, code of conduct, foundation policy pages | Yes |
| Whether a contribution came from any LLM at all (no disclosure) | No reliable method; text-based AI detectors are unreliable | Unknown |
| Which specific model produced an undisclosed contribution | No reliable signal currently exists | Unknown |
| Whether an approved model was used vs. an unapproved one in undisclosed contributions | Depends on the above | Unknown |
| Whether a contribution disclosed every model use or some were missed | No reliable signal currently exists (e.g. models A & B used but only B disclosed) | Unknown |
| Resource use relative to community size | CI/CD and storage volume compared to contributor count | Partial. Requires platform-level usage data |

**Note**: The "unknown" entries are where CHAOSS and adjacent projects can build, through tooling, partnerships, or formally surfacing the gap as unsolved.

### Filters

- **Domain:** code contributions, notetaker / meeting bots, content, moderation actions, review, autonomous / agentic use, environmental impact, infrastructure strain, data use for training
- **Supervision level:** banned, human-in-the-loop / accountable, disclosure required, limited unsupervised, fully unsupervised
- **Disclosure status:** disclosed, undisclosed, mandated by employer
- **Actor:** human contributor with AI assistance, autonomous agent
- **Usage surface:** pull requests, git commits, issues, content, moderation
- **Outcome:** accepted, rejected
- **Project size:** number of active contributors
- **Measurable now:** yes, partly, not yet

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
