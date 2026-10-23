# Policy Change

**Question:** How do communities' AI policies change over time, and how do those changes compare across projects?

This metric is part of the [AI Alignment - Community Governed Use](../ai-alignment-community-governed-use/metric-model-ai-alignment-community-governed-use.md) metrics model.

## Overview

Track documented AI-policy changes over time, classified using the [Consent Policy Specificity taxonomy of domains](https://github.com/chaoss/wg-ai-alignment/blob/main/metrics/ai-alignment-community-governed-use/ai-use-consent-policy-specificity.md#taxonomy-of-domains).

For each change, record the prior and revised provision, affected domain(s), change type and direction, source date, and evidence. Record the decision process and enforcement when documented.

This metric describes policy changes; it does not rate whether a policy is good, effective, or more aligned. A change in policy text does not by itself establish a change in practice. A project's history may be incomplete, and a selected set of projects does not establish an ecosystem-wide trend.

One revision may affect multiple domains or move in different directions. Classify each changed provision separately where practical.

**NOTE**: this can be tricky because the location of policy can be in any number of files.  Check all governance documents where possible.

## Want to Know More?

### Data Collection Strategies

#### Identify sources and establish the history checked

- Check relevant policy sources, such as repository history, contribution guides, codes of conduct, governance records, and project or foundation policy pages.
- Record each source, its history and the period or versions checked. Link findings to the relevant revision or decision.
- Distinguish checked history with no relevant change from history that was unavailable or not checked.
- Record the source-supported revision, merge, publication, or decision date. Note a separate effective date when known.

#### Compare revisions

Compare the prior and revised provision. Record:

- project, source document, and affected domain(s);
- prior and revised text, with context where needed;
- change type, direction, source date, and effective date if stated;
- links to the source evidence and a note where classification is uncertain.

Use **first-observed baseline** when the checked history does not establish when the policy began. A new policy is not automatically a tightening; report the history period checked.

#### Classify change type and direction

Classify the policy effect, not the size or tone of the edit:

- **Added provision:** a new rule appears. Record whether it is a first-observed baseline or an addition to an existing policy. Addition is a change type, not a direction.
- **Tightened:** narrows permitted use or strengthens an obligation, threshold, consequence, or enforcement.
- **Loosened:** broadens permitted use or reduces an obligation, threshold, consequence, or enforcement.
- **Mixed:** includes material changes in both directions. Split the record when practical; otherwise explain the combination.
- **Clarified / no direction established:** wording changes, but the evidence does not show a directional effect.
- **Removed provision:** record the removal; call it loosening only when it reduces a restriction or obligation.
- **Administrative / no substantive change:** formatting or relocation without a policy change. Exclude from directional totals.

These categories describe changes; they are not a severity scale. Base classifications on the policy text or decision record, not commit messages alone. State when direction is uncertain.

#### Record decision and enforcement information when available

Record these when documented; they are not required:

- **Decision process:** vote, consensus, maintainer decision, or other stated process; link to evidence.
- **Vote result:** result, turnout, margin, and eligible group or denominator when available. Otherwise use “not reported”; do not estimate.
- **Enforcement:** the stated mechanism, or “not stated.”
- **Implementation status:** proposed, adopted/effective, approved but not yet effective, or unknown when supported by evidence. Keep this separate from enforcement.

### Filters

Use the core filters for each change. Context filters are optional when sources provide them.

| Filter | Values or format | Why it is workable |
|---|---|---|
| Project / community | Project name or stable identifier | Every record belongs to a project. |
| Domain affected | One or more Consent Policy Specificity domains, or “unable to determine” | Use the taxonomy labels. Record multiple domains when applicable; explain uncertainty. |
| Change direction | Tightened, loosened, mixed, or no direction established | Keep direction separate from whether a provision was added or removed. |
| Change type | First-observed baseline, added, modified, removed, clarified, or administrative / no substantive change | Describes what changed, not how restrictive it is. |
| Source event date | Date and basis: revision, merge, decision, publication, or effective date | Use the date supported by the source; distinguish it from scan dates. |
| Evidence / history status | Direct evidence; partial history; no change found in checked history; unavailable or unchecked | Report only what was reviewed; no change found does not mean no change ever occurred. |
| Consent-type attribute changed | Supervision, scope, accountability, proportionality, or another supported attribute | These are cross-cutting attributes, not domains. |

#### Handling domain assignment

- Assign every affected domain supported by the evidence; do not force one primary  (AI policy specificity) domain.
- Treat supervision, scope, accountability, and proportionality as cross-cutting Consent-type attributes, not domains. Record them separately when relevant.
- Record disclosure as a provision where relevant; do not add it as a domain.
- If an observed change does not fit a domain, note it as outside the taxonomy and exclude it from domain comparisons.
- Use **unable to determine** when evidence cannot establish the subject or scope; state what is unclear. This is distinct from no change found or history unavailable.

Do not require every filter for every project. Distinguish unavailable, not stated, and not applicable when supported. Do not add policy elements as domains.

### Comparisons across projects

State the projects and sources, period examined, and whether the sample is exhaustive, a defined cohort, or purposive. Report how many histories were checked alongside change counts.

Compare changes by domain, type, and direction, with the period and history coverage shown. Raw counts do not measure policy strictness or change rates without a defensible sample and denominator.

### Visualizations

- A linked timeline of policy revisions by date, project, domain, and change type/direction.
- A project-by-domain view showing the direction and type of each change.
- A comparison view that includes the sample, period, and history coverage.

Do not place first-observed baselines on a tightening/loosening scale. Show a legend when color or position indicates direction; direction is qualitative, not a measured score.

Example timeline from the pilot ([Reference link](https://github.com/emmairwin/ai-oss-use-specificity/blob/main/reports/policy-change-2026-10-23.md)):

![Example timeline of 28 policy revisions across 21 projects. Markers link to source evidence, colors identify projects, and numbered entries list revisions in chronological order with domain labels.](https://github.com/emmairwin/ai-oss-use-specificity/blob/main/images/2026-10-23/policy-change.svg)

## References

- [Consent Policy Specificity taxonomy of domains](https://github.com/chaoss/wg-ai-alignment/blob/main/metrics/ai-alignment-community-governed-use/ai-use-consent-policy-specificity.md#taxonomy-of-domains)
- CHAOSS AI Alignment Collection of [AI Policies](https://github.com/chaoss/wg-ai-alignment/blob/main/moderation/README.md)

## Contributors

- Emma Irwin
- Adrian Edwards
- Justin Wheeler
- Coraline Ada Ehmke
- Omkar Petkar
- Andrew Nesbitt

Add your name if you have contributed.

## Additional Information

To edit this metric, please submit a Change Request using the process designated by the CHAOSS AI Alignment working group.

To reference this metric in software or publications, use its stable URL.
