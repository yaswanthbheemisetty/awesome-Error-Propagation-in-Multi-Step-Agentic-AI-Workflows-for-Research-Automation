# Awesome [Error-Propagation-in-Multi-Step-Agentic-AI-Workflows-for-Research-Automation]
This paper investigates how errors propagate and amplify across multi-agent LLM workflows used for automated scientific discovery.

A curated collection of research papers, datasets, tools,
implementations and learning resources related to [Error-Propagation-in-Multi-Step-Agentic-AI-Workflows-for-Research-Automation].
## Contents
- Overview
- AI-Assisted Research Paper
- Survey Papers
- Foundational Papers
- Recent Research
- Datasets
- Tools and Libraries
- GitHub Implementations
- Tutorials
- Citation Integrity Audit
## Overview
Brief Introduction

Agentic AI workflows use Large Language Models (LLMs) to perform complex research tasks through multiple interconnected steps, such as literature review, hypothesis generation, experiment execution, data analysis, and scientific writing. While these systems can automate significant parts of the research process, errors introduced at any stage can propagate to subsequent stages and become amplified.

Error propagation in multi-step agentic AI workflows refers to the accumulation and cascading of incorrect information, tool failures, hallucinations, or flawed reasoning throughout an AI pipeline. Understanding these failure patterns is essential for developing reliable, self-correcting, and trustworthy AI systems capable of supporting automated scientific discovery.
## AI-Assisted Research Paper

[View Paper](paper/AI_Assisted_Research_Paper.pdf)
## Survey Papers


- [LLM Agents: A Survey](https://arxiv.org/) — A comprehensive survey of large language model-based agents, covering planning, memory, tool use, reasoning, and multi-agent systems.
- [LLM-Based Multi-Agent Orchestration: A Survey of Frameworks, Communication Protocols, and Emerging Patterns](https://www.mdpi.com/1999-5903/18/6/326) — Survey of multi-agent orchestration architectures, communication protocols, coordination mechanisms, and emerging agentic patterns.


## Foundational Papers

- [ReAct: Synergizing Reasoning and Acting in Language Models](https://arxiv.org/abs/2210.03629) — Introduced the reasoning-and-acting paradigm that combines language-model reasoning with interaction with external tools and environments.

- [Reflexion: Language Agents with Verbal Reinforcement Learning](https://arxiv.org/abs/2303.11366) — Introduced verbal feedback and reflection mechanisms for improving agent performance across multiple attempts.

- [Self-Refine: Iterative Refinement with Self-Feedback](https://arxiv.org/abs/2303.17651) — Proposed iterative generation, feedback, and refinement for improving LLM outputs.

- [Teaching Large Language Models to Self-Debug](https://arxiv.org/abs/2304.05128) — Explored self-debugging techniques that allow language models to identify and correct errors in generated programs.

- [Generative Agents: Interactive Simulacra of Human Behavior](https://arxiv.org/abs/2304.03442) — Introduced agents with memory, reflection, and planning mechanisms for maintaining coherent behavior over extended interactions.

- [ChemCrow: Augmenting Large-Language Models with Chemistry Tools](https://arxiv.org/abs/2304.05376) — Demonstrated tool-augmented LLM agents for scientific and chemical reasoning workflows.

- [MetaGPT: Meta Programming for a Multi-Agent Collaborative Framework](https://arxiv.org/abs/2308.00352) — Introduced structured multi-agent collaboration using standardized roles and structured handoffs.


## Recent Research Papers

- [AgentBench: Evaluating LLMs as Agents](https://arxiv.org/abs/2308.03688) — A benchmark for evaluating LLM-based agents across multiple environments and tasks.

- [WebArena: A Realistic Web Environment for Building Autonomous Agents](https://arxiv.org/abs/2307.13854) — Introduced a realistic web environment for evaluating autonomous agents on long-horizon web tasks.

- [The AI Scientist: Towards Fully Automated Open-Ended Scientific Discovery](https://arxiv.org/abs/2408.06292) — Proposed an end-to-end system capable of generating research ideas, implementing experiments, analyzing results, and producing scientific manuscripts.

- [The AI Scientist-v2: Workshop-Level Automated Scientific Discovery via Agentic Tree Search](https://arxiv.org/abs/2504.08066) — Extended autonomous scientific discovery using agentic tree search, allowing failed experimental branches to be explored, pruned, and replaced.

- [Towards an AI Co-Scientist](https://arxiv.org/abs/2502.18864) — Presented a multi-agent system designed to assist scientists with hypothesis generation, refinement, and research exploration.

- [Agent Laboratory: Using LLM Agents as Research Assistants](https://arxiv.org/) — Explored the use of LLM agents as research assistants for conducting and supporting scientific research workflows.

## Datasets

This dataset is designed to support research on **error propagation in multi-step agentic AI workflows**. It focuses on execution traces in which an AI agent performs multiple reasoning, tool-use, and decision-making steps.

The dataset can be used to study:

- **Error Detection** — identifying the step where an agent first makes an error.
- **Error Propagation** — analyzing how an initial error affects subsequent steps.
- **Root Cause Analysis** — determining the primary cause of workflow failure.
- **Failure Recovery** — evaluating whether an agent can detect and recover from an earlier mistake.
- **Workflow Reliability** — measuring how reliability changes as the number of sequential steps increases.

Each workflow can be represented as a sequence or graph of agent steps, including the agent's action, tool interaction, outcome, and associated failure information.

> **Note:** The dataset is intended for research and benchmarking of agent reliability, error propagation, and failure analysis rather than simply measuring final task accuracy.
## Tools and Libraries

The project uses the following tools and libraries for developing, testing, and analyzing multi-step agentic AI workflows:

- **Python** — Primary programming language for implementing experiments and data-processing pipelines.
- **Large Language Models (LLMs)** — Used as the reasoning and decision-making components of agentic workflows.
- **PyTorch** — Used for machine learning and model-related experimentation.
- **Pandas** — Used for dataset processing, manipulation, and analysis.
- **NumPy** — Used for numerical computations and statistical operations.
- **Matplotlib** — Used to visualize experimental results, error rates, and workflow performance.
- **Jupyter Notebook / Google Colab** — Used for interactive experimentation and analysis.
- **Git & GitHub** — Used for version control, project management, and sharing research resources.
- **arXiv** — Used as a source for relevant research papers on LLM agents, scientific discovery, and AI reliability.
## GitHub Implementations

This repository provides an implementation and research resource for studying **Error Propagation in Multi-Step Agentic AI Workflows for Research Automation**.

The implementation focuses on:

- Building multi-step agentic workflows.
- Tracking execution traces across individual steps.
- Injecting and identifying errors at different stages.
- Measuring how errors propagate to downstream steps.
- Comparing self-checking and independent verification strategies.
- Analyzing workflow reliability and cascading failures.
- Providing experimental code, datasets, and supporting resources for reproducible research.

The repository is organized to make it easier to reproduce experiments, analyze agent behavior, and extend the proposed error-propagation framework.

## Tutorials

This section provides tutorials and practical resources for understanding and implementing multi-step agentic AI workflows, error detection, verification, and failure recovery.

- **LLM Agents** — Introduction to building autonomous agents using LLMs, tools, memory, planning, and reasoning.
- **ReAct Agents** — Tutorial on combining reasoning and tool-based actions in an agent workflow.
- **Multi-Agent Systems** — Guides for designing workflows involving multiple specialized AI agents.
- **Tool Calling** — Tutorials on connecting LLMs with external APIs, Python functions, search tools, and other environments.
- **Agent Evaluation** — Resources for evaluating agent performance, reliability, and failure cases.
- **Error Handling & Verification** — Practical approaches for detecting, validating, and recovering from intermediate agent errors.
- **LangChain / LangGraph** — Tutorials for building structured, stateful, and multi-step agent workflows.
- **AI Scientific Discovery** — Tutorials and examples related to using AI agents for automated research and scientific experimentation.
## Citation Integrity Audit
[View Audit](citation-audit/Citation_Integrity_Audit.pdf)
## License
...
