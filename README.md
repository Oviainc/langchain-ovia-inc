![Ovia Inc — LangChain logo, from the upstream repository's own assets](.github/images/logo-dark.svg)

## Ovia Inc — LangChain fork

This repository is a fork of [langchain-ai/langchain](https://github.com/langchain-ai/langchain), held in the Ovia Inc collection for evaluation. Modifications by Ovia Inc: this header (Ovia section, story, and reference note), added November 2026 as part of the import pass that widened the collection beyond the weekly digest. Upstream code and content are otherwise unchanged from the fork point, except where a later commit says so. All credit for the project belongs to the upstream authors and contributors; the licence is MIT, as recorded in the upstream repository.

### What this is

LangChain is a framework for building agents and LLM-powered applications. It chains together interoperable components and third-party integrations to simplify AI application development while future-proofing decisions as the underlying technology evolves. The wider ecosystem around the framework includes LangGraph for controllable agent workflows, a JavaScript/TypeScript equivalent, Deep Agents for higher-level agent patterns, and LangSmith for developing, debugging, and deploying agents and LLM applications.

### Story

LangChain grew from a component library for LLM applications into what its own README now calls "the agent engineering platform" — the framework layer underneath a large share of the agent tooling built since. The collection already held the LangGraph fork, the graph-orchestration framework built on LangChain, along with CrewAI and AutoGen on the same shelf. The base framework itself was the missing piece: evaluation notes on the orchestration layer kept pointing back at the components, model interfaces, and integration surface defined here. We forked langchain-ai/langchain in November 2026 to close that gap, so the frameworks shelf reads as a stack — components and integrations at the base, graph orchestration above them, crew and conversation frameworks beside them.

### What we evaluate

- The component model: how model interfaces, tools, and integrations compose, and where the seams sit for swapping providers.
- The relationship between the base framework and LangGraph — when plain chaining suffices and when graph control earns its complexity.
- Deep Agents as the higher-level pattern layer: planning, sub-agents, and filesystem use as built-in capabilities.
- Fit against the crew and conversation frameworks already on the shelf, on the same evaluation workloads.

---

<div align="center">
  <a href="https://docs.langchain.com/oss/python/langchain/overview">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset=".github/images/logo-dark.svg">
      <source media="(prefers-color-scheme: light)" srcset=".github/images/logo-light.svg">
      <img alt="LangChain Logo" src=".github/images/logo-dark.svg" width="50%">
    </picture>
  </a>
</div>

<div align="center">
  <h3>The agent engineering platform.</h3>
</div>

<div align="center">
  <a href="https://opensource.org/licenses/MIT" target="_blank"><img src="https://img.shields.io/pypi/l/langchain" alt="PyPI - License"></a>
  <a href="https://pypistats.org/packages/langchain" target="_blank"><img src="https://img.shields.io/pepy/dt/langchain" alt="PyPI - Downloads"></a>
  <a href="https://pypi.org/project/langchain/#history" target="_blank"><img src="https://img.shields.io/pypi/v/langchain?label=%20" alt="Version"></a>
  <a href="https://x.com/langchain_oss" target="_blank"><img src="https://img.shields.io/twitter/url/https/twitter.com/langchain_oss.svg?style=social&label=Follow%20%40LangChain" alt="Twitter / X"></a>
</div>

<br>

LangChain is a framework for building agents and LLM-powered applications. It helps you chain together interoperable components and third-party integrations to simplify AI application development — all while future-proofing decisions as the underlying technology evolves.

> [!TIP]
> Just getting started? Check out **[Deep Agents](https://docs.langchain.com/oss/python/deepagents/)** — a higher-level package built on LangChain for agents that have built-in capabilities for common usage patterns such as planning, subagents, file system usage, and more.

## Quickstart

```bash
uv add langchain
```

```python
from langchain.chat_models import init_chat_model

model = init_chat_model("openai:gpt-5.5")
result = model.invoke("Hello, world!")
```

If you're looking for more advanced customization or agent orchestration, check out [LangGraph](https://github.com/langchain-ai/langgraph), our framework for building controllable agent workflows.

For an equivalent JS/TS library, check out [LangChain.js](https://github.com/langchain-ai/langchainjs).

> [!TIP]
> For developing, debugging, and deploying AI agents and LLM applications, see [LangSmith](https://docs.langchain.com/langsmith/home).

## LangChain ecosystem

While the LangChain framework can be used standalone, it also integrates seamlessly with any LangChain product, giving developers a full suite of tools when building LLM applications.

- **[Deep Agents](https://docs.langchain.com/oss/python/deepagents/)** — Build agents that can plan, use subagents, and leverage file systems for complex tasks
- **[LangGraph](https://docs.langchain.com/oss/python/langgraph/overview)** — Build agents that can reliably handle complex tasks with our low-level agent orchestration framework
- **[Integrations](https://docs.langchain.com/oss/python/integrations/providers/overview)** — Chat & embedding models, tools & toolkits, and more
- **[LangSmith](https://www.langchain.com/langsmith)** — Agent evals, observability, and debugging for LLM apps
- **[LangSmith Deployment](https://docs.langchain.com/langsmith/deployments)** — Deploy and scale agents with a purpose-built platform for long-running, stateful workflows

## Why use LangChain?

LangChain helps developers build applications powered by LLMs through a standard interface for models, embeddings, vector stores, and more.

- **Real-time data augmentation** — Easily connect LLMs to diverse data sources and external/internal systems, drawing from LangChain's vast library of integrations with model providers, tools, vector stores, retrievers, and more
- **Model interoperability** — Swap models in and out as your engineering team experiments to find the best choice for your application's needs. As the industry frontier evolves, adapt quickly — LangChain's abstractions keep you moving without losing momentum
- **Rapid prototyping** — Quickly build and iterate on LLM applications with LangChain's modular, component-based architecture. Test different approaches and workflows without rebuilding from scratch, accelerating your development cycle
- **Production-ready features** — Deploy reliable applications with built-in support for monitoring, evaluation, and debugging through integrations like LangSmith. Scale with confidence using battle-tested patterns and best practices
- **Vibrant community and ecosystem** — Leverage a rich ecosystem of integrations, templates, and community-contributed components. Benefit from continuous improvements and stay up-to-date with the latest AI developments through an active open-source community
- **Flexible abstraction layers** — Work at the level of abstraction that suits your needs — from high-level chains for quick starts to low-level components for fine-grained control. LangChain grows with your application's complexity

---

## Resources

- [Documentation](https://docs.langchain.com/oss/python/langchain/overview) — conceptual overviews and guides
- [LangChain ecosystem overview](https://docs.langchain.com/oss/python/concepts/products) — how LangChain, LangGraph, and Deep Agents fit together
- [API reference](https://reference.langchain.com/python) — complete reference for all public classes, functions, and types
- [Discussions](https://forum.langchain.com/c/oss-product-help-lc-and-lg/langchain/14) — community forum for technical questions, ideas, and feedback
- [LangChain Academy](https://academy.langchain.com/) — comprehensive, free courses on LangChain libraries and products, made by the LangChain team
- [Contributing Guide](https://docs.langchain.com/oss/python/contributing/overview) — how to contribute and find good first issues
- [Code of Conduct](https://github.com/langchain-ai/langchain/?tab=coc-ov-file) — community guidelines and standards
