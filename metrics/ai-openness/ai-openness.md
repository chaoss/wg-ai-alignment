# AI Openness

**Question:** To what extent is an AI system open, and at which layers of its development and deployment?

## Overview

This metric measures the degree of openness of an AI system across its key components — model weights, training data, source code, evaluation methodology, and governance — allowing communities to assess, compare, and advocate for more transparent and accessible AI systems.

"Open Source AI" is not a single binary property. Like open source software before it, openness in AI exists on a spectrum and across multiple independent dimensions. A model can have open weights but closed training data; open code but proprietary evaluation; or open governance but no access to the training pipeline. Without a structured way to measure these distinctions, communities lack the vocabulary to hold AI builders accountable or make informed decisions about which AI systems to adopt and support.

This metric draws on established frameworks such as the [OSI Open Source AI Definition](https://opensource.org/ai/open-source-ai-definition) and the [Model Openness Framework (MOF)](https://arxiv.org/abs/2403.13784) to define measurable levels of openness communities can apply.

| Indicator | Implementation | Measurable now? |
| --- | --- | --- |
| Model weights available | Check whether weights are publicly downloadable without login or license restriction | Yes |
| Training data disclosed | Check whether training data sources are documented (full dataset, data card, or provenance report) | Partly |
| Source code open | Check whether training and inference code is public under an OSI-approved license | Yes |
| Evaluation methodology published | Check whether benchmarks, datasets, and scoring criteria are publicly documented | Partly |
| License permits reuse and modification | Check whether the license allows use, modification, and redistribution | Yes |
| Governance process documented | Check whether development and update decisions follow a documented, accessible process | Partly |
| Safety and alignment documentation published | Check whether red-teaming results or alignment reports are publicly available | Partly |
| Community contribution pathway exists | Check whether external contributors can submit data, feedback, or improvements | Not yet |

## Want to Know More?

### Data Collection Strategies

Known methods (as of this writing) for collecting data related to this metric.

| Attribute | How we'd collect it | Detectable today? |
| --- | --- | --- |
| Weights availability | Check HuggingFace, GitHub, or project sites for public download links | Yes |
| Training data disclosure | Read model cards, data cards, or technical reports published alongside the model | Partly |
| Source code availability | Search for a linked code repo; check for an OSI-approved license file | Yes |
| Evaluation methodology | Read published papers, model cards, or leaderboard entries | Partly |
| License reuse rights | Parse license text against OSI Open Source AI Definition criteria | Yes |
| Governance documentation | Check for GOVERNANCE.md, decision logs, or public meeting notes | Partly |
| Safety documentation | Search for red-team reports, system cards, or alignment evaluations | Partly |
| Contribution pathway | Look for CONTRIBUTING.md, feedback forms, or data contribution guides | Yes |

### Filters

- **Openness layer:** weights, training data, source code, evaluation, license, governance, safety documentation, contribution pathway
- **License type:** OSI-approved open source, open but restricted (e.g. community license), proprietary
- **Disclosure level:** fully disclosed, partially disclosed (data card / model card only), not disclosed
- **Measurable now:** yes, partly, not yet
- **Lean:** both care, leans community, leans provider

### Visualizations

*(model-level visualizations are listed in the metrics model)*

## References

- [OSI Open Source AI Definition](https://opensource.org/ai/open-source-ai-definition)
- [Model Openness Framework (MOF)](https://arxiv.org/abs/2403.13784)
- [Hugging Face Model Cards](https://huggingface.co/docs/hub/model-cards)
- [Data Cards Playbook (Google)](https://sites.research.google/datacardsplaybook/)

## Contributors

- Shiva Sharma

Add your name if you contributed

## Additional Information

To edit this metric please submit a Change Request here: (replace with correct link once metric is added to a focus area repo)

To reference this metric in software or publications please use this stable URL: (replace with permalink once published)
