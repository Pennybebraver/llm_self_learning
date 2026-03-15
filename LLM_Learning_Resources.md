# LLM Learning Resources & Evaluation Framework Guide

A curated collection of open-source materials for learning about Large Language Models (LLMs), with a special focus on LLM auto-evaluation frameworks — ideal for building a career in this space.

---

## Part 1: Foundational LLM Courses (Beginner-Friendly)

### University Courses (Free / Open Materials)

| Course | Institution | What You'll Learn | Link |
|--------|-------------|-------------------|------|
| **CS336: Language Modeling from Scratch** | Stanford | Build an LLM end-to-end: data collection, tokenizer, transformer architecture, training, evaluation | [cs336.stanford.edu](https://cs336.stanford.edu/) |
| **CME 295: Transformers & Large Language Models** | Stanford | Transformer architecture, NLP evolution, practical LLM techniques; includes an illustrated cheatsheet | [cme295.stanford.edu](https://cme295.stanford.edu/) |
| **CS324: Advances in Foundation Models** | Stanford | LLM harms (toxicity, bias), training architectures, societal impacts | [stanford-cs324.github.io](https://stanford-cs324.github.io/winter2022/) |
| **CS224N: NLP with Deep Learning** | Stanford | Deep learning foundations for NLP, attention mechanisms, transformers | [web.stanford.edu/class/cs224n](https://web.stanford.edu/class/cs224n/) |

### Self-Paced Open-Source Courses

| Course | Provider | Best For | Link |
|--------|----------|----------|------|
| **LLM Course (3-part roadmap)** | Maxime Labonne (GitHub) | Comprehensive path: Fundamentals → LLM Scientist → LLM Engineer; includes Colab notebooks | [github.com/mlabonne/llm-course](https://github.com/mlabonne/llm-course) |
| **Hugging Face LLM Course** | Hugging Face | Hands-on with Transformers library, fine-tuning, sharing models on the Hub | [huggingface.co/learn/llm-course](https://huggingface.co/learn/llm-course/en/chapter1/1) |
| **Generative AI for Beginners** | Microsoft (GitHub) | 21-lesson course covering prompt engineering, responsible AI, chatbot building | [github.com/microsoft/generative-ai-for-beginners](https://github.com/microsoft/generative-ai-for-beginners) |
| **LLM University (LLMU)** | Cohere | NLP basics → prompt engineering → fine-tuning → RAG; modular, skip what you know | [cohere.com/llmu](https://cohere.com/llmu) |
| **Full Stack LLM Bootcamp** | The Full Stack | Production-focused: prompt engineering, UX design, deployment best practices | [fullstackdeeplearning.com](https://fullstackdeeplearning.com/) |
| **Open Source LLMOps Solutions** | Duke University (Coursera) | Deploying open-source LLMs, transformer architectures, code-first approach | [coursera.org](https://www.coursera.org/learn/open-source-llmops-solutions) |

### Curated Lists (Meta-Resources)

- **Awesome LLM Courses** — a community-curated GitHub list of online LLM courses: [github.com/wikit-ai/awesome-llm-courses](https://github.com/wikit-ai/awesome-llm-courses)
- **Awesome-LLM** — papers, frameworks, and resources in one repo: [github.com/Hannibal046/Awesome-LLM](https://github.com/Hannibal046/Awesome-LLM)

---

## Part 2: LLM Auto-Evaluation Frameworks (The Career Focus)

### Why This Matters

As LLM applications scale into production, companies need reliable ways to measure quality automatically. The "LLM-as-a-Judge" paradigm — using one LLM to evaluate another's output — is rapidly becoming an industry standard. Mastering evaluation frameworks is a high-demand, career-differentiating skill.

### Key Open-Source Evaluation Frameworks

#### Tier 1: Start Here (Most Beginner-Friendly)

| Framework | What It Does | Why Start Here | Link |
|-----------|-------------|----------------|------|
| **DeepEval** | Pytest-like unit testing for LLM apps; supports G-Eval, hallucination detection, answer relevancy | Familiar testing paradigm, great docs, runs locally | [github.com/confident-ai/deepeval](https://github.com/confident-ai/deepeval) |
| **RAGAS** | Evaluation suite specifically for RAG pipelines | RAG is everywhere; this is the go-to tool for it | [github.com/explodinggradients/ragas](https://github.com/explodinggradients/ragas) |
| **OpenAI Evals** | Evaluation framework + benchmark registry by OpenAI | Well-documented, large community, write custom evals | [github.com/openai/evals](https://github.com/openai/evals) |

#### Tier 2: Production & Observability

| Framework | What It Does | Link |
|-----------|-------------|------|
| **Langfuse** | Open-source LLM engineering platform: tracing, evaluation, prompt management, A/B testing | [github.com/langfuse/langfuse](https://github.com/langfuse/langfuse) |
| **Opik (by Comet)** | End-to-end LLM testing: trace logging, LLM-judge metrics, CI/CD integration | [github.com/comet-ml/opik](https://github.com/comet-ml/opik) |
| **Arize Phoenix** | Open-source LLM observability: trace analysis, custom evaluators, prompt versioning | [github.com/Arize-ai/phoenix](https://github.com/Arize-ai/phoenix) |
| **Evidently AI** | LLM-as-a-judge with custom prompts, visual reports, test suites, monitoring dashboards | [github.com/evidentlyai/evidently](https://github.com/evidentlyai/evidently) |

#### Tier 3: Research & Benchmarking

| Framework | What It Does | Link |
|-----------|-------------|------|
| **EleutherAI lm-evaluation-harness** | 60+ standard benchmarks (MMLU, HellaSwag, Big-Bench); powers the HF Open LLM Leaderboard | [github.com/EleutherAI/lm-evaluation-harness](https://github.com/EleutherAI/lm-evaluation-harness) |
| **lmms-eval** | Multimodal evaluation across text, image, video, audio; 50+ benchmarks | [github.com/EvolvingLMMs-Lab/lmms-eval](https://github.com/EvolvingLMMs-Lab/lmms-eval) |
| **Inspect AI** | Research-grade LLM evaluation framework | [github.com/UKGovernmentBEIS/inspect_ai](https://github.com/UKGovernmentBEIS/inspect_ai) |

---

## Part 3: LLM-as-a-Judge — Deep Dive

This is the core technique behind most auto-evaluation. Learn it well.

### Tutorials & Guides (Ordered by Difficulty)

1. **Hugging Face Cookbook: LLM-as-a-Judge** — Hands-on tutorial with code
   [huggingface.co/learn/cookbook/en/llm_judge](https://huggingface.co/learn/cookbook/en/llm_judge)

2. **Evidently AI: LLM-as-a-Judge Complete Guide** — Conceptual overview with practical steps
   [evidentlyai.com/llm-guide/llm-as-a-judge](https://www.evidentlyai.com/llm-guide/llm-as-a-judge)

3. **Evidently AI: LLM-as-a-Judge Tutorial** — "Wrong but useful" practical walkthrough
   [evidentlyai.com/blog/llm-as-a-judge-tutorial](https://www.evidentlyai.com/blog/llm-as-a-judge-tutorial)

4. **Confident AI: LLM-as-a-Judge Explained** — How to run evals at scale
   [confident-ai.com/blog/why-llm-as-a-judge-is-the-best-llm-evaluation-method](https://www.confident-ai.com/blog/why-llm-as-a-judge-is-the-best-llm-evaluation-method)

5. **Towards Data Science: LLM-as-a-Judge Practical Guide** — In-depth article
   [towardsdatascience.com/llm-as-a-judge-a-practical-guide](https://towardsdatascience.com/llm-as-a-judge-a-practical-guide/)

### Research Papers & Repos

- **Awesome-LLM-as-a-Judge** — curated list of papers: [github.com/llm-as-a-judge/Awesome-LLM-as-a-judge](https://github.com/llm-as-a-judge/Awesome-LLM-as-a-judge)
- **JudgeLM** (ICLR 2025 Spotlight) — fine-tuning LLMs as scalable judges: [github.com/baaivision/JudgeLM](https://github.com/baaivision/JudgeLM)
- **judges** — a small, practical library of LLM judges: [github.com/quotient-ai/judges](https://github.com/quotient-ai/judges)

### Evaluation-Specific Course

- **Evidently AI: LLM Evaluation for AI Builders** — Free, ~3 hours, no coding required, covers core evaluation and observability concepts
  [evidentlyai.com/blog/llm-genai-courses](https://www.evidentlyai.com/blog/llm-genai-courses)

---

## Part 4: Suggested Learning Path

A recommended order for a beginner who wants to specialize in LLM evaluation:

### Phase 1: Foundations (Weeks 1–4)
- Complete the **Hugging Face LLM Course** (Chapters 1–4) for hands-on transformer basics
- Watch **Stanford CME 295** lectures and review the cheatsheet
- Browse **Maxime Labonne's LLM Course** "Fundamentals" section

### Phase 2: Build & Fine-Tune (Weeks 5–8)
- Work through **Microsoft's Generative AI for Beginners** (21 lessons)
- Start the "LLM Scientist" section of **Labonne's course** (fine-tuning, RLHF)
- Explore **Cohere's LLMU** for RAG concepts

### Phase 3: Evaluation Deep Dive (Weeks 9–12)
- Take the **Evidently AI: LLM Evaluation for AI Builders** course
- Work through the **Hugging Face LLM-as-a-Judge cookbook**
- Set up and experiment with **DeepEval** on a small project
- Read the **Awesome-LLM-as-a-Judge** paper list (start with JudgeLM)

### Phase 4: Production Skills (Weeks 13–16)
- Deploy a RAG pipeline and evaluate it with **RAGAS**
- Set up **Langfuse** or **Arize Phoenix** for tracing and monitoring
- Run benchmarks using **EleutherAI's lm-evaluation-harness**
- Build a portfolio project: an end-to-end LLM app with automated evaluation

---

## Part 5: Career Tips

**Job titles to look for:** LLM Evaluation Engineer, AI Quality Engineer, ML Evaluation Specialist, LLM Engineer, AI/ML Platform Engineer

**Key skills employers want:** Python proficiency, understanding of transformer architectures, experience with evaluation metrics (BLEU, ROUGE, G-Eval, human correlation), familiarity with RAG patterns, prompt engineering, and production LLM observability tools.

**How to stand out:** Build a public portfolio on GitHub showing evaluation pipelines you've built. Contribute to open-source evaluation frameworks like DeepEval, RAGAS, or lm-evaluation-harness. Write about your evaluation experiments on a blog or in community forums.

---

*Compiled on March 15, 2026. Links and course availability may change — always check the source for the latest information.*
