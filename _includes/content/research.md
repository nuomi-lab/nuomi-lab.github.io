# **Research**

We combine technical research on ML methodology and AI systems design with human-centred evaluation, so that the AI systems we develop are judged by whether they help real people make better decisions, not only by benchmark performance.

1. **Making Values Explicit:** We develop ML frameworks for specifying what a "good" AI model means in human contexts, including fairness, accountability, and trade-offs between the goals of different stakeholders (quantified as training objectives and metrics). We build and train AI models that optimise for capturing human values.

2. **Models People Can Understand and Question:** We develop ML methods for interpreting complex AI models and for estimating and communicating uncertainty in the outputs and the internal reasoning of these models, so that users can tell when a model's output should, and should not, be relied on.

3. **Evaluating AI With Its Users:** We rigorously study how people actually use AI systems in high-stakes settings (e.g. disease diagnosis, mental health support), and use what we learn to rework how those systems are designed, evaluated, and deployed.

## Technical Research Themes
{: .text-center}

The themes below come from prior work by our PI, Weiwei Pan, and collaborators. For each, we describe the main machine learning approach and the central insight behind it, with a few papers as examples.

- **Behaviourally grounded reinforcement learning:** We model the people an AI system assists as reinforcement learning agents, with interpretable parameters for human traits (such as how much they discount the future, or how costly they find effort), and frame AI assistance as an intervention on those parameters. Inverse reinforcement learning lets us infer these traits from behaviour.
  - *Key insight:* Helping someone does not require a complete model of human cognition, only a minimal, task-specific model of the few traits that drive their behaviour on the task at hand.
  - *Example work:* [Nofshin et al., 2024](https://arxiv.org/abs/2401.14923); [Moore et al., 2025](https://rlj.cs.umass.edu/2025/papers/Paper59.html); [Yao et al., 2024](https://arxiv.org/abs/2409.18051).

- **Sequential decision-making under real-world constraints:** We develop bandit and reinforcement learning methods for high-stakes settings such as healthcare, where an algorithm must personalise while also producing valid scientific evidence, acting safely, and learning from scarce and uneven data.
  - *Key insight:* Standard algorithmic choices carry hidden assumptions that break under deployment conditions. Building the real constraints into the learning problem itself, rather than handling them afterwards, yields methods whose guarantees hold where they matter.
  - *Example work:* [Yao et al., 2021](https://arxiv.org/abs/2004.06230); [Rathnam et al., 2023](https://arxiv.org/abs/2306.11208); [Brown et al., 2025](https://pmc.ncbi.nlm.nih.gov/articles/PMC12099420/).

- **Interpretable machine learning:** We treat explanations as measurement instruments. The properties an explanation should have (such as faithfulness, robustness, and simplicity) are formally defined, quantitatively validated, and directly optimised, rather than encouraged by heuristics.
  - *Key insight:* An explanation is useful only if we know which property of the model it measures, and how reliably. Different tasks need different properties, so explanation design is a multi-objective problem with task-dependent trade-offs.
  - *Example work:* [Chen et al., 2022](https://arxiv.org/abs/2211.05667); [Mahinpei et al., 2021](https://arxiv.org/abs/2106.13314); [Tadesse et al., 2025](https://arxiv.org/abs/2410.23880); [Nofshin et al., 2024](https://arxiv.org/abs/2406.00116).

- **Bayesian deep learning and approximate inference:** We study probabilistic models such as Bayesian neural networks and deep latent-variable models, combining theoretical analysis with controlled experiments to characterise when approximate inference methods (such as variational inference) yield reliable uncertainty.
  - *Key insight:* Approximate inference can fail silently, producing uncertainty that looks reasonable on standard metrics but does not reflect the data. These failures often have structural causes, such as non-identifiability or the inference objective itself, that can be diagnosed and corrected.
  - *Example work:* [Yao et al., 2019](https://arxiv.org/abs/1906.09686); [Coker et al., 2022](https://arxiv.org/abs/2106.07052); [Yacoby et al., 2022](https://arxiv.org/abs/1911.00569).

- **Representation learning and model steering:** We design models whose internal structure supports targeted intervention, such as latent-variable models with interpretable factors and ensembles with deliberately diverse members, and develop methods for analysing and steering the internal representations of large language models.
  - *Key insight:* When representations are entangled, an intervention aimed at one behaviour can change many others. Control methods must therefore be evaluated for fidelity (whether they change only what was intended), not just for aggregate success.
  - *Example work:* [Ross et al., 2020](https://arxiv.org/abs/1911.01291); [Subhash et al., 2023](https://arxiv.org/abs/2309.00254); [Raedler et al., 2025](https://icml.cc/virtual/2025/50956).

- **Evaluation and auditing of generative models:** We evaluate generative models through the distribution of their outputs across prompts, tasks, and populations, described in human-interpretable concepts, and draw on measurement theory from the social sciences to design probes.
  - *Key insight:* Properties such as bias are not fixed attributes that a single benchmark can certify; they shift with the task and the prompt. Evaluation must be task-specific and grounded in a theory of when a measurement generalises to real use.
  - *Example work:* [Boussard et al., 2024](https://neurips.cc/virtual/2024/103333); [Abdel Magid et al., 2025](https://arxiv.org/abs/2410.04634); [Morehouse et al., 2025](https://arxiv.org/abs/2503.00093).

## Designing With Communities
{: .text-center}

Our HCI research embeds us in communities of practice over sustained collaborations. Through interviews, iterative co-design, and user studies, we learn how practitioners work, what expertise they bring, and what success means to them, and then design AI tools around those needs. We also teach workshops on AI fundamentals, so that practitioners can take part as informed co-designers and judge AI tools for themselves.

- *Key insight:* Community needs often redefine the technical problem itself. Humanitarian frontline negotiators did not want AI that tells them what to do; they wanted support for analysing context, exploring alternatives, and assessing risks. That shifted the design goal from replacing expert judgement to strengthening it.
- *Example work:* [Ma et al., 2025](https://arxiv.org/abs/2410.09139), "ChatGPT, Don't Tell Me What to Do": Designing AI for Context Analysis in Humanitarian Frontline Negotiations.
