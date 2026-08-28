# Curated Research Papers

All 21 papers below were independently verified against arXiv, publisher pages (Nature, ACM), DOI/Crossref, or Semantic Scholar as part of this repository's curation process (see the [Citation Integrity Audit](../citation-audit/) for the methodology used, which was applied to a sampled subset first and then extended to this full collection). Each entry lists authors, year, venue, a persistent identifier, and a one-line note on why it belongs in this collection.

## Table of Contents
- [Survey / Review Papers](#survey--review-papers)
- [Foundational Papers](#foundational-papers)
- [Methods / Algorithms](#methods--algorithms)
- [Applications](#applications)
- [Evaluation Methods / Benchmarks](#evaluation-methods--benchmarks)

---

## Survey / Review Papers

- **Survey of Hallucination in Natural Language Generation**
  Ji, Z., Lee, N., Frieske, R., Yu, T., Su, D., Xu, Y., Ishii, E., Bang, Y. J., Madotto, A., & Fung, P., 2023, *ACM Computing Surveys*, 55(12), Article 248.
  [DOI: 10.1145/3571730](https://doi.org/10.1145/3571730)
  Foundational, widely-cited taxonomy (intrinsic vs. extrinsic hallucination) underpinning how this repo's paper frames context-hallucination as the propagation mechanism.

- **A Survey on Hallucination in Large Language Models: Principles, Taxonomy, Challenges, and Open Questions**
  Huang, L., Yu, W., Ma, W., Zhong, W., Feng, Z., Wang, H., Chen, Q., Peng, W., Feng, X., Qin, B., & Liu, T., 2024/2025, *ACM Transactions on Information Systems*, 43(2), Article 42.
  [DOI: 10.1145/3703155](https://doi.org/10.1145/3703155)
  Updates the hallucination taxonomy specifically for LLM-era agentic and RAG pipelines, directly relevant to Section 4's error-mode discussion.

---

## Foundational Papers

- **ReAct: Synergizing Reasoning and Acting in Language Models**
  Yao, S., Zhao, J., Yu, D., Du, N., Shafran, I., Narasimhan, K., & Cao, Y., 2023, *International Conference on Learning Representations (ICLR 2023)*.
  [arXiv:2210.03629](https://arxiv.org/abs/2210.03629) · DOI: 10.48550/arXiv.2210.03629
  Founding paradigm for the "agentic loop" (reason → act → observe) that every later multi-step research agent builds on.

- **Reflexion: Language Agents with Verbal Reinforcement Learning**
  Shinn, N., Cassano, F., Gopinath, A., Narasimhan, K., & Yao, S., 2023, *Advances in Neural Information Processing Systems (NeurIPS 2023)*.
  [arXiv:2303.11366](https://arxiv.org/abs/2303.11366) · DOI: 10.48550/arXiv.2303.11366
  Introduces episodic self-reflection as a linguistic feedback loop — a key example of the "step-level self-checking" mitigation category.

- **Chain-of-Thought Prompting Elicits Reasoning in Large Language Models**
  Wei, J., Wang, X., Schuurmans, D., Bosma, M., Xia, F., Chi, E., Le, Q. V., & Zhou, D., 2022, *Advances in Neural Information Processing Systems (NeurIPS 2022)*.
  [arXiv:2201.11903](https://arxiv.org/abs/2201.11903) · DOI: 10.48550/arXiv.2201.11903
  Establishes the reasoning-trace primitive that ReAct, Reflexion, and Tree-of-Thoughts all extend into multi-step agent pipelines.

- **Toolformer: Language Models Can Teach Themselves to Use Tools**
  Schick, T., Dwivedi-Yu, J., Dessì, R., Raileanu, R., Lomeli, M., Zettlemoyer, L., Cancedda, N., & Scialom, T., 2023, *Advances in Neural Information Processing Systems (NeurIPS 2023)*.
  [arXiv:2302.04761](https://arxiv.org/abs/2302.04761) · DOI: 10.48550/arXiv.2302.04761
  Origin of self-supervised tool-invocation, the mechanism whose runtime failures drive the "Code & Tool Execution State Corruption" pathway.

- **Generative Agents: Interactive Simulacra of Human Behavior**
  Park, J. S., O'Brien, J. C., Cai, C. J., Morris, M. R., Liang, P., & Bernstein, M. S., 2023, *Proceedings of the 36th Annual ACM Symposium on User Interface Software and Technology (UIST '23)*.
  [DOI: 10.1145/3586183.3606763](https://doi.org/10.1145/3586183.3606763)
  Introduced memory-and-reflection architectures for long-horizon agents, a precursor to the working-memory/context-drift issues discussed in Section 4.4.

---

## Methods / Algorithms

- **Tree of Thoughts: Deliberate Problem Solving with Large Language Models**
  Yao, S., Yu, D., Zhao, J., Shafran, I., Griffiths, T. L., Cao, Y., & Narasimhan, K., 2023, *Advances in Neural Information Processing Systems (NeurIPS 2023)*.
  [arXiv:2305.10601](https://arxiv.org/abs/2305.10601) · DOI: 10.48550/arXiv.2305.10601
  Generalizes linear reasoning chains into search trees — the direct conceptual ancestor of the "progressive agentic tree search" mitigation covered in Section 5.3.

- **Self-Refine: Iterative Refinement with Self-Feedback**
  Madaan, A., Tandon, N., Gupta, P., Hallinan, S., Gao, L., Wiegreffe, S., Alon, U., Dziri, N., Prabhumoye, S., Yang, Y., Gupta, S., Majumder, B. P., Hermann, K., Welleck, S., Yazdanbakhsh, A., & Clark, P., 2023, *Advances in Neural Information Processing Systems (NeurIPS 2023)*.
  [arXiv:2303.17651](https://arxiv.org/abs/2303.17651) · DOI: 10.48550/arXiv.2303.17651
  Demonstrates same-model self-critique — the paper explicitly used as the "step-level self-checking" contrast case against independent cross-verification.

- **Improving Factuality and Reasoning in Language Models through Multiagent Debate**
  Du, Y., Li, S., Torralba, A., Tenenbaum, J. B., & Mordatch, I., 2023, *International Conference on Machine Learning (ICML 2024)*.
  [arXiv:2305.14325](https://arxiv.org/abs/2305.14325) · DOI: 10.48550/arXiv.2305.14325
  Direct empirical source for the "multi-agent debate can reduce or amplify errors" discussion (false-consensus cascades vs. genuine correction).

- **MetaGPT: Meta Programming for A Multi-Agent Collaborative Framework**
  Hong, S., Zheng, X., Chen, J., Cheng, Y., Zhang, C., Wang, J., Wang, Z., Yau, S. K. S., Lin, Z., Zhou, L., Ran, C., Xiao, L., Wu, C., & Schmidhuber, J., 2023, *arXiv preprint*.
  [arXiv:2308.00352](https://arxiv.org/abs/2308.00352) · DOI: 10.48550/arXiv.2308.00352
  The paper that coined "cascading hallucination" from naively chained LLM agents and proposed SOP-based structured handoffs as the fix — central to Section 5.1.

- **CAMEL: Communicative Agents for "Mind" Exploration of Large Language Model Society**
  Li, G., Hammoud, H. A. A. K., Itani, H., Khizbullin, D., & Ghanem, B., 2023, *Advances in Neural Information Processing Systems (NeurIPS 2023)*.
  [arXiv:2303.17760](https://arxiv.org/abs/2303.17760) · DOI: 10.48550/arXiv.2303.17760
  Role-playing/"inception prompting" framework for autonomous multi-agent cooperation without continuous human steering.

- **AutoGen: Enabling Next-Gen LLM Applications via Multi-Agent Conversation**
  Wu, Q., Bansal, G., Zhang, J., Wu, Y., Zhang, S., Zhu, E., Li, B., Jiang, L., Zhang, X., & Wang, C., 2023, *arXiv preprint*.
  [arXiv:2308.08155](https://arxiv.org/abs/2308.08155) · DOI: 10.48550/arXiv.2308.08155
  Generalizable conversable-agent framework underlying many of the tools in this repo's [Tools & Libraries](../tools/) section.

- **Voyager: An Open-Ended Embodied Agent with Large Language Models**
  Wang, G., Xie, Y., Jiang, Y., Mandlekar, A., Xiao, C., Zhu, Y., Fan, L., & Anandkumar, A., 2023, *Transactions on Machine Learning Research (TMLR 2024)*.
  [arXiv:2305.16291](https://arxiv.org/abs/2305.16291) · DOI: 10.48550/arXiv.2305.16291
  Skill-library + iterative-prompting architecture that treats execution errors as feedback rather than context contaminants — a real long-horizon rollback example.

---

## Applications

- **Augmenting Large Language Models with Chemistry Tools (ChemCrow)**
  Bran, A. M., Cox, S., Schilter, O., Baldassari, C., White, A. D., & Schwaller, P., 2024, *Nature Machine Intelligence*, 6, 525–535.
  [DOI: 10.1038/s42256-024-00832-8](https://doi.org/10.1038/s42256-024-00832-8) (also as [arXiv:2304.05376](https://arxiv.org/abs/2304.05376))
  Domain-specific scientific tool-use agent (18 chemistry tools); shows real-world consequences when a research-automation agent's intermediate step is wrong.

- **The AI Scientist: Towards Fully Automated Open-Ended Scientific Discovery**
  Lu, C., Lu, C., Lange, R. T., Foerster, J., Clune, J., & Ha, D., 2024, *arXiv preprint*.
  [arXiv:2408.06292](https://arxiv.org/abs/2408.06292) · DOI: 10.48550/arXiv.2408.06292
  End-to-end automated hypothesis→code→paper pipeline; the primary case study this repository's paper builds its DAG error-propagation model around.

- **The AI Scientist-v2: Workshop-Level Automated Scientific Discovery via Agentic Tree Search**
  Yamada, Y., Lange, R. T., Lu, C., Hu, S., Lu, C., Foerster, J., Clune, J., & Ha, D., 2025, *arXiv preprint*.
  [arXiv:2504.08066](https://arxiv.org/abs/2504.08066) · DOI: 10.48550/arXiv.2504.08066
  Replaces the linear v1 pipeline with progressive tree search and branch rollback — the concrete implementation of Section 5.3's mitigation strategy.

---

## Evaluation Methods / Benchmarks

- **AgentBench: Evaluating LLMs as Agents**
  Liu, X., Yu, H., Zhang, H., Xu, Y., Lei, X., Lai, H., Gu, Y., Ding, H., Men, K., Yang, K., Zhang, S., Deng, X., Zeng, A., Du, Z., Zhang, C., Shen, S., Zhang, T., Su, Y., Sun, H., Huang, M., Dong, Y., & Tang, J., 2023, *International Conference on Learning Representations (ICLR 2024)*.
  [arXiv:2308.03688](https://arxiv.org/abs/2308.03688) · DOI: 10.48550/arXiv.2308.03688
  8-environment benchmark showing long-horizon multi-step tasks are exactly where LLM agents fail most — direct empirical support for the "5–10 step reliability cliff" cited in Section 2.2.

- **WebArena: A Realistic Web Environment for Building Autonomous Agents**
  Zhou, S., Xu, F. F., Zhu, H., Zhou, X., Lo, R., Sridhar, A., Cheng, X., Ou, T., Bisk, Y., Fried, D., Alon, U., & Neubig, G., 2023, *International Conference on Learning Representations (ICLR 2024)*.
  [arXiv:2307.13854](https://arxiv.org/abs/2307.13854) · DOI: 10.48550/arXiv.2307.13854
  Execution-verified, self-hostable web benchmark; best agent solves only ~14% of tasks vs. 78% for humans, illustrating compounding step failure.

- **SWE-bench: Can Language Models Resolve Real-World GitHub Issues?**
  Jimenez, C. E., Yang, J., Wettig, A., Yao, S., Pei, K., Press, O., & Narasimhan, K., 2023, *International Conference on Learning Representations (ICLR 2024)*.
  [arXiv:2310.06770](https://arxiv.org/abs/2310.06770) · DOI: 10.48550/arXiv.2310.06770
  2,294 real GitHub-issue repair tasks requiring multi-file, multi-step coordinated agent edits — the coding-agent analogue of this repo's own research-automation focus.

- **GAIA: A Benchmark for General AI Assistants**
  Mialon, G., Fourrier, C., Swift, C., Wolf, T., LeCun, Y., & Scialom, T., 2023, *arXiv preprint*.
  [arXiv:2311.12983](https://arxiv.org/abs/2311.12983) · DOI: 10.48550/arXiv.2311.12983
  466 real-world, tool-use-and-reasoning questions; human accuracy (92%) vs. GPT-4 + plugins (15%) is a stark, oft-cited illustration of agentic reliability gaps.

