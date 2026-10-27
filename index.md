---
layout: profile
role: Co-founder, Voltspan AI
tagline: Built AI agents at Microsoft and Amazon. Now building the GPU clusters that train them.
description: "Jiri Gesi, co-founder of Voltspan AI. Builds AI agents: previously Today in Microsoft 365 Copilot and Rufus, Amazon's AI shopping agent."
previously: "[Microsoft Copilot Today](https://blogs.microsoft.com/blog/2026/09/25/introducing-the-new-copilot-with-home-code-and-autopilot/) · [Amazon Rufus](https://www.aboutamazon.com/news/retail/amazon-rufus) · Ph.D. UC Irvine"
experience:
  - org: Voltspan AI
    url: https://voltspan.ai
    when: Now
    role: Co-founder
    note: We build and run NVIDIA GPU clusters as the foundation for agent model training and agent clouds.
  - org: Microsoft
    role: Senior Researcher, Microsoft 365 Copilot
    note: "Built [Today](https://blogs.microsoft.com/blog/2026/09/25/introducing-the-new-copilot-with-home-code-and-autopilot/) on the Copilot science team: an agentic command center across email, calendar, Teams and tasks that drafts replies, proposes schedule changes and lines up follow-ups. Featured in Satya Nadella's new Copilot launch. [Watch the preview](https://www.youtube.com/watch?v=Jv-iQSZ3YVY)."
  - org: Amazon
    role: Applied Scientist, Store Foundation AI
    note: "Core member of the team that built [Rufus](https://www.aboutamazon.com/news/retail/amazon-rufus), Amazon's AI shopping agent, from scratch: training the model, deploying it at Amazon scale, and building the product end to end. Rufus is now [Alexa for Shopping](https://www.aboutamazon.com/news/retail/alexa-for-shopping-ai-assistant)."
  - org: UC Irvine
    role: Ph.D., Computer Science
    note: Software engineering and machine learning, with Prof. Iftekhar Ahmed.
links:
  - title: voltspan.ai
    url: https://voltspan.ai
  - title: LinkedIn
    url: https://www.linkedin.com/in/jirigesi
  - title: Google Scholar
    url: https://scholar.google.com/citations?user=pZTCjMsAAAAJ
service:
  - label: Reviewer (ML)
    text: EMNLP 2025, 2024; ICML 2025, 2024; NeurIPS 2025, 2024, 2023; ICLR 2025, 2024; TIST 2024; WWW 2024; SIGIR 2024.
  - label: Reviewer (Software Engineering)
    text: TOSEM 2025, 2024, 2023; MSR 2024, 2023; ASE 2024, 2023; SEA4DQ 2024; ESE 2021.
  - label: Program Committee / Organizing
    text: PROMISE 2025; ASE 2024; MSR 2024; SEA4DQ 2024; AIware 2024.
---

<section id="research" class="reveal" markdown="1">
## Research

My research centers on **post-training for LLMs**.

<div class="areas">
<div class="area" markdown="1">
<span class="glass-icon tint-blue" aria-hidden="true"><svg viewBox="0 0 24 24"><circle cx="6" cy="6" r="2.2"/><circle cx="18" cy="6" r="2.2"/><circle cx="12" cy="18" r="2.2"/><path d="M7.6 7.6 10.6 16M16.4 7.6 13.4 16M8.2 6h7.6"/></svg></span>

#### LLM Reasoning
Teaching LLMs to reason with **verifiable rewards**: chain-of-thought via SFT, then RL with **GRPO/GSPO**. Formal math in LEAN with Yong Lin and Prof. Chi Jin (Princeton) led to **Gödel-Prover-V2**, an open-source SOTA theorem prover featured on [Thinking Machines’ Tinker](https://thinkingmachines.ai/tinker/).
</div>
<div class="area" markdown="1">
<span class="glass-icon tint-volt" aria-hidden="true"><svg viewBox="0 0 24 24"><path d="M5 7h14M5 12h14M5 17h14"/><circle cx="9" cy="7" r="2"/><circle cx="15" cy="12" r="2"/><circle cx="11" cy="17" r="2"/></svg></span>

#### Supervised Fine-Tuning
High-quality chain-of-thought data is the **cornerstone** of reasoning. We also study how to **avoid catastrophic forgetting** when fine-tuning for a domain.
</div>
<div class="area" markdown="1">
<span class="glass-icon tint-violet" aria-hidden="true"><svg viewBox="0 0 24 24"><rect x="5" y="8" width="14" height="11" rx="3"/><path d="M12 4v4M9 13h.01M15 13h.01"/><circle cx="12" cy="3.5" r="1"/></svg></span>

#### LLM Agents
Building **practical agents**: the **OPeRA** shopping-behavior dataset, **Shop-R1** and VLM shopping agents, and **multi-agent** evaluators for agent systems.
</div>
</div>
</section>
