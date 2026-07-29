# Metrics Model: AI Alignment - Community Aligned Training (Feedback)

👉See list of acronyms and meaning in the [Appendix](#acronyms).

👉You may also be interested in [precedents](#precedents) around such human feedback

👉You may also be interested in learning about [synthetic data](#acronyms) and related gaps.

## Framing and terminology

This work sits under the AI Alignment for Open Source Communities working group in CHAOSS. We build metrics that let our projects and communities measure how well-aligned the AI in our spaces (through use, or otherwise) is with the intentions and goals of those communities. This metric is one such instrument: it measures the feedback loop, whether a community can give effective feedback to a model builder and see its impact, as the means by which alignment with that community increases.

👉AI Alignment resides within the AI safety discipline.

## Why It Matters

AI models are built on the labor of open source communities in two distinct ways: as a dependency of the technology (the frameworks, libraries, and tooling models and their infrastructure run on) and as the content they are trained on (the code, documentation, and discussion absorbed into the models). Yet those communities have no way to feed back into the models the way paid annotators and synthetic data do. This metrics model measures that feedback loop: whether a community can give feedback to a model builder and see its impact, as the means by which alignment with that community increases.

This metric treats community feedback as a way to center the values, labour and intention of open communities AI is built on, using empirical language we hope model builders will respond to. The specific metrics described within are:

- [AI feedback governance](ai-feedback-governance.md)
- [Feedback channel quality](feedback-channel-quality.md)
- Efficiency (of the process)
- Effectiveness (measures of value to model builders and communities)

**NOTE**: While this metric model focuses on improvement to the model itselff, alternate solutions including open weight are potential solutions for alignment. Additionally, [despite outreach](https://sunnydeveloper.com/be-the-first/), we have not yet found a model builder willing to engage with, and prototype community alignment - we hope this model can be part of advocacy for encouraging such partnerships.

### What we want to measure

Structured feedback is already routine inside AI development: preference data, RLHF, evaluation suites, red-teaming, post-deployment evals, internal review. Open source communities have no equivalent loop despite the value of that opportunity for model builders and communities alike.

Public-input precedents exist (Collective Constitutional AI, the Alignment Assemblies, OpenAI's Democratic Inputs, Meta's Community Forum; see appendix), but they address what an AI's values should be, via representative public samples. This metric addresses the source communities whose content trained the model, reporting concrete behavioral defects. The precedents prove external input can reach a model; the source-community loop is the gap they leave open.

👉See example list of precedents in [Appendix](#precedents).

### Something builders and communities care about (value exchange)

*influenced Rohin Shah talk - [How to Theorize So Empiricists Will Listen](https://www.youtube.com/watch?v=BWHbxv5kxLI).

Feedback is a translation and the value must carry both ways, from community to the builder and back. The table below describes the value to each.

Note: this is not unlike the translations we already do in open source to describe 'business value' to business - like hiring pipelines, security, reduced engineering capacity etc.

◆ = verifiable, re-testable subset

| Lean | Feedback type | Why community cares | Why builders care |
| --- | --- | --- | --- |
| Both care | ◆ Quality of contribution | Low-quality, high-volume, or confusing AI output wastes maintainer time | Their tool producing low-value output on repos they depend on |
| Both care | ◆ Accuracy / factuality | Wrong info about their project | Hallucination is a tracked quality metric |
| Both care | Safety | Harm in their spaces | High priority: misuse, liability, public trust |
| Both care | Bias / discriminatory | Harm to people | Eval target, reputational, employment and legal risk |
| Both care | Privacy | Exposure of contributors' data | Legal and compliance risk |
| Both care | ◆ Tooling / agent behavior | Rate limits, spam, ignoring robots.txt or opt-outs | Their agents misbehaving in workflows they rely on |
| Both care | Environmental impact | Model meets community standards | Brand, ESG reporting, public scrutiny of AI energy use |
| Both care | Accessibility | Inclusive participation | Compliance requirements, procurement, brand reputation |
| Leans community | Attribution / provenance | Credit and agency for their work | Mostly license and legal risk |
| Leans community | Licensing / compliance | Their license terms respected | Compliance pressure, not desire |
| Leans community | Financial cost | Cost to give feedback and evaluate fixes | Not their cost, so easily ignored |

## User Stories

**Maintainers**

- As a maintainer I want to communicate governance decisions around AI to model builders.
- As a maintainer dealing with AI-generated low-quality PRs, I want to flag the contribution pattern to the provider whose tool produced it, so that I'm not bearing the full cost of triaging output I didn't ask for.
- As a maintainer, I want a documented intake SLA from each major model provider, so that I can decide whether filing feedback is worth my time before I start.

**Foundations and maintainer collectives**

- As a foundation representative, I want baseline metrics on response times, acknowledgment rates, and attribution rates across major model providers, so that I can negotiate collective intake agreements on behalf of member projects from a position of evidence.
- As a foundation, I want a standard taxonomy for AI-feedback categories (bias, attribution, safety, accessibility, agent behavior, environmental), so that reports from different projects are comparable and aggregable.

**Contributors and community members**

- As a community member I want to know what the governance is for raising issues within my community (to gain consensus to report on behalf of that project).
- As a community member who has experienced harm (misattribution, harassment via AI-generated content, privacy exposure), I want a non-public channel for reporting, so that I'm not forced to disclose identity or details to get a response.

**Model providers**

- As a model provider building feedback intake, I want to know what counts as a usable channel from the community's perspective (language, identity disclosure, account requirements, response substance), so that I don't build something that fails accessibility before it ever has a chance to fail effectiveness.
- As a model provider, I want to cite community feedback as a contributing factor in model changes (with consent and attribution), so that the ecosystem can see reciprocal benefit and our investment in feedback infrastructure is legible.

**Researchers and policy**

- As a researcher, I want a public, replicable dataset of AI-feedback events and outcomes across providers and time, so that I can study patterns, identify failure modes, and inform policy.

**Funders**

- As a funder of open source infrastructure, I want to see whether the projects I support are receiving proportional value back from the AI ecosystem, so that I can direct grants toward gaps the AI industry is failing to fill.

## Metrics in the Metrics Model

This model contains three metrics: Method of Feedback, Effectiveness of Feedback, and Efficiency of Feedback. Indicators across all three are split into two tiers: a detectable-today core that can be measured now, and a standards-we're-asking-for layer that becomes measurable only once providers adopt a short list of practices.

### [AI Feedback Governance](ai-feedback-governance.md)

- **Description.** Whether the community has policy for when and how feedback to AI builders happens: a decided, written expectation that feedback is something this project does, through which path, triggered by what, and decided by whom.
- **Objectives.** Establish that feedback is governed by policy rather than left to whoever happens to speak up. Effective feedback governance does three things: it provides a consensus path for reaching a shared community position; it provides a non-consensus path (through the Code of Conduct or another confidential route) for feedback that cannot or should not wait for consensus, such as harm or safety; and it routes through the community's own leadership first, because the issue is often how AI is being used within the project rather than the model itself. Governance decides whether a matter is resolved internally or escalated to the builder.
- **Implementation.** See data collection strategies section.

### [Feedback Channel Quality](feedback-channel-quality.md)

- **Description.** Determine the quality of a channel in providing a feedback loop between open source communities and model builders.
- **Objectives.** Discover whether a usable feedback channel exists at all, its accessibility for community and model builders, categories of feedback accepted (as per value lists above) and other SLA details.
- **Implementation.** See data collection strategies section.

### Effectiveness of Feedback

- **Description.** Determine whether or not feedback was effectively resolved to the satisfaction of governance agreement (for community and/or model builder).
- **Objectives.** Whether feedback was in scope and if so - did it produce an observable change (in model behavior, policy, attribution, compensation, reciprocal contribution, or community-facing tooling), and whether that change persists.
- **Implementation.** See data collection strategies section.

Existing CHAOSS metrics to draw on: [Change Request Acceptance Ratio](https://www.chaoss.community/kb/metric-change-request-acceptance-ratio/), [Change Requests Accepted](https://www.chaoss.community/kb/metric-change-requests-accepted/), [Time to Close](https://www.chaoss.community/kb/metric-time-to-close/), [Change Requests Duration](https://www.chaoss.community/kb/metric-change-requests-duration/) and [Review Cycle Duration within a Change Request](https://www.chaoss.community/kb/metric-review-cycle-duration-within-a-change-request/), [Change Request Closure Ratio](https://www.chaoss.community/kb/metric-change-request-closure-ratio/)

| Indicator | Implementation | Measurable now? |
| --- | --- | --- |
| Model behavior changed | Re-test the behavior against the model; read changelogs, model and system cards | Yes |
| Policy changed | Review provider policy pages, contribution rules, and model-card updates | Yes |
| Community posture changed | Track the community's own policy, bounty, or moderation changes after the outcome | Yes |
| Change persisted | Re-test across later releases to confirm it didn't silently revert | Yes |
| Attribution given | Look for the change credited to community feedback in changelogs or cards | Not yet |
| Compensation | Public records and self-report: grant, contract, sponsorship, or paid time | Not yet |
| Reciprocal contribution | Track provider contributions back to the project (code, fixes, infrastructure, roadmap seat) | Not yet |

### Efficiency of Feedback (community)

- **Description.** The cost of the loop to each side. On the community side, the effort to give feedback and the wait for a response. On the model-builder side, the effort and cost to respond and implement. Neither side's time is free.
- **Objectives.** Capture what the loop costs both communities and builders, so proportionality can be judged. A channel that technically exists but is expensive for a community to use, or slow and costly for a provider to answer, is not a working loop.
- **Implementation.** See data collection strategies section.

Existing CHAOSS metrics to draw on: [Time to First Response](https://www.chaoss.community/kb/metric-time-to-first-response/), [Issue Response Time](https://www.chaoss.community/kb/metric-issue-response-time/), [Labor Investment](https://www.chaoss.community/kb/metric-labor-investment/), [Collaboration Platform Activity](https://www.chaoss.community/kb/metric-collaboration-platform-activity/) and Inclusivity

| Indicator | Cost to | Implementation | Measurable now? |
| --- | --- | --- | --- |
| Effort to give feedback | Community | Classify effort: single message, incident report, blog post, or multi-project letter | Yes |
| Wait for a response | Community | Timestamp from submission to first response (the time a community waits) | Yes |
| Escalation count | Community | Count how many times feedback had to be repeated or escalated | Yes |
| Provider effort & cost | Provider | Infer from public timing (time to acknowledgment, time to change, whether it shipped); otherwise provider self-report | Not yet |

## Data collection strategies

Known methods (as of this writing) for collecting data related to metrics.

| Attribute | How we'd collect it | Detectable today? |
| --- | --- | --- |
| Channel exists | Manual audit of provider sites, repos, docs, foundation channels | Partial. Public channels found by audit; private arrangements unknown |
| Reachable | Read stated requirements; community self-report on real usability | Partial. Requirements visible; usability needs community reporting |
| Governance behind signal | Read project decision process / consensus records where published | Partial. Visible where projects document governance |
| Model behavior changed | Re-test against the model; read changelogs, model & system cards | Partial. Visible in changelogs and testing; unknown under silent retraining |
| Policy changed | Review provider policy pages, contribution rules, model-card updates | Detectable when public |
| Community governance changed | Track the community's own policy, bounty, or moderation changes | Detectable; it's the community's own record |
| Attribution given | Look for change credited to community feedback in changelogs / cards | Unknown. Providers rarely attribute |
| Compensation | Public records and self-report: grant, contract, sponsorship, paid time | Partial. Public funding detectable; private needs self-report |
| Reciprocal contribution | Track provider contributions back to the project (code, fixes, infra) | Partial. Public detectable; informal unknown |
| Change persisted | Re-test across later releases to confirm no silent revert | Partial. Needs ongoing testing and version disclosure |
| Effort to give feedback | Classify: single message, incident report, blog post, multi-project letter | Partial. Public visible; private needs self-report |
| Time to response | Timestamp from submission to first response | Partial. Public visible; private needs self-report |
| Escalation count | How many times feedback was repeated or escalated | Partial. Visible when public |
| Provider effort & cost | Infer from public timing; otherwise provider self-report | Unknown. Provider-side cost not disclosed |

## Tooling & signals (that might) be available

- Public submission threads on provider repos, maintainer forums, foundation channels.
- Provider changelogs, model cards, system cards.
- Public post-mortems and incident write-ups by maintainers.
- Foundation-level statements (Linux Foundation, OpenInfra) as proxies for collective feedback weight.
- vibebench.standardagents.ai: an existing tool we know of
- GitHub MCP

## Visualizations

- Funnel: submissions → acknowledged → substantive response → observable change → persistent change → reciprocal value.
- Three-axis plot (effectiveness, efficiency, value exchange) scoring the same incident on each, split by core vs. ask tier.
- Provider comparison: response rate, time-to-acknowledgment, time-to-change, attribution rate, reciprocal-value rate.
- Escalation map: steps required for each successful change, with value-exchange outcome at each tier.

## Appendix

### Acronyms

| Acronym | Meaning |
| --- | --- |
| RLHF | Reinforcement Learning from Human Feedback - training a model from human preference judgments. |
| RLVR | Reinforcement Learning from Verifiable Rewards - training on tasks where correctness is checkable (math, code, format compliance), not subjective preference. |
| CAI | Constitutional AI - using a written set of principles plus AI feedback in place of some human labels. |
| Reward model | A model trained on preference data that scores outputs, standing in for the "true" objective during RL. |
| Preference data | Pairs of responses where a human or AI marked which is better; the fuel for RLHF. |
| Model / system card | Provider-published doc describing a model's behavior, limits, and changes. |
| SLA | Service-Level Agreement - a documented commitment to respond within defined scope and time. |
| Synthetic Data | Training examples generated by an AI model rather than collected from people, often produced and ranked by models against a set of principles (as in Constitutional AI). One of the structured intake paths builders control, alongside paid annotators. |

### Precedents

**Collective Constitutional AI (Anthropic × CIP, 2023)**
~1,000 representative members of the US public used the Polis platform to propose and vote on principles; a model was then trained on the resulting constitution. The closest proof that external input can become a real training signal, but values-level and one-time, not source-community defect feedback.

**Alignment Assemblies (Collective Intelligence Project)**
A program of public-input processes feeding collective intelligence into AI development. One ran with the Creative Commons Foundation on how CC should respond to CC-licensed work in AI training: the nearest to a content-community governance question, and CC is in our references.

**Democratic Inputs to AI (OpenAI grant program)**
Funded teams prototyping democratic processes for deciding AI behavior rules. Institutional precedent for soliciting external input; again values/governance rather than maintainer feedback.

**Meta Community Forum on generative AI**
A deliberative forum gathering public views on generative-AI policy. Public-values input, not source-community intake.

**Columbia Convening on Openness & AI Safety (2024 → proceedings 2025)**
Insufficient participatory mechanisms for the communities most affected by AI harms, with a roadmap prioritizing participatory inputs and expanded harm taxonomies. The closest existing framing to this metric, and recent. (Earlier readout: [blog.mozilla.org/en/mozilla/ai/columbia-convening-research-agenda/](https://blog.mozilla.org/en/mozilla/ai/columbia-convening-research-agenda/).)

**PiPrO — Participatory-informed Preference Optimization (PLOS Digital Health, 2026)**
The most recent example: a reinforcement-learning method that folds community-derived input alongside expert input via continuous feedback, letting communities directly shape model recommendations. A healthcare-domain simulation study, but conceptually the nearest to a feedback loop built into optimization rather than one-off public-values collection.

## References

**Framing**

- Irwin, E. (2026). After the Pull Request: Four Proposed Areas of Work for Open Community Representation. [https://sunnydeveloper.com/](https://sunnydeveloper.com/)
- Irwin, E. AI Consent for Open Communities. [https://sunnydeveloper.com/ai-consent-for-open-communities/](https://sunnydeveloper.com/ai-consent-for-open-communities/)
- Creative Commons (2026). Update on CC Signals: What Changed and Why. [https://creativecommons.org/2026/04/23/update-on-cc-signals-what-changed-and-why/](https://creativecommons.org/2026/04/23/update-on-cc-signals-what-changed-and-why/)
- Invest in Open Infrastructure: Sustaining the Commons in the AI Economy: A Landscape Scan of Challenges and Strategies for Bridging AI Companies and Open Curated Collections

**Existing partial feedback loops between maintainers and AI / agent providers**

- GitHub maintainer discussion #470. [https://github.com/community/maintainers/discussions/470](https://github.com/community/maintainers/discussions/470)
- GitHub maintainer discussion #442. [https://github.com/community/maintainers/discussions/442](https://github.com/community/maintainers/discussions/442)
- GitHub maintainer discussion #646. [https://github.com/community/maintainers/discussions/646](https://github.com/community/maintainers/discussions/646)

**Effectiveness via escalation: feedback that worked only after public escalation**

- Stenberg, D. Death by a thousand slops. [https://daniel.haxx.se/blog/2025/07/14/death-by-a-thousand-slops/](https://daniel.haxx.se/blog/2025/07/14/death-by-a-thousand-slops/)
- The New Stack: Drowning in AI Slop Reports, curl Ends Bug Bounties. [https://thenewstack.io/drowning-in-ai-slop-reports-curl-ends-bug-bounties/](https://thenewstack.io/drowning-in-ai-slop-reports-curl-ends-bug-bounties/)

**Constructive examples of feedback resulting in better behavior**

- Joshua Rogers' Curl contributions. [https://mastodon.social/@bagder/115241241075258997](https://mastodon.social/@bagder/115241241075258997)

**Foundation-level positions**

- Linux Foundation generative AI policy. [https://www.linuxfoundation.org/legal/generative-ai](https://www.linuxfoundation.org/legal/generative-ai)
- OpenInfra Foundation AI policy. [https://openinfra.org/legal/ai-policy](https://openinfra.org/legal/ai-policy)

**CTA for model builders**

Be the first open model builder to demonstrate alignment with open source communities

## Contributors

- Emma Irwin
- Coraline Ada Ehmke
- Justin Wheeler
- Adrian Edwards

Add your name if you contributed

## Additional Information

To edit this metric please submit a Change Request here: (replace with correct link once metric is added to a focus area repo)

To reference this metric in software or publications please use this stable URL: (replace with permalink once published)
