# Consent Policy Specificity

**Question:** How specifically, does a community's AI policy addresses each domain where AI shows up, rather than one blanket statement covering all use.

This metric is part of the [AI Alignment - Community Governed Use](../ai-alignment-community-governed-use/metric-model-ai-alignment-community-governed-use.md) metrics mode.

## Overview

For each domain, determine whether the policy specifies a supervision level, a scope limit, an accountability holder, and, where relevant, a proportionality threshold, or is silent. A project can be highly specific about code contributions and not mention notetaker bots; that gap is what this metric surfaces.

A summary roll-up (overall AI use posture, across all domains) may sit alongside the per-domain breakdown.

### Taxonomy of domains

What we look for the policy to address, specifically:

- Code contributions (PRs, issues, comments)
- Notetaker / meeting bots (recorded discussion, closed or small-group content)
- Content (documentation, blogs, design assets)
- Moderation actions
- Review (who or what may review using AI)
- Autonomous / agentic use
- Environmental Impact (energy use, water use, hardware/carbon footprint)
- Infrastructure strain (server load, hardware cost/financing)
- Data use for training (platform user data)

### Consent-type attributes

Within each domain, specificity is scored against attributes that sit across domains rather than being domains themselves:

- Supervision level (banned, human-in-the-loop / accountable, disclosure required, limited unsupervised, fully unsupervised)
- Scope or volume limits
- Who holds accountability
- Proportionality (resource use relative to contributor count or community size)

## Want to Know More?

### Data Collection Strategies

- Policy text per domain: manual audit of CONTRIBUTING files, governance repos, code of conduct, foundation policy pages
- Supervision level, scope, accountability holder: text analysis of policy documents against the taxonomy above
- Proportionality threshold: manual review of policy text for stated resource-to-community-size limits. Detectable today: partial, only where explicitly stated.

### Filters

To be added.

### Visualizations

- A policy coverage matrix that shows which areas are clear, partial, or missing.

## References

To be added.

## Contributors

- Emma Irwin
- Adrian Edwards
- Justin Wheeler
- Coraline Ada Ehmke
- Omkar Petkar
- Andrew Nesbitt

Add your name if you have contributed

## Additional Information

To edit this metric please submit a Change Request here: (replace with correct link)

To reference this metric in software or publications please use this stable URL: (replace with permalink)
