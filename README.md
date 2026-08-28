# awesome-llm-hallucination-detection
A curated collection of research papers, datasets, tools, implementations, and learning resources for detecting, evaluating, and mitigating hallucinations in Large Language Models (LLMs).
# Awesome Token-Level Uncertainty and Hallucination Detection

A curated collection of research papers, datasets, tools, implementations, and learning resources on token-level uncertainty as a predictor of hallucination in large language models (LLMs). This repository accompanies my AI-assisted research paper and citation-integrity audit on the same topic, organizing verified references and resources for anyone studying uncertainty quantification and factuality in LLMs.

## Contents

- [Overview](#overview)
- [AI-Assisted Research Paper](#ai-assisted-research-paper)
- [Citation Integrity Audit](#citation-integrity-audit)
- [Curated Research Papers](#curated-research-papers)
- [Datasets](#datasets)
- [Tools and Libraries](#tools-and-libraries)
- [GitHub Implementations](#github-implementations)
- [Tutorials and Learning Resources](#tutorials-and-learning-resources)
- [License](#license)

## Overview

Large language models generate text autoregressively, assigning probability distributions to each successive token. These distributions offer an internal signal of the model's confidence, making quantities like predictive entropy, token probability, and sequence likelihood natural candidates for estimating when a model is at risk of hallucinating. The central challenge is that this internal uncertainty is not the same thing as external truth: a model can be uncertain purely about *how* to phrase a correct answer, or confidently generate something false.

This repository organizes resources around that problem. It covers the foundations of predictive uncertainty (token probability, entropy, probability margins), the key limitation of naive entropy — that it conflates uncertainty about *meaning* with uncertainty about *wording* — and the methods developed to address it, including semantic entropy, semantic entropy probes, calibration-tuning, self-consistency analysis, and conformal abstention. It also surveys the broader research direction toward multilevel uncertainty frameworks that combine token-level signals with semantic disagreement, calibration, claim-level analysis, and external evidence, since no single uncertainty metric is a reliable standalone hallucination detector.

The goal is to provide a single, verified entry point into this literature for anyone building or evaluating hallucination-detection systems.

## AI-Assisted Research Paper

**Title:** Token-Level Uncertainty as a Predictor of Hallucination in Large Language Models

This paper reviews the theoretical foundations of predictive uncertainty in LLMs and surveys work on token probabilities, predictive entropy, sequence likelihood, calibration, semantic entropy, self-consistency, abstention, hidden-state uncertainty, and factuality evaluation. It argues that token-level uncertainty is a useful predictive risk signal but not a direct measure of truth, and concludes that reliable hallucination detection requires combining local uncertainty with semantic, calibrated, claim-level, and evidence-based methods.

[View Paper](paper/AI_Assisted_Research_Paper.pdf)

## Citation Integrity Audit

Before including any reference in this repository, each citation was checked for a correct title, authors, publication year, venue, and DOI, and verified to genuinely exist and match its linked source (via Google Scholar, Crossref, and publisher/ACL Anthology/arXiv records). References were not accepted simply because they were AI-generated — every entry listed under [Curated Research Papers](#curated-research-papers) reflects independent verification.

[View Audit](citation-audit/Citation_Integrity_Audit.pdf)

## Curated Research Papers

See [references/references.md](references/references.md) for the full categorized list (survey papers, foundational papers, recent research, methods, and applications).

## Datasets

See [datasets/datasets.md](datasets/datasets.md) for benchmark datasets relevant to hallucination and factuality evaluation.

## Tools and Libraries

See [tools/tools.md](tools/tools.md) for libraries and frameworks used to compute uncertainty and evaluate hallucination detection.

## GitHub Implementations

See [implementations/github-repositories.md](implementations/github-repositories.md) for reference implementations of the methods discussed in the paper.

## Tutorials and Learning Resources

*(To be added — see instruction sheet Section 8 for the minimum requirement of 5 authoritative resources, e.g. documentation, lectures, or benchmark guides.)*

## License

This repository's original content (README, curation, and audit) is released under the [MIT License](LICENSE). Linked papers, datasets, and tools remain under their respective original licenses.
