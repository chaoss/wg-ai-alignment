# Preference Signaling for AI Training: Where Our Community Can Contribute

*Based on Stefano Maffulli's "[The Landscape of Preference Signaling for AI Training," April 2026*](https://www.maffulli.net/the-landscape-of-preference-signaling-for-ai-training/), please find a list of initiatives and ways to connect, contribute and review.

---

## Why This Matters

The open web and software commons were built without anticipating that everything created would be used to train AI systems. A range of initiatives is now working to establish reciprocity between AI developers and the communities whose work powers them.

This document maps the current landscape of preference signaling initiatives and where participation is possible based on the mapping from Stefano's paper./

---

## The Initiatives

---

### 1. IETF AI Preferences (AiPref) Working Group

**What it is:** Building the shared vocabulary and technical standards that all other initiatives reference. The foundational layer of preference signaling.

**Governance:** Open standards body (IETF). Community-run, standards-track process.

**Status:** Active. RFC expected late 2026/early 2027.

**Where to participate:**
- [Working Group home](https://ietf-wg-aipref.github.io/)
- [IETF Datatracker](https://datatracker.ietf.org/wg/aipref/about/)
- [GitHub repository](https://github.com/ietf-wg-aipref/drafts)
- Mailing list: [ai-control@ietf.org](mailto:ai-control@ietf.org) / [Archive](https://mailarchive.ietf.org/arch/browse/ai-control/) / [Subscribe](https://www.ietf.org/mailman/listinfo/ai-control/)

---

### 2. TDM-AI Protocol

**What it is:** Cryptographically binds creator preferences to content using content-derived fingerprints (ISCC identifiers). Preferences travel with the content even if metadata is stripped or files are moved.

**Governance:** Developed by [Liccium B.V.](https://liccium.com/), a Dutch rights management company. The [CommonsDB](https://openfuture.eu/project/commonsdb/) registry implementation is EU co-funded.

**Status:** Active development. CommonsDB registry due July 2026.

**Where to participate:**
- [TDM-AI documentation](https://docs.tdmai.org/)
- [GitHub repository](https://github.com/liccium/tdmai)

---

### 3. Really Simple Licensing (RSL)

**What it is:** Machine-readable licensing built on RSS, adding compensation models (pay-per-crawl, pay-per-inference) and content protection. Includes the RSL Collective for smaller publishers and creators.

**Governance:** Standard maintained by the RSL Technical Steering Committee, representing major publishing and technology companies. The [RSL Collective](https://rslcollective.org/) is a nonprofit collective rights organization, free to join.

**Status:** RSL 1.0 published December 2025.

**Where to participate:**
- [RSL Standard](https://rslstandard.org/)
- [GitHub repository](https://github.com/rslstandard/rsl)
- [RSL Collective](https://rslcollective.org/) (nonprofit, free to join)

---

### 4. Creative Commons Signals

**What it is:** A framework for data stewards (organizations managing large content collections such as Common Crawl, libraries, and data cooperatives) to express reciprocity conditions for AI reuse. Four signal types: Credit, Direct Contribution, Ecosystem Contribution, and Open.

**Governance:** Led by [Creative Commons](https://creativecommons.org/), a nonprofit organization.

**Status:** Draft proposal. Community input sought via GitHub.

**Where to participate:**
- [CC Signals overview](https://creativecommons.org/ai-and-the-commons/cc-signals/)
- [GitHub repository and discussions](https://github.com/creativecommons/cc-signals)

---

### 5. CodeCommons / AI Preference Attachment for Software

**What it is:** Builds on the [Software Heritage](https://www.softwareheritage.org/) archive to create ethical AI training datasets. Proposes embedding AI preferences directly in file headers so they travel with code when copied or vendored into other projects.

**Governance:** Funded by the French government via the France 2030 program. Academic and institutional partners in France and Italy.

**Status:** Actively developed.

**Where to participate:**
- [CodeCommons project](https://codecommons.org/)
- [Software Heritage GitLab](https://gitlab.softwareheritage.org/)

---

### 6. Cloudflare AI Crawl Control

**What it is:** A service that gives website owners visibility and control over AI crawler access, with options to block, allow, or charge for access at the network edge.

**Governance:** A commercial product developed and controlled by [Cloudflare](https://www.cloudflare.com/).

**Status:** Launched July 2025.

**Where to follow:**
- [Cloudflare AI Crawl Control](https://www.cloudflare.com/ai-crawl-control/)

---

## Cross-Cutting Themes

A few shared challenges across all six initiatives, drawn from Maffulli's analysis:

**The acquisition layer:** Most signals operate at the moment of crawling. What happens to data after it is downloaded, and how preferences follow it through training and use, remains an open problem across all initiatives.

**Attribution is evolving:** Attribution in the AI era is likely to attach to datasets rather than individual works. What meaningful attribution looks like in practice is still being defined.

**Balancing access and protection:** Restricting AI crawler access can unintentionally affect beneficial uses alongside harmful ones.

**Global representation:** These initiatives are currently concentrated in Western Europe and North America.

---

*Contributions, corrections, and additions to this document are welcome via pull request.*