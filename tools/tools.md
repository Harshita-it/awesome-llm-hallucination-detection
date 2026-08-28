# Tools and Libraries

Software and frameworks useful for implementing or experimenting with token-level and semantic uncertainty methods.

- **LM-Polygraph**
  [GitHub](https://github.com/IINemo/lm-polygraph)
  A library implementing many uncertainty quantification methods for LLMs (entropy, semantic entropy, ensembling) in one framework.

- **Hugging Face Transformers**
  [GitHub](https://github.com/huggingface/transformers) / [Docs](https://huggingface.co/docs/transformers)
  Standard library for loading LLMs and accessing token-level logits/probabilities needed for entropy computation.

- **SelfCheckGPT (toolkit)**
  [GitHub](https://github.com/potsawee/selfcheckgpt)
  Reference implementation of black-box, sampling-based hallucination detection via self-consistency.

- **OpenAI / Anthropic API logprobs**
  [OpenAI docs](https://platform.openai.com/docs/api-reference) 
  API-level access to token log-probabilities, useful for computing predictive entropy without hosting a model.

- **scikit-learn**
  [Docs](https://scikit-learn.org/)
  Useful for building calibration curves, ROC/AUROC analysis, and evaluating uncertainty-based detectors.
