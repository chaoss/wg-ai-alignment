# Metrics Model: AI Alignment - Community Governed AI Use

**Question:** How clear and compliant is a project/community's governance around AI use?

👉See [detection limits and platform-default constraints](#detection-limits-and-platform-default-constraints) in the Appendix for what cannot be measured today.

👉You may also be interested in [failure modes](#failure-modes-examples-of-ai-being-used-in-ways-that-motivate-detection) that motivate detection.

## Framing and terminology

This work sits under the AI Alignment for Open Source Communities working group in CHAOSS. We build metrics that let our projects and communities measure how well-aligned the AI in our spaces (through use, or otherwise) is with the intentions and goals of those communities. This metrics model is one such instrument: it measures governed use, whether a community has decided what AI use it consents to, and whether actual use matches that decision.

## Why It Matters

AI is changing how we build software and how we collaborate, and it comes with as-yet-unknown impacts on communities where AI is being used to communicate and build. Using AI tools in ways that obscure their presence, misrepresent authorship, or process others' contributions without transparency undermines the trust and authenticity our communities depend on.

Governance is only part of the picture. Communities are actively writing and rewriting their own rules for AI use, often ahead of any formal standard, and those rules keep changing as new failure modes surface. This metrics model gives communities a way to see their own policy as it evolves, to check whether use matches that policy, and to track misuse even in communities that have no formal policy yet.

**NOTE**: These metrics represent a synthesis of existing policies and the tensions surrounding them, as well as an ambition to reach a level of collaborative success in the open that goes beyond what we've previously known to be possible. Some metrics may be challenging to measure with current methods. We state the measurement goal regardless, in the belief that naming what we want to know is itself what drives the research and tooling innovation needed to measure it.

## User Stories

**Project and team leaders**

- As a project leader, I want to measure the existing use of AI in my community so that I can determine future project policy on the use of AI in the project.
- As a team leader, I want to be aware of tools and workflows that people use to participate in my project.
- As a project leader considering a disclosure-and-ban policy, I want to see how similar projects have fared so I can judge the tradeoffs before adopting it.
- As a project leader considering a conditional, human-in-the-loop policy, I want a way to express task-specific rules rather than a blanket yes or no.
- As a project leader who has decided not to restrict AI use, I want to state that clearly so contributors who disagree can choose to fork or leave rather than block others.
- As a project leader considering an outright ban, I want to see how that reasoning was received elsewhere before deciding whether it holds for my project.
- As a project leader who adopted a conditional policy, I want to check whether disclosed AI-assisted contributions meet its requirements, so I can tell whether the policy is working or just written down.

**Maintainers**

- As a project maintainer, I want to verify or be aware of the ways that my community members and contributors are (or aren't) abiding by the policies the community has consented to, so it can inform my response and maintenance of a healthy community.
- As a maintainer, I want to see an overview of the specific AI tools and models being used in my (or other) communities, so I can compare tool quality and learn about new frontier models as contributors adopt them.
- As a maintainer, I want to distinguish AI-assisted human contribution from autonomous agent activity in my workflows, so I know which policy provisions apply to a given contribution.
- As a maintainer, I want a way to signal that my project has an active human community and pre-LLM history, so a platform's graduated policy places my project correctly rather than flagging it on resource use alone.
- As a maintainer with a zero-tolerance policy, I want guidance on responding warmly to AI-assisted submissions I still plan to reject, so the contributor leaves treated like any other well-meaning first-time submitter, not shamed.

**Community members**

- As a community member, I want to know who controls the data behind the AI tools I interact with in a community, so I know where my data is and how I can assert my rights (e.g. GDPR).
- As a community member, I want to know what category of tool is being used in a space I'm participating in (assistant, notetaker, autonomous agent), so I can judge what kind of consent applies before I speak or contribute.
- As a meeting participant, I want to know whether a notetaker bot is a passive transcription tool or one that shares content onward (e.g. training, third-party analysis), so I can judge whether my consent to be recorded covers what happens to that recording.

**Moderators and community managers**

- As a content moderator, I want to mitigate against new forms of social engineering attacks and toxic behavior facilitated by AI usage so that I can better protect the psychological safety of my community.
- As a community manager, I want to understand how AI usage might impact code of conduct enforcement.
- As a community manager, I want to see which policy provisions actually reduce low-quality AI-driven contribution load, so I can decide what to adopt before we hit the same problem.

**Contributors**

- As a potential contributor, I want to know if my preferences for AI use match community policies.
- As a contributor who wants to use AI extensively, I want to know where a project sits on the ban-to-permissive spectrum so I don't invest effort building a contribution the project won't accept.
- As a contributor who codes without AI assistance, I want to be trusted at face value rather than accused of undisclosed LLM use, so suspicion doesn't fall on people doing their own work just because AI use has become harder to rule out.
- As a contributor, I want to understand the rationale behind AI policies to limit use (not just that they do).
- As a contributor whose employer requires AI tool use as a condition of employment, I want a way to disclose (attribute) that my use was mandated rather than chosen.

**Foundations and maintainer collectives**

- As a foundation representative, I want to compare how member projects' AI policies have shifted over time so that I can identify where a shared foundation-level position would help.
- As a foundation representative, I want the stated rationale behind a policy change broken out as separate, checkable claims, so member projects can evaluate the reasoning on its merits rather than treating the outcome as self-justifying.
- As a foundation representative, I want licensing-related misuse claims (e.g. license laundering) framed as legally unsettled rather than established fact, so member projects don't overstate a position courts haven't yet resolved.

**Model builders**

- As a model builder, I want to perform broad analysis across all of GitHub to see how many open source projects are adopting AI, and for what purposes, so I can choose what tools to build to serve the most common needs.
- As a model builder, I want to see how often disclosure-labeling provisions recur across projects, so I can design tooling that makes disclosure easy rather than an afterthought.

## Related Metrics Models

- [AI Alignment - Community Aligned Training (Feedback)](../ai-alignment-community-feedback/metrics-model-ai-alignment-community-aligned-training-feedback.md) — measures whether a community can give feedback to a model builder and see its impact, as the means by which alignment with that community increases. Where this model measures use a community consents to, that model measures the loop back to the builder.

## Metrics in the Metrics Model

This model contains five metrics. Together they cover what a community has decided (Consent Policy Specificity), how that decision moves (Policy Change), what is actually in use (Use Composition), whether the two match (Use Compliance), and the harm that occurs whether or not a policy exists to name it (Misuse).

### [Consent Policy Specificity](ai-use-consent-policy-specificity.md)

- **Description.** How specifically a community's AI policy addresses each domain where AI shows up, rather than one blanket statement covering all use.
- **Objectives.** For each domain, determine whether the policy specifies a supervision level, a scope limit, an accountability holder, and, where relevant, a proportionality threshold, or is silent. A project can be highly specific about code contributions and not mention notetaker bots; that gap is what this metric surfaces. A summary roll-up (overall AI use posture, across all domains) may sit alongside the per-domain breakdown.
- **Implementation.** See data collection strategies section.

### [Policy Change](ai-use-policy-change.md)

- **Description.** How a community's AI policy changes over time, and how that compares to shifts happening across other projects.
- **Objectives.** Track tightening, loosening, and newly added provisions per domain (see Consent Policy Specificity), so a community can see its own trajectory and where it sits relative to the wider ecosystem. Also capture the enforcement mechanism (whether a change is enforced automatically, case-by-case, or not yet applied) and, where a change is decided by vote, the participation rate and result.
- **Implementation.** See data collection strategies section.

### [Use Composition](ai-use-composition.md)

- **Description.** What AI tools, models, and ownership structures are in use across a community's spaces.
- **Objectives.** Establish what is actually present: tool types in use at category level (assistant, notetaker, autonomous agent, moderation bot), specific named tools (Copilot, ChatGPT, Claude), the underlying model or family and its openness, and who controls the tool and its data.
- **Implementation.** See data collection strategies section.

### [Use Compliance](ai-use-compliance.md)

- **Description.** Whether actual or disclosed AI use matches what current policy permits.
- **Objectives.** Check disclosed or detected use (per Use Composition) against the specificity and supervision level set for that domain (per Consent Policy Specificity).
- **Implementation.** See data collection strategies section.

### [Misuse](ai-use-misuse.md)

- **Description.** AI use that causes harm or violates community norms and expectations.
- **Objectives.** Capture harm and disruption that predates or falls outside written policy, so that communities without an AI policy, or with use that violates the Code of Conduct, can still measure it. Other potentials:
  - **License laundering** — AI regenerating code from training data in a way that strips out copyleft reciprocity requirements.
  - **Wrongful accusation** — contributors who did not use AI being wrongly accused of undisclosed use; harm produced by retaliation and other motivations.
- **Implementation.** See data collection strategies section.

## Data collection strategies

What we would look for to create baselines and track progress.

**Covers usage (cross-cutting, applies across metrics)**

- Pull Requests (code, documentation, for issue-type: security, bug, etc.)
- Git commits (commit message, trailers, etc. from a specified branch)
- Issues (opening, commenting, closing)
- Content (documentation, blogs, social media, printed assets, design contributions, etc.)
- Moderation (flagging, tagging, hiding, deleting)

### Consent Policy Specificity

| Attribute | How we'd collect it | Detectable today? |
| --- | --- | --- |
| Policy text per domain | Manual audit of CONTRIBUTING files, governance repos, code of conduct, foundation policy pages | Yes |
| Supervision level, scope, accountability holder | Text analysis of policy documents against the taxonomy | Yes |
| Proportionality threshold | Manual review of policy text for stated resource-to-community-size limits | Partial. Only where explicitly stated |

### Policy Change

| Attribute | How we'd collect it | Detectable today? |
| --- | --- | --- |
| Policy version history | Git / version history of policy documents | Yes |
| Direction of change | Classify each revision as tightening, loosening, or adding a new provision, per domain | Yes |

### Use Composition

| Attribute | How we'd collect it | Detectable today? |
| --- | --- | --- |
| Bot / agent identity in workflows | Account identity, signed commits, workflow YAML, integration manifests | Yes |
| Tool / model identification | Self-report, known signatures | Partial. Known signatures only |
| Environmental footprint disclosure | Model / system cards, provider ESG reports | Partial. Only where publicly disclosed |
| Ownership | Provider terms of service, public corporate records, self-report | Partial |
| Resource use relative to community size | CI/CD and storage volume compared to contributor count | Partial. Requires platform-level usage data |

### Misuse

| Attribute | How we'd collect it | Detectable today? |
| --- | --- | --- |
| Self-disclosed AI use by human contributors | Depends on policy and culture; no technical enforcement | Partial |
| Whether a contribution came from any LLM at all (no disclosure) | No reliable method; text-based AI detectors are unreliable | Unknown |
| Which specific model produced an undisclosed contribution | No reliable signal currently exists | Unknown |
| Whether an approved model was used vs. an unapproved one in undisclosed contributions | Depends on the above | Unknown |
| License 'laundering' incidents | Maintainer or legal self-report; no reliable automated signal currently exists | Unknown |
| Wrongful accusation incidents | Maintainer self-report, code of conduct records; no reliable automated signal currently exists | Unknown |

**Note**: The "unknown" entries are where CHAOSS and adjacent projects can build, through tooling, partnerships, or formally surfacing the gap as unsolved.

### Detection capability map (what we can and can't detect today)

| Question | Signal | Detectable today? |
| --- | --- | --- |
| Bot / agent identity in workflows | Account identity, signed commits, workflow YAML, integration manifest | Detectable |
| Self-disclosed AI use by human contributors | Depends on policy and culture; no technical enforcement | Partial |
| Whether a contribution came from any LLM at all (no disclosure) | Text-based AI detectors are unreliable (see MIT Sloan EdTech reference) | Unknown |
| Which specific model produced an undisclosed contribution | No reliable signal currently exists | Unknown |
| Whether an approved model was used vs. an unapproved one in undisclosed contributions | Depends on the above | Unknown |
| Whether a contribution disclosed every model use or some were missed (e.g. models A & B used but only B disclosed) | No reliable signal currently exists | Unknown |

Marking these gaps is part of the work. The "unknown" entries are where the WG and adjacent projects can build, through tooling, partnerships, or formally surfacing the gap as unsolved.

## Filters

- Project size (number of active contributors)
- Project age
- Technology ecosystem (Python, Rust, etc.)
- Usage
- Community size
- Governance accountable (single maintainer, foundation, company, etc.)
- Funding status
- Carbon energy footprint

## Tooling & Resources

Available tools / signals:

- [Ecosyste.ms](https://ecosyste.ms/) (usage, ecosystem, solo maintainer)
- GraphQL (comment metadata like hidden comments)
- Coraline's tool (Repository Invitations) — see her [2017 blog post](https://where.coraline.codes/blog/) (section *Collaboration* particularly)
- [agents-to-block](https://github.com/adrinjalali/agents-to-block) (community-maintained list of AI agents)
- Account identity, signed commits, workflow YAML, integration manifests (for bot / agent identification)
- [unveil-project/identity](https://github.com/unveil-project/identity) — AgentScan, GitHub AI Agent Detector. An open experiment in detecting automation patterns on GitHub
- CHAOSS Disclosure — detects AI disclosures in git commits and pull requests
- Airflow Energy Metrics Provider (measuring energy consumption and carbon footprint in Airflow DAGs)

## Visualizations

- Timeline of detected AI use events
- Funnel from detected potential AI use → reviewed → action taken
- Stacked bar showing the gap between policy scope and platform-default scope
- Pie chart showing contributions with AI use accepted and rejected

*(Cite tool/website and date created/retrieved. Citation should be below the image as Figure X: Title (Source, Year).)*

## Appendix

### Related efforts in adjacent spaces (mapped in WG Issue #61)

**On whether AI is used at all (Use)**

- Mozilla Foundation — evaluation named as a 2025 priority, with fellows working on community-driven approaches to AI use. [https://www.mozillafoundation.org/en/what-we-fund/programs/bringing-ai-down-to-earth-evaluation-as-a-main-ai-theme-in-2025/](https://www.mozillafoundation.org/en/what-we-fund/programs/bringing-ai-down-to-earth-evaluation-as-a-main-ai-theme-in-2025/)
- LCFI participatory analysis (Arnstein's ladder applied to AI governance) — frames whether communities have real participation in AI governance, including the choice not to use AI. [https://www.lcfi.ac.uk/news-events/blog/post/will-participatory-approaches-in-ai-governance-help](https://www.lcfi.ac.uk/news-events/blog/post/will-participatory-approaches-in-ai-governance-help)

**Cross-cutting (touches Use, Approval, Actions, and Improvements)**

- Metagov's Collective Governance for AI — framework mapping where community governance could sit across the AI stack. [https://metagov.org/cg-ai/](https://metagov.org/cg-ai/)

### Failure modes (examples of AI being used in ways that motivate detection)

- **OCaml PR #14369** — AI tools used with a niche language nearly directly lifted another author's code, including headers and attribution. [https://github.com/ocaml/ocaml/pull/14369](https://github.com/ocaml/ocaml/pull/14369)
- **Castle Game Engine forum** — AI produced code referencing obsolete or non-existent engine APIs and going against project portability practices. [https://forum.castle-engine.io/t/for-you-with-ia/2048/4](https://forum.castle-engine.io/t/for-you-with-ia/2048/4)
- **Modern Pascal book submission** — AI-written prose that "looks professional but is just factually wrong in many points." [https://github.com/modern-pascal/modern-pascal-introduction/issues/28](https://github.com/modern-pascal/modern-pascal-introduction/issues/28)

### Detection limits and platform-default constraints

- MIT Sloan EdTech: AI Detectors Don't Work (limits of detection-based enforcement). [https://mitsloanedtech.mit.edu/ai/teach/ai-detectors-dont-work/](https://mitsloanedtech.mit.edu/ai/teach/ai-detectors-dont-work/)
- agents-to-block (community-maintained list of AI agents to block). [https://github.com/adrinjalali/agents-to-block](https://github.com/adrinjalali/agents-to-block)
- GitHub maintainer discussions on AI features and platform defaults the community cannot fully override:
  - [https://github.com/community/maintainers/discussions/470](https://github.com/community/maintainers/discussions/470)
  - [https://github.com/community/maintainers/discussions/442](https://github.com/community/maintainers/discussions/442)
  - [https://github.com/community/maintainers/discussions/646](https://github.com/community/maintainers/discussions/646)

## Metrics Model Validated By

*(to be added)*

## References

**Framing**

- Irwin, E. (2026). After the Pull Request: Four Proposed Areas of Work for Open Community Representation. [https://sunnydeveloper.com/](https://sunnydeveloper.com/)
- Irwin, E. AI Consent for Open Communities. [https://sunnydeveloper.com/ai-consent-for-open-communities/](https://sunnydeveloper.com/ai-consent-for-open-communities/)
- CHAOSS AI Alignment Working Group, Issue #61. [https://github.com/chaoss/wg-ai-alignment/issues/61](https://github.com/chaoss/wg-ai-alignment/issues/61)

**Policies consulted**

- Ongoing list: [https://github.com/chaoss/wg-ai-alignment/blob/main/moderation/README.md](https://github.com/chaoss/wg-ai-alignment/blob/main/moderation/README.md)
- Recommendations when using LLM-gen-AI — Software Freedom Conservancy. [https://sfconservancy.org/](https://sfconservancy.org/)

## Contributors

- Emma Irwin
- Adrian Edwards
- Justin Wheeler
- Coraline Ada Ehmke
- Omkar Petkar
- Andrew Nesbitt

Add your name if you contributed

## Additional Information

To edit this metrics model please submit a Change Request here: (replace with correct link once the model is added to a focus area repo)

To reference this metrics model in software or publications please use this stable URL: (replace with permalink once published)
