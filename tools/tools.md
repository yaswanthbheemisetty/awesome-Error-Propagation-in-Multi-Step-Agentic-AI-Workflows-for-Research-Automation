# Tools & Libraries

Software frameworks used to build, orchestrate, or verify the kinds of multi-step agentic workflows discussed in this repository's research paper.

- **LangChain**
  [github.com/langchain-ai/langchain](https://github.com/langchain-ai/langchain)
  General-purpose framework for chaining LLM calls, tool use, and memory; the most widely-used base layer for building ReAct-style agent loops.

- **LangGraph**
  [github.com/langchain-ai/langgraph](https://github.com/langchain-ai/langgraph)
  Graph-based orchestration layer (built on LangChain) for stateful, multi-step, and multi-agent workflows — directly relevant to modeling agent pipelines as a DAG, as this paper does in Section 3.

- **AutoGen**
  [github.com/microsoft/autogen](https://github.com/microsoft/autogen)
  Microsoft's multi-agent conversation framework (companion library to the AutoGen paper in [references.md](../references/references.md)); supports customizable "conversable agents" and human-in-the-loop checkpoints.

- **CrewAI**
  [github.com/crewAIInc/crewAI](https://github.com/crewAIInc/crewAI)
  Role-based multi-agent orchestration framework (agents with defined roles, goals, and tools) built independently of LangChain; useful for implementing the "assembly line" / SOP-style handoffs described in the MetaGPT paper.

- **LlamaIndex**
  [github.com/run-llama/llama_index](https://github.com/run-llama/llama_index)
  Data-framework for connecting LLMs to external knowledge sources and structured retrieval pipelines; relevant to mitigating the "literature retrieval and context contamination" error pathway (Section 4.1) via more reliable grounding.
