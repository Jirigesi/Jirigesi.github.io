---
layout: home2
description: "Jiri Gesi"
tags: [Jekyll, theme, responsive, blog, template]
---

I’m an **Applied Scientist at Amazon Store Foundation AI**, focusing on **post-training large language models (LLMs)** for shopping applications and agents. Our post-trained LLMs have been deployed to power a variety of Amazon shopping applications such as personalization support, product re-ranking, and related LLM-powered experiences.

My research interest centers on machine learning—especially **post-training for LLMs**. Key areas of interest:

- **(1) LLM Reasoning.** Enabling LLMs to reason with **"verifiable" rewards**. Within Amazon, we’ve shown that post-training can instill reasoning—e.g., teaching models to internalize **chain-of-thought** via SFT, then pushing further with RL methods like **GRPO/GSPO** across diverse tasks. I also collaborate on **formal mathematical reasoning** (with Yong Lin and Prof. Chi Jin from Princeton University), leveraging formal methods (LEAN) to reason in formal languages—culminating in the SOTA open-source theorem-proving model **Gödel-Prover V2**.

- **(2) LLM SFT (Supervised Fine-Tuning).** I view SFT as the **cornerstone** of reasoning: high-quality chain-of-thought data first teaches models to follow instructions and to solve varied tasks reliably. At Amazon, we curate CoT datasets across tasks to build solid reasoning foundations. We’ve also explored techniques to **mitigate catastrophic forgetting**—see our study **“SFT Doesn’t Always Hurt General Capabilities.”**

- **(3) LLM Agents.** The north star is **building practical agents**. To better simulate real human shopping behavior, we built **OPeRA**, a dataset of real shopping trajectories covering **Observation, Persona, Rationale, and Action**. We develop agents like **Shop-R1** and **VLM shopping agents**, and we build **multi-agent** evaluators to assess agent systems more robustly.

Beyond LLM post-training, we have successfully pre-trained a set of high-quality sub-10B models, leveraging scaling laws to set hyperparameters (e.g., batch size, learning rate), optimizing compute budgets, and curating high-signal data mixtures. Before Amazon, I obtained my Ph.D. at UC Irvine with Prof. Iftekhar Ahmed, working at the intersection of software engineering and ML—an area advanced by studies like SWE-Bench and SWE-Agent.


## 📝 Selected Papers

### 🔹 LLM Reasoning & Training

[**Gödel-Prover-V2: Scaling Formal Theorem Proving with Scaffolded Data Synthesis and Self-Correction**](https://arxiv.org/abs/2508.03613)  
*Authors:* Yong Lin, Shange Tang, Bohan Lyu, Ziran Yang, Jui-Hui Chung, Haoyu Zhao, Lai Jiang, Yihan Geng, Jiawei Ge, Jingruo Sun, Jiayun Wu, **Jiri Gesi**, Ximing Lu, David Acuna, Kaiyu Yang, Hongzhou Lin, Yejin Choi, Danqi Chen, Sanjeev Arora, Chi Jin  
**Summary:** Introduces a theorem-proving LLM stack combining scaffolded data synthesis, verifier-guided self-correction, and model averaging. Achieves strong MiniF2F and PutnamBench results while remaining much smaller than prior SOTA.

---

[**SFT Doesn’t Always Hurt General Capabilities: Revisiting Domain-Specific Fine-Tuning in LLMs**](https://arxiv.org/abs/2509.20758)  
*Authors:* Jiacheng Lin, Zhongruo Wang, Kun Qian, Tian Wang, Arvind Srinivasan, Hansi Zeng, Ruochen Jiao, Xie Zhou, **Jiri Gesi**, Dakuo Wang, Yufan Guo, Kai Zhong, Weiqi Zhang, Sujay Sanghavi, Changyou Chen, Hyokun Yun, Lihong Li  
**Summary:** Re-examines the “SFT hurts generality” assumption. Shows small learning rates largely mitigate degradation while preserving target-domain gains; introduces **TALR** (Token-Adaptive Loss Reweighting) to further improve the trade-off.

---

[**Beyond Self-Learned Attention: Mitigating Attention Bias in Transformer-Based Models Using Attention Guidance**](https://arxiv.org/abs/2402.16790)  
*Authors:* **Jiri Gesi**, Iftekhar Ahmed  
**Summary:** Introduces **SyntaGuid**, which guides attention toward syntax/AST signals to counter bias toward special tokens. Improves multiple software-engineering LLM tasks without extra data, correcting a notable share of prior errors.

---

### 🔹 LLM Agents & Simulation

[**Shop-R1: Rewarding LLMs to Simulate Human Behavior in Online Shopping via Reinforcement Learning**](https://arxiv.org/abs/2507.17842)  
*Authors:* Yimeng Zhang, Tian Wang, **Jiri Gesi**, Ziyi Wang, Yuxuan Lu, Jiacheng Lin, Sinong Zhan, Vianne Gao, Ruochen Jiao, Junze Liu, Kun Qian, Yuxin Tang, Ran Xue, Houyu Zhang, Qingjun Cui, Yufan Guo, Dakuo Wang  
**Summary:** Frames shopper simulation as two-stage RL—first generate rationales, then predict actions—with tailored rewards. Improves realism and controllability versus task-completion baselines and enables downstream evaluation/policy analysis.

---

[**OPeRA: A Dataset of Observation, Persona, Rationale, and Action for Evaluating LLMs on Human Online Shopping Behavior Simulation**](https://arxiv.org/abs/2506.05606)  
*Authors:* Ziyi Wang, Yuxuan Lu, Wenbo Li, Amirali Amini, Bo Sun, Yakov Bart, Weimin Lyu, **Jiri Gesi**, Tian Wang, Jing Huang, Yu Su, Upol Ehsan, Malihe Alikhani, Toby Jia-Jun Li, Lydia Chilton, Dakuo Wang  
**Summary:** A public dataset pairing user personas, browser observations, fine-grained web actions, and just-in-time rationales. Establishes benchmarks for next-action/rationale prediction and digital-twin evaluation.

---

[**Prompting is Not All You Need! Evaluating LLM Agent Simulation Methodologies with Real-World Online Customer Behavior Data**](https://arxiv.org/abs/2503.20749)  
*Authors:* Yuxuan Lu, Jing Huang, Yan Han, Bingsheng Yao, Sisong Bei, **Jiri Gesi**, Yaochen Xie, Qi He, Dakuo Wang  
**Summary:** Evaluates LLMs on web action generation using real shopping behavior data. Shows fine-tuning with real trajectories significantly outperforms prompting alone, and adding synthesized reasoning traces further improves accuracy.

---

[**LLM Agent Meets Agentic AI: Can LLM Agents Simulate Customers to Evaluate Agentic-AI-Based Shopping Assistants?**](https://arxiv.org/abs/2509.21501)  
*Authors:* Lu Sun, Shihan Fu, Bingsheng Yao, Yuxuan Lu, Wenbo Li, Hansu Gu, **Jiri Gesi**, Jing Huang, Chen Luo, Dakuo Wang  
**Summary:** Combines a large-scale human study with persona-grounded “digital-twin” simulation. Shows simulations can mirror real-world task outcomes and UX dimensions, enabling faster and cheaper iteration on shopping assistants.

---

[**Multi-Agent-as-Judge: Aligning LLM-Agent-Based Automated Evaluation with Multi-Dimensional Human Evaluation**](https://arxiv.org/abs/2507.21028)  
*Authors:* Jiaju Chen, Yuxuan Lu, Xiaojie Wang, Huimin Zeng, Jing Huang, **Jiri Gesi**, Ying Xu, Bingsheng Yao, Dakuo Wang  
**Summary:** Proposes **MAJ-Eval**—multi-persona evaluator agents that debate and aggregate judgments. Produces evaluations more aligned with expert ratings than typical automatic metrics in domains like education and medicine.

---

[**UXAgent: A System for Simulating Usability Testing of Web Design with LLM Agents**](https://arxiv.org/abs/2504.09407)  
*Authors:* Yuxuan Lu, Bingsheng Yao, Hansu Gu, Jing Huang, Jessie Wang, Yang Li, **Jiri Gesi**, Qi He, Toby Jia-Jun Li, Dakuo Wang  
**Summary:** A practical framework to simulate UX studies before recruiting participants. Generates personas and browsing agents, logs quantitative traces/interviews, and provides replays to help teams iterate rapidly on study design.


---

## 🌐 Community Service  

**Conference Reviews (ML):** EMNLP 2025, 2024; ICML 2025, 2024; NeurIPS 2025, 2024, 2023; ICLR 2025, 2024; TIST 2024; WWW 2024; SIGIR 2024.  
**Conference Reviews (Software Engineering):** TOSEM 2025, 2024, 2023; MSR 2024, 2023; ASE 2024, 2023; SEA4DQ 2024; ESE 2021.  
**Program Committee / Organizing Roles:** PROMISE 2025; ASE 2024; MSR 2024; SEA4DQ 2024; AIware 2024.
