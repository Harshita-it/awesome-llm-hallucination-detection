# Datasets

Benchmarks and datasets relevant to token-level uncertainty and hallucination detection in LLMs.

- **TruthfulQA**
  Source: [GitHub](https://github.com/sylinrl/TruthfulQA) / Lin, Hilton & Evans (2022)
  Description: 817 questions across 38 categories designed to probe whether models mimic human falsehoods rather than answer truthfully.
  Use: Standard benchmark for measuring factual reliability and calibration of model confidence.

- **FEVER (Fact Extraction and VERification)**
  Source: [fever.ai](https://fever.ai/)
  Description: ~185K claims labeled Supported / Refuted / NotEnoughInfo against Wikipedia evidence.
  Use: Useful for evaluating claim-level factuality verification alongside uncertainty scores.

- **HaluEval**
  Source: [GitHub](https://github.com/RUCAIBox/HaluEval)
  Description: Large-scale benchmark of LLM-generated hallucinated and non-hallucinated samples across QA, dialogue, and summarization.
  Use: Directly supports evaluating hallucination-detection methods, including uncertainty-based ones.

*Note: state clearly in your README that these are general-purpose reliability/hallucination benchmarks rather than domain-specific data, since your paper is a theoretical/survey piece rather than an applied study on a specific dataset.*
