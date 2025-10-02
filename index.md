---
layout: home2
description: "Jiri Gesi"
tags: [Jekyll, theme, responsive, blog, template]
---

<span style="color: orange; font-weight: bold;">
We are hiring Applied Scientist Interns and full-time positions!  
Contact me if you're interested in working on LLMs for retrieval & ranking.
</span>

---

## 👋 About Me  

I’m currently an **Applied Scientist at Amazon Store Foundation AI**, where I focus on **post-training large language models (LLMs)** for shopping applications and agents.  
Our post-trained LLMs have been successfully launched in Amazon experiences such as **Rufus, Personalization, and Search**.  

Outside of work, I enjoy traveling, music festivals, saying “Yes!”, coding, and reading research papers.  

---

## 📑 Selected Papers  

## 📑 Selected Papers

### Goedel-Prover-V2: Scaling Formal Theorem Proving with Scaffolded Data Synthesis and Self-Correction
[arXiv](https://arxiv.org/abs/2508.03613) • [Code & models](https://github.com/Goedel-LM/Goedel-Prover-V2)

![Goedel-Prover-V2 — recommended: first-page figure with pipeline overview](/assets/papers/goedel-prover-v2.png)

**One-paragraph summary.** Introduces a family of theorem-proving LLMs that combine **scaffolded data synthesis**, **verifier-guided self-correction (Lean feedback)**, and **model averaging**. The 8B model hits **84.6% pass@32 on MiniF2F**, and the 32B model reaches **88.1% (90.4% with self-correction)**; it also tops **PutnamBench** among open-source models while being far smaller than prior SOTA. :contentReference[oaicite:0]{index=0}

**Use this picture:** the model/pipeline diagram on the first PDF page (clean, recognizable). Save as: `/assets/papers/goedel-prover-v2.png`.

---

### LLM Agent Meets Agentic AI: Can LLM Agents Simulate Customers to Evaluate Agentic-AI-Based Shopping Assistants?
[arXiv](https://arxiv.org/abs/2509.21501)

![Agentic shopping simulation — recommended: overview figure showing human study + digital-twin agents](/assets/papers/agentic-shopping-sim.png)

**One-paragraph summary.** First **large-scale human study** (multi-turn with an agentic shopping assistant) plus a **persona-grounded “digital twin” simulation** where LLM agents replay user behaviors for apples-to-apples evaluation. Shows the agentic simulation can mirror real-world task outcomes and UX dimensions, enabling faster/cheaper iteration on shopping assistants. :contentReference[oaicite:1]{index=1}

**Use this picture:** the framework/overview figure from the HTML/PDF. Save as: `/assets/papers/agentic-shopping-sim.png`.

---

### SFT Doesn’t Always Hurt General Capabilities: Revisiting Domain-Specific Fine-Tuning in LLMs
[arXiv](https://arxiv.org/abs/2509.20758)

![SFT trade-off — recommended: Figure 1 (learning-rate vs. general capability trade-offs)](/assets/papers/sft-doesnt-always-hurt.png)

**One-paragraph summary.** Re-examines the belief that domain SFT ruins general abilities. Finds that **smaller learning rates** largely **mitigate general-capability degradation** while keeping domain performance; introduces **TALR (Token-Adaptive Loss Reweighting)** to further improve the balance. Provides theory (token-tree/code-length view) + practical guidelines. :contentReference[oaicite:2]{index=2}

**Use this picture:** Figure 1 with the Pareto trade-offs. Save as: `/assets/papers/sft-doesnt-always-hurt.png`.

---

### Multi-Agent-as-Judge: Aligning LLM-Agent-Based Automated Evaluation with Multi-Dimensional Human Evaluation
[arXiv](https://arxiv.org/abs/2507.21028)

![MAJ-Eval — recommended: system diagram showing persona mining + multi-agent debate](/assets/papers/maj-eval.png)

**One-paragraph summary.** Proposes **MAJ-Eval**, which automatically builds **multi-persona** evaluator agents from source docs and runs **in-group debates** to produce multi-dimensional feedback. Achieves **closer alignment to expert ratings** vs. common automated metrics and prior LLM-as-Judge setups in education and medical domains. :contentReference[oaicite:3]{index=3}

**Use this picture:** architecture/flow figure of MAJ-Eval. Save as: `/assets/papers/maj-eval.png`.

---

### Shop-R1: Rewarding LLMs to Simulate Human Behavior in Online Shopping via Reinforcement Learning
[arXiv](https://arxiv.org/abs/2507.17842) • [PDF](https://arxiv.org/pdf/2507.17842)

![Shop-R1 — recommended: two-stage (rationale → action) RL training graphic](/assets/papers/shop-r1.png)

**One-paragraph summary.** Frames shopper simulation as **two-stage RL**: first generate **rationales**, then **predict actions**, each with tailored rewards. Improves realism and controllability of shopping-behavior simulation vs. pure task-completion baselines; supports downstream evaluation and policy analysis. :contentReference[oaicite:4]{index=4}

**Use this picture:** pipeline figure from the PDF. Save as: `/assets/papers/shop-r1.png`.

---

### OPeRA: A Dataset of Observation, Persona, Rationale, and Action for Evaluating LLMs on Human Online Shopping Behavior Simulation
[arXiv](https://arxiv.org/abs/2506.05606) • [PDF](https://arxiv.org/pdf/2506.05606)

![OPeRA — recommended: data schema (observation/persona/rationale/action) figure](/assets/papers/opera-dataset.png)

**One-paragraph summary.** Releases **OPeRA**, the first public dataset pairing **user personas**, **browser observations**, **fine-grained web actions**, and **just-in-time rationales** from real shopping sessions. Establishes **benchmarks** for predicting next actions/rationales and evaluating “digital-twin” agents. :contentReference[oaicite:5]{index=5}

**Use this picture:** the dataset schema/collection pipeline figure. Save as: `/assets/papers/opera-dataset.png`.

---

### UXAgent: A System for Simulating Usability Testing of Web Design with LLM Agents
[arXiv](https://arxiv.org/abs/2504.09407) • [CHI EA’25 PDF (Amazon Science)](https://assets.amazon.science/ce/a8/3e0f868d478cac3d07b9ee8c2804/uxagent-an-llm-agent-based-usability-testing-framework-for-web-design.pdf)

![UXAgent — recommended: system architecture + persona generator + replay interface](/assets/papers/uxagent.png)

**One-paragraph summary.** A practical tool to **simulate UX studies** before recruiting people. Generates **personas** and **LLM agents** that browse target sites via a universal connector, logging quantitative traces, interviews, and replay videos—helping UX teams iterate on study design quickly. :contentReference[oaicite:6]{index=6}

**Use this picture:** the 3-module system diagram (Persona Generator, Agent, Browser Connector). Save as: `/assets/papers/uxagent.png`.

---

### Beyond Self-Learned Attention: Mitigating Attention Bias in Transformer-Based Models Using Attention Guidance
[arXiv](https://arxiv.org/abs/2402.16790)

![Attention Guidance — recommended: SyntaGuid overview with syntax/AST guidance arrows](/assets/papers/attention-guidance.png)

**One-paragraph summary.** Introduces **SyntaGuid**, which explicitly **guides attention** toward meaningful **syntax tokens/AST elements** to counter bias toward special tokens. Improves several software-engineering LLM tasks without extra data, fixing a sizable portion of prior mistakes. :contentReference[oaicite:7]{index=7}

**Use this picture:** conceptual figure illustrating syntax-guided attention. Save as: `/assets/papers/attention-guidance.png`.


---

## 🎓 Research Community Service  

**Conference Reviews (ML):**  
- EMNLP 2025  
- ICML 2025  
- NeurIPS 2025, 2024, 2023  
- ICLR 2024, 2025  
- TIST 2024  
- WWW 2024  

**Conference Reviews (Software Engineering):**  
- TOSEM 2025, 2024, 2023  
- MSR 2024, 2023  
- ASE 2024, 2023  
- SEA4DQ 2024  
- ESE 2021  

**Program Committee / Organizing Roles:**  
- PROMISE 2025  
- ASE 2024  
- MSR 2024  
- SEA4DQ 2024  
- AIware 2024  

---

## 🌍 Site Visitors  

This site has been visited:  

[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fjirigesi.github.io&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=Visitors&edge_flat=false)](https://hits.seeyoufarm.com)  

**Tracking daily and total visits since Feb 1, 2022.**

---
