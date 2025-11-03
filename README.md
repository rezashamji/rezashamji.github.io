# Reza Shamji
Research Associate @ Zitnik Lab (Harvard Medical School)

I work on **foundational sequence & multimodal architectures beyond dense self-attention**, aiming for **reasoning, long memory, and stability**.  
I’m especially interested in **algorithmic memory** and **higher-order inductive biases**, and I study **non-attention candidates** (e.g., state-space / retention, long-convolution / implicit filters, retrieval systems) as **stepping stones to new designs** rather than endpoints.

---

## Preprints & Manuscripts

- **[Democratizing AI Scientists using ToolUniverse](https://arxiv.org/abs/2509.23426)** · *arXiv (2025)*  
  **Zitnik Lab — Harvard Medical School**  
  Co-author. Open ecosystem enabling agent access to **600 + scientific tools** ([aiscientist.tools](https://aiscientist.tools)); highlighted in  
  **[Nature (“How AI Agents Will Change Research”)](https://www.nature.com/articles/d41586-025-03246-7)**,  
  **[Science (“The silicon cell AI cell models could transform biomedicine — if they work as promised”)](https://www.science.org/content/article/can-ai-capture-mind-boggling-complexity-human-cell)**,  
  and **[Decoding Bio’s BioByte (“ToolUniverse Democratizes AI Scientists”)](https://decodingbio.substack.com/p/biobyte-134-tooluniverse-democratizes)**.  
  *(Nature Biotechnology submission under review.)*

- **Multimodal VLM architectures study** *(ICLR 2026 submission under review; anonymous)*  
  **Kempner Institute (Harvard – MIT) · Advised by Yilun Du & Sham Kakade**  
  Co-author. Conducted during a Kempner Institute internship on **vision-language model design choices** and **cross-modality transfer**.  
  *Title / link omitted for anonymity · manuscript available upon request · code examples available.*

---

## Research & Engineering

### Zitnik Lab — Research Associate  _(Sept 2025 – Present)_
- **Hybrid keyword + embedding datastore (SQLite FTS5 + FAISS):** ingest → deduplicate → embed → index pipeline with CLI + agent API; Hugging Face sync + local caching → labs and agents can instantly build **searchable knowledge bases**.  
- **EUHealth datasets:** transformed EU Health Portal metadata into a **weekly-refreshed index** with topic / country / language filters + a link classifier to flag downloadable datasets for reproducible population-level research.  
- **AlphaFold integration:** UniProt-driven flow for agents to fetch **predicted 3D structures**, **pLDDT**, and **PDB/mmCIF** files—adding structural biology evidence into agentic reasoning.  
- **ODPHP (preventive care):** integrated HHS **MyHealthFinder** to structure demographic-specific recommendations (age / sex / pregnancy), enabling **policy-grounded preventive-care guidance**.

*These engineering contributions underpin the ToolUniverse preprint above (arXiv 2025).*

---

### Kempner Institute — ML Research Engineer Intern (Multimodal AI)  _(Jun – Sept 2025)_
**Advised by Yilun Du & Sham Kakade**
- **End-to-end VQA benchmarking:** ChartQA, RealWorldQA, MMT-Bench, MathVista, DocVQA, TextVQA—dataset factories, OCR / table serialization, collate functions, and custom scorers (numeric relative error, **ANLS**, MCQ).  
- **Transformer / VLM infrastructure:** configurable **QK normalization** (LayerNorm, RMSNorm, custom) for robust OCR / vision token handling; integrated **Qwen3-8B** into cross-attention fusion with selective freezing; built a **YAML-driven LR-scheduler registry** (cosine warmup + custom).  
- **Training at scale:** multi-node **FSDP/DDP** on **H100s** via Slurm with **Weights & Biases** monitoring.

*This work forms the empirical and infrastructure core of the (anonymous) ICLR 2026 VLM submission above.*

---

## Technical Skills
**Python** (PyTorch; HF Transformers / Tokenizers; TorchVision), **Distributed** (DDP / FSDP / DTensor), **Slurm / NCCL**, **WebDataset**, **Pandas / Numpy**, **W&B**, **YAML**;  
**C++**, **Java**, **OCaml**; **Docker / Conda**; **SQL**  
**Hardware:** multi-node **H100 / A100** (e.g., 4 × 4 GPUs, FSDP)

---

## Education
**Harvard University** — A.B. in Computer Science (Secondary in Economics) · _Expected May 2025_

---

## Languages
**English** (native)  ·  **Mandarin** (fluent)

---

## Contact & Links
- Email:  rezamshamji@gmail.com  
- LinkedIn:  [LinkedIn Profile](https://www.linkedin.com/in/rezashamji/)  
- Github:  [GitHub Profile](https://github.com/rezashamji)

---

*Preprint policy:* The multimodal VLM submission is under double-blind review; **title and link intentionally omitted**. *Manuscript available upon request; code examples available.*
