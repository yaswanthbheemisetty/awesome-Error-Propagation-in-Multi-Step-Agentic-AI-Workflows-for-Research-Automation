# Datasets & Benchmarks

These are the primary interactive-environment datasets/benchmarks used in agentic-AI reliability research. Each one doubles as both a *dataset* (tasks + environments + ground truth) and the empirical basis for one of the [papers](../references/references.md) in this collection, so descriptions below focus on the data itself rather than repeating the paper summary.

- **AgentBench**
  Source: [github.com/THUDM/AgentBench](https://github.com/THUDM/AgentBench) · Paper: Liu et al., 2023 ([arXiv:2308.03688](https://arxiv.org/abs/2308.03688))
  Description: 8 distinct interactive environments (OS, Database, Knowledge Graph, Digital Card Game, Lateral Thinking Puzzles, House-Holding/ALFWorld, Web Shopping, Web Browsing), each with task-specific success metrics scored over multi-turn agent rollouts.
  Use in this project: Used as the primary source for the multiplicative step-success-rate figures (e.g., the 5–10 step reliability cliff) discussed in Section 2.2 of the paper.

- **WebArena**
  Source: [github.com/web-arena-x/webarena](https://github.com/web-arena-x/webarena) · Paper: Zhou et al., 2023 ([arXiv:2307.13854](https://arxiv.org/abs/2307.13854))
  Description: 812 long-horizon tasks (241 templates) across four fully-functional, self-hostable websites (e-commerce, forum, GitLab-style dev platform, CMS), graded by programmatic, execution-based success checks rather than surface-form matching.
  Use in this project: Cited as evidence that even strong CoT-augmented agents solve only ~14% of tasks end-to-end, illustrating how error compounds across long action sequences.

- **GAIA (General AI Assistants benchmark)**
  Source: [huggingface.co/datasets/gaia-benchmark/GAIA](https://huggingface.co/datasets/gaia-benchmark/GAIA) · Paper: Mialon et al., 2023 ([arXiv:2311.12983](https://arxiv.org/abs/2311.12983))
  Description: 466 real-world questions spanning three difficulty levels (1–2 steps up to arbitrarily long tool-use chains), with reasoning, multi-modality, and web-browsing requirements; scored by short, unambiguous ground-truth answers.
  Use in this project: Referenced for the human-vs-agent performance gap (92% vs. 15%) as a benchmark-level illustration of agentic unreliability on tool-use-heavy, multi-step tasks.

- **SWE-bench**
  Source: [github.com/princeton-nlp/SWE-bench](https://github.com/princeton-nlp/SWE-bench) · Paper: Jimenez et al., 2023 ([arXiv:2310.06770](https://arxiv.org/abs/2310.06770))
  Description: 2,294 real GitHub issue/pull-request pairs across 12 popular Python repositories; an agent must edit a real codebase to resolve an issue, with success measured by whether the repository's own test suite passes.
  Use in this project: Used as the coding-agent analogue to the paper's "code & tool execution state corruption" pathway (Section 4.2) — silent failures here directly correspond to unresolved or partially-resolved issues.
