# Feedback Channel Quality

**Question:** To be added.

## Overview

This metric is part of the [AI Alignment - Community Aligned Training (Feedback)](metrics-model-ai-alignment-community-aligned-training-feedback.md) metrics model, which measures whether a community can give feedback to a model builder and see its impact, as the means by which alignment with that community increases.

Determine the quality of a channel in providing a feedback loop between open source communities and model builders.

Discover whether a usable feedback channel exists at all, its accessibility for community and model builders, categories of feedback accepted (as per the value exchange table in the metrics model) and other SLA details.

| Indicator | Implementation | Measurable now? |
| --- | --- | --- |
| Channel exists | Audit provider sites, repos, docs, and foundation channels (provider intake, community channel, foundation liaison, or none documented) | Yes |
| Reachable | Check it isn't blocked by language, identity disclosure, or account barriers; gather community self-report on real usability | Yes |
| Channel is governed | Check whether the project has a defined process governing the channel: what it is, who may use it, what counts as valid feedback, and how decisions are made | Partly |
| Confidential intake exists | Check for a path for harm reports without public disclosure or consensus, with quality conferred by downstream triage | Partly |
| CoC covers AI harms (proxy) | Check whether the project's Code-of-Conduct scope covers AI-related harm, with a route to the provider | Partly |
| Documented intake commitment | Look for a published SLA, scope, who reviews, and an escalation path | Not yet |

Existing CHAOSS metrics to draw on: [Chat Platform Inclusivity](https://www.chaoss.community/kb/metric-chat-platform-inclusivity/), [Psychological Safety](https://www.chaoss.community/kb/metric-psychological-safety/), [Code of Conduct for a Project](https://www.chaoss.community/kb/metric-code-of-conduct-for-a-project/), [Documentation Discoverability](https://www.chaoss.community/kb/metric-documentation-discoverability/)

## Want to Know More?

### Data Collection Strategies

Known methods (as of this writing) for collecting data related to this metric.

| Attribute | How we'd collect it | Detectable today? |
| --- | --- | --- |
| Channel exists | Manual audit of provider sites, repos, docs, foundation channels | Partial. Public channels found by audit; private arrangements unknown |
| Reachable | Read stated requirements; community self-report on real usability | Partial. Requirements visible; usability needs community reporting |
| Governance behind signal | Read project decision process / consensus records where published | Partial. Visible where projects document governance |

### Filters

- **Channel type:** provider intake, community channel, foundation liaison, none documented
- **Feedback type:** ◆ quality of contribution, ◆ accuracy / factuality, safety, bias / discriminatory, privacy, ◆ tooling / agent behavior, environmental impact, accessibility, attribution / provenance, licensing / compliance, financial cost
- **Lean:** both care, leans community
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
