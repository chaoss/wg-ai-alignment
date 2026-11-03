# AI-Assisted Contributions Policy

This is the AI policy of the CHAOSS AI Alignment Working Group. It is a fork of the [Fedora AI-Assisted Contributions Policy](https://docs.fedoraproject.org/en-US/council/policy/ai-contribution-policy/); see [Attribution and License](#attribution-and-license).

You MAY use AI assistance for contributing to the AI Alignment Working Group, as long as you follow the principles described below.

## Accountability

You MUST take the responsibility for your contribution. Contributing to this working group means vouching for the quality, license compliance, and utility of your submission. All contributions, whether from a human author or assisted by large language models (LLMs) or other generative AI tools, must meet the working group's standards for inclusion. The contributor is always the author and is fully accountable for the entirety of these contributions.

## Transparency

You MUST disclose the use of AI tools when the significant part of the contribution is taken from a tool without changes. You SHOULD disclose the other uses of AI tools, where it might be useful. Routine use of assistive tools for correcting grammar and spelling, or for clarifying language, does not require disclosure.

Information about the use of AI tools will help us evaluate their impact, build new best practices and adjust existing processes.

Disclosures are made where authorship is normally indicated. For contributions tracked in git, the recommended method is an `Assisted-by:` commit message trailer, placed alongside the `Signed-off-by:` line required by the [Developer Certificate of Origin](CONTRIBUTING.md#developer-certificate-of-origin-dco). For other contributions, disclosure may include a note in the pull request description or issue comment, a document preamble, or presentation speaker notes.

Examples:

```
Assisted-by: generic LLM chatbot
Assisted-by: ChatGPTv5
```

## Contribution & Community Evaluation

AI tools may be used to assist human reviewers by providing analysis and suggestions. You MUST NOT use AI as the sole or final arbiter in making a substantive or subjective judgment on a contribution, nor may it be used to evaluate a person's standing within the community (e.g., for funding, leadership roles, or Code of Conduct matters). This does not prohibit the use of automated tooling for objective technical validation, such as CI/CD pipelines, automated testing, or spam filtering. The final accountability for accepting a contribution, even if implemented by an automated system, always rests with the human contributor who authorizes the action.

## Large Scale Initiatives

The policy does not cover the large scale initiatives which may significantly change the ways the working group operates or lead to exponential growth in contributions in some parts of the working group. Such initiatives need to be discussed separately with the [working group co-chairs](CONTRIBUTING.md#working-group-chairs).

## Reporting Concerns

Concerns about possible policy violations should be reported privately to the [working group co-chairs](CONTRIBUTING.md#working-group-chairs). Concerns that also involve a Code of Conduct matter should be reported to the CHAOSS Code of Conduct Team at chaoss-conduct@googlegroups.com, following the [Procedure for making a Code of Conduct report](https://chaoss.community/procedure-for-making-a-code-of-conduct-report/).

The key words "MAY", "MUST", "MUST NOT", and "SHOULD" in this document are to be interpreted as described in [RFC 2119](https://datatracker.ietf.org/doc/html/rfc2119).

## Attribution and License

This policy is adapted from the [Fedora AI-Assisted Contributions Policy](https://docs.fedoraproject.org/en-US/council/policy/ai-contribution-policy/) (Version 1.0, last reviewed 2025-10-24) by Jason Brooks, the Fedora Council, and the Fedora community, used under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/). Changes from the original: references to Fedora and the Fedora Council were replaced with this working group and its co-chairs, and the disclosure methods and reporting channels were adapted to how this working group operates.

This document is licensed under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/). The rest of this repository is licensed under the [MIT License](LICENSE.txt).
