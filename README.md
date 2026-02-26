# Reza Shamji

**Research Associate** @ Zitnik Lab (Harvard Medical School)
*PhD applications due Fall 2026 (hopeful entry Fall 2027) — theoretical deep learning & alternatives to neural networks*

---

## 🔍 Looking for Collaborations

I'm actively seeking **exposure to theoretical deep learning research** before submitting PhD applications this fall. If you work on alternatives to gradient descent, transformer architecture theory, model implicit bias, and/or transfomer/SSM/alternative to transformer training dynamics—**I'd love to connect**. Early feedback and collaborative projects would help ground my research direction.

---

## Research Vision

I’m driven by a fundamental question: **Is gradient descent on deep neural networks the right path toward artificial intelligence?**

My research interests span two interconnected directions:

**1. LLM Reasoning & Knowledge Integration**
Currently, I study how large language models leverage external knowledge—particularly when knowledge *helps* vs. *harms* performance. I’m developing **model-agnostic predictors** to determine when retrieval-augmented systems should be deployed, understanding the inductive biases that govern when agent decision-making improves under external constraints.

**2. Theoretical Deep Learning & Architecture Alternatives**
My longer-term vision is to rethink artificial intelligence from first principles. I believe understanding the mathematics of transformers—attention mechanisms, QKV matrices, MLP/hidden state dynamics—is essential groundwork. But I’m skeptical that gradient descent is the most computationally representative path to general intelligence. During my PhD, I plan to:
- **Explore alternative learning paradigms** beyond gradient descent, potentially informed by (but not limited to) neuroscience
- **Question core assumptions** about what makes a system "intelligent," building toward methods that may fundamentally differ from current neural network approaches

---

## Preprints & Manuscripts

- **[Democratizing AI Scientists using ToolUniverse](https://arxiv.org/abs/2509.23426)** · *arXiv 2025*
  Zitnik Lab — Harvard Medical School · Co-author, advised by [Marinka Žitnik](https://zitniklab.hms.harvard.edu/bio/).
  Open ecosystem enabling agent access to **1600+ scientific tools** ([aiscientist.tools](https://aiscientist.tools)). Partnered with Anthropic's Claude. ToolUniverse serves as an official research connector within Claude to power scientific discovery.
  Featured in [Nature](https://www.nature.com/articles/d41586-025-03246-7), [Science](https://www.science.org/content/article/can-ai-capture-mind-boggling-complexity-human-cell), and [DecodingBio's BioByte](https://decodingbio.substack.com/p/biobyte-134-tooluniverse-democratizes).

- **Understanding the Design Space and Cross-Modality Transfer for Vision-Language Models** · *ICML submission under review*
  Kempner Institute (Harvard) · Co-author, advised by [Yilun Du](https://yilundu.github.io/) & [Sham Kakade](https://shamulent.github.io/).
  Systematically mapped VLM design choices across image tokenizers, fusion architectures (Joint-Decoder, Cross-Attention, Mixture-of-Transformers), and layer-freezing recipes on a Qwen3 backbone, evaluating 50+ controlled configurations. Introduced three synthetic cross-modality transfer datasets (SpatialMap/Grid/Ring) with matched image-text task pairs to isolate AI reasoning from perception. *Manuscript/code available upon request.*

---

## Research & Engineering

### [Zitnik Lab](https://zitniklab.hms.harvard.edu/) — Research Associate  _(Sept 2025 – Present)_

**Foundational LLM Health Reasoning & Knowledge Integration**
- Studying **inductive biases in retrieval-augmented clinical decision making** — developing model-agnostic predictors for when external knowledge (e.g., knowledge graphs) improves vs. degrades LLM performance
- Implemented and evaluated **GRPO** to study post-training reasoning methods for health reasoning tasks
**External Stakeholder Collaboration**
- Coordinating deliverables with **Gates Foundation** to translate research findings into deployable AI products

**Infrastructure & ToolUniverse Integration**
- Architected a hybrid **semantic-keyword datastore (SQLite FTS5 + FAISS)** with CLI + agent APIs, enabling researchers to convert lab-specific documents into AI-searchable collections for private or public use
- Transformed **FAIR DCAT-AP metadata** into a weekly-refreshed database of ~300 EU public-health datasets (21 tools; disease surveillance, cancer registries, mortality) with structured filtering and automated link extraction
- Integrated **AlphaFold (UniProt)** and **HHS MyHealthFinder** APIs to ground agent reasoning in structural biology and clinical guidance
- Driving **CZI Biohub partnership** to integrate foundation models into ToolUniverse for molecular/protein discovery
<small>Core infrastructure and findings underpin the [ToolUniverse preprint](https://arxiv.org/abs/2509.23426) ("Democratizing AI Scientists using ToolUniverse").</small>



---

### Kempner Institute — ML Research Engineer Intern (Multimodal AI)  _(Jun – Sept 2025)_

Advised by [Yilun Du](https://yilundu.github.io/) & [Sham Kakade](https://shamulent.github.io/).

**Large-Scale Ablation Study & Key Findings**
- **Image tokenizers trained with text-aware objectives** consistently outperform text-blind tokenizers
- **Modality-separated fusion (Mixture-of-Transformers)** with freezing recipes that preserve base LLM knowledge improves out-of-domain generalization
- **Cross-modality transfer is limited** without tightly aligned/structured representations; image→text transfer stronger than text→image

**Infrastructure & Benchmarking**
- Built **end-to-end VQA benchmarking** for ChartQA, RealWorldQA, MMT-Bench, MathVista, DocVQA, TextVQA: dataset factories, OCR/table serialization, collate functions, and custom scorers (numeric relative-error, ANLS, MCQ)
- Implemented configurable **query-key normalization** (LayerNorm, RMSNorm, custom) to stabilize OCR/vision token processing
- Integrated **Qwen3-8B** into cross-attention fusion with selective freezing and developed a **YAML-driven LR scheduler registry** (cosine warmup, custom schedulers)
- Ran multi-node training/eval (**FSDP/DDP on H100s**) using Slurm with W&B monitoring

<small>Findings underpin the VLM architecture design space preprint (ICML 2026 submission under review, manuscript and code available upon request).</small>

---

## Selected Projects

### ChainEnv RL Benchmarks (JAX)

A compact sandbox to probe **exploration under sparse rewards** in a tunable 1-D chain (pure, vectorized JAX; laptop-friendly).  
**Repo:** [github.com/rezashamji/jax-chainenv-benchmarks](https://github.com/rezashamji/jax-chainenv-benchmarks)

- Compares **PPO, PQN, DDPG, SAC** with deterministic evaluation vs exploratory training.
- Cleanly separates **exploration** from **optimization** and contrasts **on-policy** vs **off-policy** credit flow.
- Shows that as difficulty rises, learning becomes **exploration-limited** (not optimizer-limited); SAC/PQN help when discovery is easy, harder settings need discrete critics or intrinsic bonuses/parallelism.

---

## Technical Skills

- **Languages:** Python, C++, Java, OCaml, SQL  
- **ML / DL:** PyTorch, JAX, HF Transformers & Tokenizers, TorchVision, WebDataset  
- **Systems & Scaling:** DDP, FSDP, DTensor, Slurm, NCCL, Docker, Conda  
- **Data / Tooling:** Pandas, NumPy, YAML, Weights & Biases  
- **Hardware:** multi-node H100 / A100 (e.g., 4×4 GPUs with FSDP)

---

## Education

**Harvard University** — A.B. in Computer Science (Secondary in Economics)
*May 2025*

**Relevant Coursework:** Algorithms & Limitations, Distributed Systems & Machine Organization, Semantics of Programming Languages, Probability, Linear Algebra

---

## Languages

English (native) · Mandarin (fluent)

---

## Contact & Links

- Email:  reza_shamji@hms.harvard.edu 
- LinkedIn:  [LinkedIn Profile](https://www.linkedin.com/in/rezashamji/)  
- GitHub:  [GitHub Profile](https://github.com/rezashamji)
- CV: [Download CV (PDF)](/Reza_Shamji_CV.pdf)
