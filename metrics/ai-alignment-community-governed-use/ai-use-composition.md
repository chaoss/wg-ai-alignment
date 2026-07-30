# Use Composition

**Question:** To be added.

## Overview

This metric is part of the [AI Alignment - Community Governed AI Use](metric-model-ai-alignment-community-governed-use.md) metrics model, which measures how clear and compliant a project's governance around AI use is.

What AI tools, models, and ownership structures are in use across a community's spaces.

Establish what is present in a community's spaces: the categories of tool operating, the named products, the underlying models and their openness, and who controls the tool and its data.

| Indicator | Implementation | Measurable now? |
| --- | --- | --- |
| Tool types in use | Identify at category level: assistant, notetaker, autonomous agent, moderation bot, etc. | Yes |
| Specific tools in use | Identify named products: Copilot, ChatGPT, Claude, etc. | Partly |
| Model type | Identify the underlying model or family and its openness | Partly |
| AI tool owner | Identify who controls the tool and its data | Partly |
| Bot / agent identity in workflows | Account identity, signed commits, workflow YAML, integration manifests | Yes |
| Environmental footprint | Read model / system cards and provider ESG reports for disclosed energy, water, and carbon figures | Partly |
| Resource use relative to community size | Compare CI/CD and storage volume against contributor count | Not yet |

## Want to Know More?

### Data Collection Strategies

Known methods (as of this writing) for collecting data related to this metric.

| Attribute | How we'd collect it | Detectable today? |
| --- | --- | --- |
| Bot / agent identity in workflows | Account identity, signed commits, workflow YAML, integration manifests | Yes |
| Tool / model identification | Self-report, known signatures | Partial. Known signatures only |
| Environmental footprint disclosure | Model / system cards, provider ESG reports | Partial. Only where publicly disclosed |
| Ownership | Provider terms of service, public corporate records, self-report | Partial |
| Resource use relative to community size | CI/CD and storage volume compared to contributor count | Partial. Requires platform-level usage data |

Tooling and signals that may help: [Ecosyste.ms](https://ecosyste.ms/), GraphQL (comment metadata like hidden comments), [agents-to-block](https://github.com/adrinjalali/agents-to-block), [unveil-project/identity](https://github.com/unveil-project/identity) (AgentScan), CHAOSS Disclosure, Airflow Energy Metrics Provider. See the metrics model for the full list.

### Filters

- **Tool type:** assistant, notetaker, autonomous agent, moderation bot
- **Model openness:** open weight, open source, closed
- **Owner:** company, foundation, individual, unknown
- **Usage surface:** pull requests, git commits, issues, content, moderation
- **Project size:** number of active contributors
- **Community size**
- **Technology ecosystem:** Python, Rust, etc.
- **Carbon energy footprint**
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
