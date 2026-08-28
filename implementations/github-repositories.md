# GitHub Implementations

Reference implementations directly tied to the papers in this collection. Selected for documentation quality, activity, and direct correspondence to a cited paper (not by star count alone).

- **ysymyth/ReAct** — [github.com/ysymyth/ReAct](https://github.com/ysymyth/ReAct)
  Official implementation of the ReAct paper (ICLR 2023). Implements the interleaved reasoning-and-acting loop across the paper's QA, fact-verification, and interactive decision-making benchmarks.

- **noahshinn/reflexion** — [github.com/noahshinn/reflexion](https://github.com/noahshinn/reflexion)
  Official implementation of Reflexion (NeurIPS 2023). Demonstrates the Actor/Evaluator/Self-Reflection loop and episodic memory buffer described in the paper.

- **geekan/MetaGPT** — [github.com/geekan/MetaGPT](https://github.com/geekan/MetaGPT)
  Official, actively maintained implementation of the MetaGPT multi-agent SOP framework; directly relevant to this paper's Section 5.1 discussion of schema-restricted agent handoffs as an error-mitigation strategy.

- **princeton-nlp/tree-of-thought-llm** — [github.com/princeton-nlp/tree-of-thought-llm](https://github.com/princeton-nlp/tree-of-thought-llm)
  Official implementation of Tree of Thoughts (NeurIPS 2023), including the code repo referenced directly in the paper for all prompts and search strategies.

- **MineDojo/Voyager** — [github.com/MineDojo/Voyager](https://github.com/MineDojo/Voyager)
  Official implementation of Voyager; illustrates a working skill-library-plus-rollback architecture where execution errors become feedback signals rather than propagating silently — a real-world instance of the checkpoint-rollback idea in Section 7.1 of the paper.

- **princeton-nlp/SWE-agent** — [github.com/SWE-agent/SWE-agent](https://github.com/SWE-agent/SWE-agent)
  Agent-computer interface built specifically for the SWE-bench benchmark; useful as a concrete example of tool-execution sandboxing and structured environment feedback for coding agents.

- **web-arena-x/webarena** — [github.com/web-arena-x/webarena](https://github.com/web-arena-x/webarena)
  Canonical implementation used to reproduce the WebArena paper's results; self-hostable and includes the functional-correctness validators used to score long-horizon web tasks.
