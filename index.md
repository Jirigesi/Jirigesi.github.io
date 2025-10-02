---
layout: home2
description: "Jiri Gesi"
tags: [Jekyll, theme, responsive, blog, template]
---

I’m an **Applied Scientist at Amazon Store Foundation AI**, focusing on **post-training large language models (LLMs)** for shopping applications and agents.  
Our post-trained LLMs power variety of Amazon shopping applications such as personalization support, product rerank, and related LLM-powered experiences.

My research interest centers on machine learning—especially **post-training for LLMs**. Key areas of interest:

- **(1) LLM Reasoning.** Enabling LLMs to reason with **verifiable rewards**. Within Amazon, we’ve shown that post-training can instill reasoning—e.g., teaching models to internalize **chain-of-thought** via SFT, then pushing further with RL methods like **GRPO/GSPO** across diverse tasks. I also collaborate on **formal mathematical reasoning** (e.g., with Yong Lin and Chi Jin from Princeton University), leveraging formal methods (LEAN) to reason in formal languages—culminating in the SOTA open-source theorem-proving model **Gödel-Prover V2**.

- **(2) LLM SFT (Supervised Fine-Tuning).** I view SFT is the **cornerstone** of reasoning: high-quality chain-of-thought data first teaches models to follow instructions and to solve varied tasks reliably. At Amazon, we curate CoT datasets across tasks to build solid reasoning foundations. We’ve also explored techniques to **mitigate catastrophic forgetting**—see our study **“SFT Doesn’t Always Hurt General Capabilities.”**

- **(3) LLM Agents.** The north star is **building practical agents**. To better simulate real human shopping behavior, we built **OPeRA**, a dataset of real shopping trajectories covering **Observation, Persona, Rationale, and Action**. We develop agents like **Shop-R1** (two-stage: rationale → action with distinct rewards) and **VLM shopping Agents** variant, and we build **multi-agent** evaluators to assess agent systems more robustly.

Beyond LLM post-training, we have successfully pre-trained a set of high-quality sub-10B models, leveraging scaling laws to set hyperparameters (e.g., batch size, learning rate), optimizing compute budgets, and curating high-signal data mixtures. Before Amazon, I obtained my Ph.D. at UC Irvine with Prof. Iftekhar Ahmed, working at the intersection of software engineering and ML—an area advanced by studies like SWE-Bench, SWE-Agent.


## 📑 Selected Studies

### Gödel-Prover-V2: Scaling Formal Theorem Proving with Scaffolded Data Synthesis and Self-Correction
[arXiv](https://arxiv.org/abs/2508.03613)

**Authors:** Yong Lin, Shange Tang, Bohan Lyu, Ziran Yang, Jui-Hui Chung, Haoyu Zhao, Lai Jiang, Yihan Geng, Jiawei Ge, Jingruo Sun, Jiayun Wu, **Jiri Gesi**, Ximing Lu, David Acuna, Kaiyu Yang, Hongzhou Lin, Yejin Choi, Danqi Chen, Sanjeev Arora, Chi Jin. :contentReference[oaicite:0]{index=0}

Introduces a family of theorem-proving LLMs that combine **scaffolded data synthesis**, **verifier-guided self-correction (Lean feedback)**, and **model averaging**. The 8B model hits **84.6% pass@32 on MiniF2F**, and the 32B model reaches **88.1% (90.4% with self-correction)**; it also tops **PutnamBench** among open-source models while being far smaller than prior SOTA.

---

### Shop-R1: Rewarding LLMs to Simulate Human Behavior in Online Shopping via Reinforcement Learning
[arXiv](https://arxiv.org/abs/2507.17842)

**Authors:** Yimeng Zhang, Tian Wang, **Jiri Gesi**, Ziyi Wang, Yuxuan Lu, Jiacheng Lin, Sinong Zhan, Vianne Gao, Ruochen Jiao, Junze Liu, Kun Qian, Yuxin Tang, Ran Xue, Houyu Zhang, Qingjun Cui, Yufan Guo, Dakuo Wang. :contentReference[oaicite:1]{index=1}

Frames shopper simulation as **two-stage RL**: first generate **rationales**, then **predict actions**, each with tailored rewards. Improves realism and controllability of shopping-behavior simulation vs. pure task-completion baselines; supports downstream evaluation and policy analysis.

---

### OPeRA: A Dataset of Observation, Persona, Rationale, and Action for Evaluating LLMs on Human Online Shopping Behavior Simulation
[arXiv](https://arxiv.org/abs/2506.05606)

**Authors:** Ziyi Wang, Yuxuan Lu, Wenbo Li, Amirali Amini, Bo Sun, Yakov Bart, Weimin Lyu, **Jiri Gesi**, Tian Wang, Jing Huang, Yu Su, Upol Ehsan, Malihe Alikhani, Toby Jia-Jun Li, Lydia Chilton, Dakuo Wang. :contentReference[oaicite:2]{index=2}

Releases **OPeRA**, the first public dataset pairing **user personas**, **browser observations**, **fine-grained web actions**, and **just-in-time rationales** from real shopping sessions. Establishes **benchmarks** for predicting next actions/rationales and evaluating “digital-twin” agents.

---

### SFT Doesn’t Always Hurt General Capabilities: Revisiting Domain-Specific Fine-Tuning in LLMs
[arXiv](https://arxiv.org/abs/2509.20758)

**Authors:** Jiacheng Lin, Zhongruo Wang, Kun Qian, Tian Wang, Arvind Srinivasan, Hansi Zeng, Ruochen Jiao, Xie Zhou, **Jiri Gesi**, Dakuo Wang, Yufan Guo, Kai Zhong, Weiqi Zhang, Sujay Sanghavi, Changyou Chen, Hyokun Yun, Lihong Li. :contentReference[oaicite:3]{index=3}

Re-examines the belief that domain SFT ruins general abilities. Finds that **smaller learning rates** largely **mitigate general-capability degradation** while keeping domain performance; introduces **TALR (Token-Adaptive Loss Reweighting)** to further improve the balance. Provides theory (token-tree/code-length view) + practical guidelines.

---

### LLM Agent Meets Agentic AI: Can LLM Agents Simulate Customers to Evaluate Agentic-AI-Based Shopping Assistants?
[arXiv](https://arxiv.org/abs/2509.21501)

**Authors:** Lu Sun, Shihan Fu, Bingsheng Yao, Yuxuan Lu, Wenbo Li, Hansu Gu, **Jiri Gesi**, Jing Huang, Chen Luo, Dakuo Wang. :contentReference[oaicite:4]{index=4}

First **large-scale human study** (multi-turn with an agentic shopping assistant) plus a **persona-grounded “digital twin” simulation** where LLM agents replay user behaviors for apples-to-apples evaluation. Shows the agentic simulation can mirror real-world task outcomes and UX dimensions, enabling faster/cheaper iteration on shopping assistants.

---

### Multi-Agent-as-Judge: Aligning LLM-Agent-Based Automated Evaluation with Multi-Dimensional Human Evaluation
[arXiv](https://arxiv.org/abs/2507.21028)

**Authors:** Jiaju Chen, Yuxuan Lu, Xiaojie Wang, Huimin Zeng, Jing Huang, **Jiri Gesi**, Ying Xu, Bingsheng Yao, Dakuo Wang. :contentReference[oaicite:5]{index=5}

Proposes **MAJ-Eval**, which automatically builds **multi-persona** evaluator agents from source docs and runs **in-group debates** to produce multi-dimensional feedback. Achieves **closer alignment to expert ratings** vs. common automated metrics and prior LLM-as-Judge setups in education and medical domains.

---

### UXAgent: An LLM Agent-Based Usability Testing Framework for Web Des



---

## Community Service  

**Conference Reviews (ML):** EMNLP 2025, 2024; ICML 2025, 2024; NeurIPS 2025, 2024, 2023; ICLR 2025, 2024; TIST 2024; WWW 2024. SIGIR: 2024 
**Conference Reviews (Software Engineering):** TOSEM 2025, 2024, 2023; MSR 2024, 2023; ASE 2024, 2023; SEA4DQ 2024; ESE 2021.  
**Program Committee / Organizing Roles:** PROMISE 2025; ASE 2024; MSR 2024; SEA4DQ 2024; AIware 2024.
 

---
