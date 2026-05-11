# Reza Shamji

**Research Associate** @ Zitnik Lab (Harvard Medical School)
*Applying to **PhDs in mathematics**, Fall 2026 — chasing whether free will and consciousness can be mathematically modeled.*

---

## Research Vision

**The question I want to spend my life on:** can free will and consciousness be **mathematically modeled** — or are humans, in some formal sense, *beyond* mathematics? That is the single thing I want to know before I die, and the reason I am applying to **PhDs in mathematics** this fall.

**Why I'm starting in AI:** because it is the closest thing to **mathematically-defined human reasoning** I have seen in my lifetime, which makes it the right place to begin — even though it isn't the destination. Even "superintelligence," as it's usually defined, lives in the language of productivity and economic value, not the language of agency, free will, or consciousness. AI gets me near the math. The math is what I will need to take the bigger question further.

**Within AI, the bet I'm making:** backpropagation — the chain rule we use to update every weight in a network — *does not look like how brains actually learn*. Real neurons appear to update **locally**: each connection adjusts based on the activity of the two cells it sits between, sometimes gated by a chemical signal like dopamine. Backprop, by contrast, needs a global error signal that travels backwards across the entire network through carefully matched weights — something brains do not appear to implement. Whether the brain nonetheless *approximates* something gradient-like through some other mechanism is genuinely open. And backprop has its own problems even in silico — vanishing gradients, credit assignment, an implicit-bias story still unsettled. The honest position is that **the function-update rule is the open frontier**; if we want intelligences different from the ones gradient descent produces, that is where I want to look first.

**And this is where the small question meets the large one.** The bet on alternatives to backprop holds in both directions AI could be heading. *If* the goal is to reach the human brain — the highest intelligence we have evidence of — backprop is the wrong tool, for the reasons above. *If* the goal is to surpass it (which I find more honest — humans have     placed ourselves at the center of the world, and assuming the brain is the ceiling of possible intelligence is the same instinct), backprop has scaled impressively and may keep doing so, but empirically, scaled backprop today has not even reached human-level intelligence. In either case, I think an alternative function-update rule is required — to close that gap, and to push past it.

That is what connects this work to the bigger question. I'm not claiming the math of free will and consciousness lives literally inside an alternative to backprop — that would be a leap. What I am claiming is that chasing such an alternative is the closest *grounded* AI problem to the question I actually care about: close enough to give me a real taste of the mathematical foundations, and concrete enough that I can do real work on it now — instead of waving hands about consciousness from the outside.

Before my PhD, I want to work on:
- **Alternatives to gradient descent** as the substrate of learning — local update rules, energy-based methods, biologically-plausible updates, anything that lets a function improve itself without backprop's global signal
- **The mathematics of why current architectures work at all** — attention, implicit bias, training dynamics — as the groundwork for proposing what comes after

---

## ◆ <span style="color: #0F79D0;">Looking for Collaborations</span>

I'm looking for collaborators before I submit math PhD applications this fall. If you work on **alternatives to backpropagation**, the **mathematics of why current architectures work**, or formal approaches to **consciousness, agency, or free will** (however speculative) — **I'd love to connect**. Early feedback and shared projects would help me ground my direction before applications.

---

## Writing

- **[How AI Actually Works](https://rezashamji.substack.com/p/how-ai-actually-works)** · *Substack, May 2026*
  An explanation of AI from the ground up — through the math, with no prerequisites and no buzzwords. Walks Vision Transformers from pixels → patch embeddings → Q/K/V attention → vision-language models, and connects to the question I'm actually chasing: whether consciousness and free will can be mathematically modeled.
- More writing at [rezashamji.substack.com](https://rezashamji.substack.com).

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

**KG-Router — Knowledge-Graph–Grounded Routing for High-Stakes QA**
- Building **KG-Router**: training an LLM agent to *route over typed tools* in a curated knowledge graph rather than free-generating answers. The goal is **reliable, auditable retrieval** in domains where hallucination has real consequences — medicine, law, science.
- The shift in framing: stop asking *"what does the model say?"* and start asking *"which slice of grounded knowledge does it consult, and in what order?"* The routing policy is trained via **SFT followed by RL** on (query → tool sequence → grounded answer) traces, evaluated against ungrounded-LLM and naïve-RAG baselines.
- Validating in medical QA first (HealthBench, AfriMedQA), with early results showing meaningful gains over both ungrounded and naïve-RAG baselines. The contribution I'm targeting, though, is the **methodology** — converting any heterogeneous knowledge graph into a typed tool surface an LLM can route over reliably — not the medical numbers themselves.

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
