# Reza Shamji

Research Associate @ Zitnik Lab (Harvard Medical School)

I work on **foundational sequence & multimodal architectures beyond dense self-attention**, aiming for **reasoning, long memory, and stability**.  
I’m especially interested in **algorithmic memory** and **higher-order inductive biases**, and I study **non-attention candidates** (e.g., state-space / retention, long-convolution / implicit filters, retrieval systems) as **stepping stones to new designs** rather than endpoints.

---

## Preprints & Manuscripts

- **[Democratizing AI Scientists using ToolUniverse](https://arxiv.org/abs/2509.23426)** · *arXiv 2025*  
  Zitnik Lab — Harvard Medical School · Co-author. Open ecosystem enabling agent access to **600+ scientific tools** ([aiscientist.tools](https://aiscientist.tools)).  
  Highlighted in [Nature](https://www.nature.com/articles/d41586-025-03246-7), [Science](https://www.science.org/content/article/can-ai-capture-mind-boggling-complexity-human-cell), and [Decoding Bio / BioByte](https://decodingbio.substack.com/p/biobyte-134-tooluniverse-democratizes).  
  *(Nature Biotechnology submission under review.)*

- **Multimodal VLM architectures study** · *ICLR 2026 submission under review (anonymous)*  
  Kempner Institute (Harvard–MIT) · Co-author, advised by Yilun Du & Sham Kakade.  
  Empirical study of **vision–language model design choices** and **cross-modality transfer**.  
  *Title/link omitted for anonymity; manuscript available on request.*

---

## Research & Engineering

### Zitnik Lab — Research Associate  _(Sept 2025 – Present)_

- Built a hybrid **keyword + embedding datastore (SQLite FTS5 + FAISS)** with CLI + agent API, letting labs transform their **own data (text/JSON) into searchable, agent-accessible knowledge bases** with Hugging Face sync and ToolUniverse integration.
- Transformed **EU Health Portal** metadata into a weekly-refreshed index with topic / country / language filters and a link classifier for reproducible population-level studies.
- Integrated **AlphaFold / UniProt** flows so agents can fetch predicted 3D structures (pLDDT, PDB/mmCIF) as part of their reasoning.
- Connected HHS **MyHealthFinder** to structure demographic-specific preventive-care recommendations (age / sex / pregnancy).

<small>These contributions underpin the ToolUniverse preprint above.</small>

---

### Kempner Institute — ML Research Engineer Intern (Multimodal AI)  _(Jun – Sept 2025)_

Advised by Yilun Du & Sham Kakade.

- Built **end-to-end VQA benchmarking** for ChartQA, RealWorldQA, MMT-Bench, MathVista, DocVQA, TextVQA, including dataset factories, OCR/table serialization, collate functions, and custom scorers (numeric error, ANLS, MCQ).
- Implemented configurable **QK normalization** (LayerNorm, RMSNorm, custom) and integrated **Qwen3-8B** into cross-attention fusion with selective freezing plus a YAML-driven LR scheduler registry.
- Ran large-scale training with **FSDP/DDP on H100s** via Slurm, with Weights & Biases monitoring.

<small>These contributions underpin the VLM preprint above.</small>

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
- **ML / DL:** PyTorch, HF Transformers & Tokenizers, TorchVision, WebDataset  
- **Systems & Scaling:** DDP, FSDP, DTensor, Slurm, NCCL, Docker, Conda  
- **Data / Tooling:** Pandas, NumPy, YAML, Weights & Biases  
- **Hardware:** multi-node H100 / A100 (e.g., 4×4 GPUs with FSDP)

---

## Education

**Harvard University** — A.B. in Computer Science (Secondary in Economics)  
Expected May 2025

---

## Languages

English (native) · Mandarin (fluent)

---

## Contact & Links

- Email:  rezashamji@gmail.com  
- LinkedIn:  [LinkedIn Profile](https://www.linkedin.com/in/rezashamji/)  
- GitHub:  [GitHub Profile](https://github.com/rezashamji)
- CV: [Download CV (PDF)](/Reza_Shamji_CV.pdf)

<small>
Preprint policy: the multimodal VLM submission is under double-blind review; title and link are intentionally omitted. Manuscript available upon request; code examples available.
</small>
