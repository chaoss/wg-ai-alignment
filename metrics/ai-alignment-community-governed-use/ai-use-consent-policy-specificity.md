# Consent Policy Specificity

**Question:** To be added.

## Overview

This metric is part of the [AI Alignment - Community Governed AI Use](metric-model-ai-alignment-community-governed-use.md) metrics model, which measures how clear and compliant a project's governance around AI use is.

How specifically a community's AI policy addresses each domain where AI shows up, rather than one blanket statement covering all use.

For each domain, determine whether the policy specifies a supervision level, a scope limit, an accountability holder, and, where relevant, a proportionality threshold, or is silent. A project can be highly specific about code contributions and not mention notetaker bots; that gap is what this metric surfaces. A summary roll-up (overall AI use posture, across all domains) may sit alongside the per-domain breakdown.

### Taxonomy of domains

What we look for the policy to address, specifically.

| Domain | Implementation | Measurable now? |
| --- | --- | --- |
| Code contributions | Check whether policy addresses PRs, issues, and comments | Yes |
| Notetaker / meeting bots | Check whether policy addresses recorded discussion, closed or small-group content | Yes |
| Content | Check whether policy addresses documentation, blogs, design assets | Yes |
| Moderation actions | Check whether policy addresses AI use in moderation | Yes |
| Review | Check whether policy states who or what may review using AI | Yes |
| Autonomous / agentic use | Check whether policy addresses agentic use distinctly from assisted use | Yes |
| Environmental impact | Check whether policy addresses energy use, water use, hardware / carbon footprint | Partly |
| Infrastructure strain | Check whether policy addresses server load, hardware cost / financing | Partly |
| Data use for training | Check whether policy addresses platform user data used for training | Partly |

### Consent-type attributes

Within each domain, specificity is scored against attributes that sit across domains rather than being domains themselves.

| Attribute | Implementation | Measurable now? |
| --- | --- | --- |
| Supervision level | Classify as banned, human-in-the-loop / accountable, disclosure required, limited unsupervised, or fully unsupervised | Yes |
| Scope or volume limits | Look for stated limits on length or quantity of AI-assisted contribution | Yes |
| Who holds accountability | Look for a named accountability holder for AI-assisted contribution in that domain | Yes |
| Proportionality | Look for a stated resource-use threshold relative to contributor count or community size | Partly |

## Want to Know More?

### Data Collection Strategies

Known methods (as of this writing) for collecting data related to this metric.

| Attribute | How we'd collect it | Detectable today? |
| --- | --- | --- |
| Policy text per domain | Manual audit of CONTRIBUTING files, governance repos, code of conduct, foundation policy pages | Yes |
| Supervision level, scope, accountability holder | Text analysis of policy documents against the taxonomy above | Yes |
| Proportionality threshold | Manual review of policy text for stated resource-to-community-size limits | Partial. Only where explicitly stated |

### Filters

- **Domain:** code contributions, notetaker / meeting bots, content, moderation actions, review, autonomous / agentic use, environmental impact, infrastructure strain, data use for training
- **Supervision level:** banned, human-in-the-loop / accountable, disclosure required, limited unsupervised, fully unsupervised
- **Project size:** number of active contributors
- **Project age**
- **Technology ecosystem:** Python, Rust, etc.
- **Governance accountable:** single maintainer, foundation, company
- **Funding status**
- **Measurable now:** yes, partly

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
