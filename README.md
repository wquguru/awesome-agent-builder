# Awesome Agent Builder

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![License: CC0-1.0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg)](https://creativecommons.org/publicdomain/zero/1.0/)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

> The complete resource map for building AI agents — organized by developer growth stage.
>
> AI Agent 开发者完整资源地图 —— 按成长阶段组织。

Unlike other awesome lists that simply dump 300+ links, this project organizes resources along **your growth path** as an agent developer — from first principles to production deployment, from learning to career.

与其他简单罗列 300+ 链接的 awesome 列表不同，本项目按照 **开发者成长路径** 组织资源 —— 从基础原理到生产部署，从学习到职业发展。

Curated by [AgentWay.dev](https://agentway.dev) | 由 [AgentWay.dev](https://agentway.dev) 策划

---

## Contents | 目录

- [How to Use This List | 如何使用本列表](#how-to-use-this-list--如何使用本列表)
- [The SDK Wars | SDK 混战](#the-sdk-wars--which-framework-should-you-choose--sdk-混战--你该选哪个框架)
- [Stage 1: Agent Fundamentals | 基础入门](#stage-1-agent-fundamentals--基础入门)
  - [Agent Frameworks | Agent 框架](#agent-frameworks--agent-框架)
  - [Starter Templates & Boilerplates | 入门模板](#starter-templates--boilerplates--入门模板)
- [Stage 2: Tools & Integration | 工具与集成](#stage-2-tools--integration--工具与集成)
  - [Tool Use & Function Calling | 工具调用](#tool-use--function-calling--工具调用)
  - [MCP Servers & Ecosystem | MCP 服务与生态](#mcp-servers--ecosystem--mcp-服务与生态)
  - [Memory & Context Management | 记忆与上下文管理](#memory--context-management--记忆与上下文管理)
  - [Prompt Engineering | 提示词工程](#prompt-engineering--提示词工程)
- [Stage 3: Advanced Patterns | 高级模式](#stage-3-advanced-patterns--高级模式)
  - [Multi-Agent Systems | 多 Agent 系统](#multi-agent-systems--多-agent-系统)
  - [RAG & Knowledge | RAG 与知识库](#rag--knowledge--rag-与知识库)
  - [Evaluation & Testing | 评估与测试](#evaluation--testing--评估与测试)
  - [Coding Agents | 编程 Agent](#coding-agents--编程-agent)
- [Stage 4: Production & Operations | 生产部署](#stage-4-production--operations--生产部署)
  - [Agent Deployment & Hosting | 部署与托管](#agent-deployment--hosting--部署与托管)
  - [Observability & Monitoring | 可观测与监控](#observability--monitoring--可观测与监控)
  - [Safety & Guardrails | 安全与护栏](#safety--guardrails--安全与护栏)
  - [LLM Serving & Inference | 模型服务与推理](#llm-serving--inference--模型服务与推理)
- [Learning Resources | 学习资源](#learning-resources--学习资源)
  - [Structured Courses | 系统课程](#structured-courses--系统课程)
  - [Tutorials & Guides | 教程与指南](#tutorials--guides--教程与指南)
  - [Books | 书籍](#books--书籍)
  - [Podcasts & Videos | 播客与视频](#podcasts--videos--播客与视频)
  - [Newsletters | 订阅通讯](#newsletters--订阅通讯)
- [Career & Jobs | 职业发展](#career--jobs--职业发展)
  - [Top Companies Are Hiring | 头部团队招聘](#top-companies-are-hiring--agent-is-real--头部团队正在大规模招聘--agent-不是概念)
  - [In-Demand Roles | 热门岗位](#in-demand-roles--热门岗位)
  - [Job Boards | 招聘平台](#job-boards--招聘平台)
  - [Interview Prep | 面试准备](#interview-prep--面试准备)
  - [Portfolio Projects | 作品集项目](#portfolio-projects--作品集项目)
- [Community | 社区](#community--社区)
  - [Discord & Slack Communities | Discord 与 Slack 社区](#discord--slack-communities--discord-与-slack-社区)
  - [Conferences & Meetups | 会议与活动](#conferences--meetups--会议与活动)
  - [Chinese Community | 中文社区](#chinese-community--中文社区)

---

## How to Use This List | 如何使用本列表

This list is organized by **developer growth stage**. Pick your current level and explore:

本列表按 **开发者成长阶段** 组织，找到你当前的级别开始探索：

| Stage | You Are Here If... | 适合你如果... |
|---|---|---|
| **Stage 1: Fundamentals** | Building your first agent, learning the basics | 正在构建第一个 Agent，学习基础知识 |
| **Stage 2: Tools & Integration** | Adding tools, memory, and external services | 为 Agent 添加工具、记忆和外部服务 |
| **Stage 3: Advanced Patterns** | Designing multi-agent systems, RAG, eval | 设计多 Agent 系统、RAG、评估体系 |
| **Stage 4: Production** | Deploying, monitoring, and securing agents | 部署、监控和保障 Agent 安全 |

Legend | 图例:
- Tags indicate maturity: `Production` `Experimental` `Research`
- 标签表示成熟度：`生产可用` `实验性` `研究性`

---

## The SDK Wars — Which Framework Should You Choose? | SDK 混战 —— 你该选哪个框架？

Agent development frameworks are emerging at breakneck speed — Claude Agent SDK, Vercel AI SDK, Google GenAI SDK, LangChain, Pydantic AI... It feels just like the TensorFlow vs. PyTorch vs. PaddlePaddle deep learning framework wars all over again. As a developer, the choices are overwhelming.

Agent 开发框架层出不穷 —— Claude Agent SDK、Vercel AI SDK、Google GenAI SDK、LangChain、Pydantic AI…… 这场景像极了当年 TensorFlow、PyTorch、PaddlePaddle 深度学习框架混战，开发者目不暇接。

**So which framework should you choose? npm weekly downloads tell a clear story.** Over the past year (March 2025 → March 2026):

**应该选择哪个？npm 周下载量给出了明确答案。** 过去一年（2025.03 → 2026.03）：

| SDK | npm Package | Mar 2025 | Mar 2026 | YoY Growth |
|---|---|---|---|---|
| **Vercel AI SDK** | `ai` | 1.04M | 4.54M | **4.4x** 🔥 |
| **Google GenAI SDK** | `@google/genai` | 3K | 4.76M | **1,658x** 🚀 |
| **Anthropic SDK** | `@anthropic-ai/sdk` | 1.08M | 4.51M | **4.2x** 🔥 |
| **Claude Code** | `@anthropic-ai/claude-code` | 164K | 4.02M | **24.5x** 🚀 |
| **Claude Agent SDK** | `@anthropic-ai/claude-agent-sdk` | — | 1.58M | *New in 2025* |
| **LangChain Core** | `@langchain/core` | 865K | 1.59M | **1.8x** |
| **LangChain** | `langchain` | 691K | 990K | **1.4x** |

> *Data source: [npm API](https://api.npmjs.org/) — verified March 23, 2026 | 数据来源：npm 官方 API，2026年3月23日核实*

**The trend is clear | 趋势很明确：**
- **Claude ecosystem surges** — Claude Code (24.5x!) is the fastest growing package. Combined with Anthropic SDK (4.51M) and Claude Agent SDK (1.58M, launched late 2025), the Claude ecosystem shows the strongest developer momentum.
- **Model-native SDKs win** — Developers are moving from general orchestration frameworks (LangChain 1.4x) to model-native SDKs (Vercel 4.4x, Anthropic 4.2x, Google 1,658x).
- **Pydantic AI is the Python dark horse** — 2.9M weekly PyPI downloads. The "FastAPI of agents" is resonating with Python developers.

**Claude 生态势能最强** —— Claude Code（24.5倍增长！）是增速最快的包。结合 Anthropic SDK（周下载451万）和 Claude Agent SDK（158万，2025下半年新发布），Claude 生态展现出最强开发者动能。**模型原生 SDK 胜出** —— 开发者正从通用编排框架（LangChain 1.4倍）迁移到模型原生 SDK（Vercel 4.4倍, Anthropic 4.2倍, Google 1,658倍）。**Pydantic AI 是 Python 黑马** —— PyPI 周下载290万，"Agent 界的 FastAPI" 定位深入人心。

> **Deep analysis | 深入分析**: [AgentWay — Framework Guide](https://agentway.dev/learn/docs/frameworks) covers framework selection strategy in detail.

---

## Stage 1: Agent Fundamentals | 基础入门

> Start here. Understand what agents are, pick a framework, and build your first agent loop.
>
> 从这里开始。理解 Agent 是什么，选择框架，构建你的第一个 Agent 循环。

### Agent Frameworks | Agent 框架

Full-featured frameworks for building agent applications. Ranked by adoption and ecosystem maturity.

用于构建 Agent 应用的全功能框架，按采用度和生态成熟度排列。

| Project | Stars | Weekly Downloads | Description | Best For |
|---|---|---|---|---|
| [Claude Agent SDK](https://github.com/anthropics/claude-agent-sdk-typescript) | — | 1.58M (npm) 🚀 | Anthropic's agent framework — tool use, computer use, agentic loops. New in 2025, fastest ecosystem growth. | Claude-native agents |
| [AI SDK (Vercel)](https://github.com/vercel/ai) | 15k+ | 4.54M (npm) 🔥 | Multi-provider TypeScript SDK for streaming AI in React/Next.js apps. 4.4x YoY. | TypeScript / Web |
| [LangGraph](https://github.com/langchain-ai/langgraph) | 15k+ | 34.5M (PyPI/mo) | Stateful, graph-based agent workflows. LangChain's production agent layer. `Production` | Complex workflows |
| [LangChain](https://github.com/langchain-ai/langchain) | 100k+ | 990K (npm) | The original LLM application framework with extensive integrations. | Broad ecosystem |
| [CrewAI](https://github.com/crewAIInc/crewAI) | 25k+ | — | Role-playing agent orchestration for collaborative teams. Fastest-adopted multi-agent framework. | Multi-agent teams |
| [AutoGen](https://github.com/microsoft/autogen) | 40k+ | — | Event-driven multi-agent framework by Microsoft. Merging with Semantic Kernel. | Multi-agent conv. |
| [Semantic Kernel](https://github.com/microsoft/semantic-kernel) | 25k+ | — | Microsoft enterprise SDK for Python, C#, Java with plugins and planning. `Production` | Enterprise / .NET |
| [OpenAI Agents SDK](https://github.com/openai/openai-agents-python) | 15k+ | — | Lightweight multi-agent SDK with tracing, handoffs, and guardrails. | GPT-native agents |
| [Google ADK](https://github.com/google/adk-python) | 10k+ | — | Modular agent dev kit integrating Gemini/Vertex AI. | Google ecosystem |
| [Pydantic AI](https://github.com/pydantic/pydantic-ai) | 15k+ | 2.9M (PyPI) | Type-safe agent framework built on Pydantic. "FastAPI of agents." | Python + type safety |
| [Mastra](https://github.com/mastra-ai/mastra) | 10k+ | — | Opinionated TypeScript framework with RAG and observability. | TypeScript apps |
| [Strands Agents](https://github.com/strands-agents/sdk-python) | 5k+ | — | AWS model-driven agent SDK with Bedrock integration. `Production` | AWS / Bedrock |

**How to choose | 如何选择:**
- 🟢 **Just starting?** → Claude Agent SDK or OpenAI Agents SDK — minimal API, fast to learn
- ⚡ **Claude ecosystem?** → Claude Agent SDK + Claude Code — strongest growth momentum (24.5x YoY)
- 🔷 **TypeScript / Web?** → Vercel AI SDK (4.5M weekly) + Mastra — dominant TS stack
- 🔄 **Complex workflows?** → LangGraph — graph-based state machines, production-proven
- 🤝 **Multi-agent teams?** → CrewAI or AutoGen — role-based collaboration
- 🐍 **Python + Type Safety?** → Pydantic AI — the FastAPI of agents (2.9M weekly)
- 🏢 **Enterprise / .NET?** → Semantic Kernel — C#/Java/Python, Microsoft ecosystem

> **Learn more | 深入学习**: [AgentWay — Agent Basics](https://agentway.dev/learn/docs/basics) covers the agent loop pattern used by all these frameworks.

### Starter Templates & Boilerplates | 入门模板

Get started quickly with production-ready templates.

使用生产级模板快速起步。

| Project | Stack | Description |
|---|---|---|
| [LangChain Templates](https://github.com/langchain-ai/langchain/tree/master/templates) | Python | Official templates for common agent patterns. |
| [CrewAI Examples](https://github.com/crewAIInc/crewAI-examples) | Python | Multi-agent collaboration examples. |
| [Vercel AI Chatbot](https://github.com/vercel/ai-chatbot) | Next.js | Full-stack chatbot template with streaming. |
| [OpenAI Cookbook](https://github.com/openai/openai-cookbook) | Python/JS | Comprehensive examples for GPT APIs. |
| [Anthropic Cookbook](https://github.com/anthropics/anthropic-cookbook) | Python | Examples for Claude tool use, agents, and more. |
| [Awesome MCP Servers](https://github.com/punkpeye/awesome-mcp-servers) | Various | Curated list of MCP server implementations. |

---

## Stage 2: Tools & Integration | 工具与集成

> Give your agents superpowers. Connect external tools, manage memory, and craft effective prompts.
>
> 赋予你的 Agent 超能力。连接外部工具、管理记忆、设计高效提示词。

### Tool Use & Function Calling | 工具调用

Libraries and patterns for giving agents real-world capabilities.

赋予 Agent 真实世界能力的库和模式。

| Project | Stars | Description |
|---|---|---|
| [Composio](https://github.com/ComposioHQ/composio) | 15k+ | 150+ pre-built tool integrations for agents (GitHub, Slack, etc.). |
| [Browser Use](https://github.com/browser-use/browser-use) | 55k+ | Let agents control web browsers with natural language. |
| [Computer Use (Anthropic)](https://docs.anthropic.com/en/docs/agents-and-tools/computer-use) | — | Official Claude computer use capability for GUI automation. |
| [Crawl4AI](https://github.com/unclecode/crawl4ai) | 40k+ | AI-friendly web crawler and scraper for agent pipelines. |
| [Firecrawl](https://github.com/mendableai/firecrawl) | 30k+ | Turn websites into LLM-ready markdown/structured data. |
| [E2B](https://github.com/e2b-dev/e2b) | 5k+ | Secure cloud sandboxes for AI-generated code execution. |
| [Toolhouse](https://github.com/toolhouseai/toolhouse) | 1k+ | Cloud-based tool infrastructure for agents. |

### MCP Servers & Ecosystem | MCP 服务与生态

Model Context Protocol — the open standard for connecting AI to tools and data.

模型上下文协议 —— 连接 AI 与工具和数据的开放标准。

| Project | Stars | Description |
|---|---|---|
| [MCP Specification](https://github.com/modelcontextprotocol/specification) | 5k+ | The official MCP protocol spec. |
| [MCP Servers (Official)](https://github.com/modelcontextprotocol/servers) | 20k+ | Reference MCP server implementations (filesystem, GitHub, Slack, etc.). |
| [Awesome MCP Servers](https://github.com/punkpeye/awesome-mcp-servers) | 40k+ | Community-curated MCP servers collection. |
| [MCP TypeScript SDK](https://github.com/modelcontextprotocol/typescript-sdk) | 5k+ | Official TypeScript SDK for building MCP servers/clients. |
| [MCP Python SDK](https://github.com/modelcontextprotocol/python-sdk) | 5k+ | Official Python SDK for building MCP servers/clients. |

> **Learn more | 深入学习**: [AgentWay — MCP & Skills](https://agentway.dev/learn/docs/mcp) walks through building your own MCP server from scratch.

### Memory & Context Management | 记忆与上下文管理

Solutions for giving agents persistent memory and context.

赋予 Agent 持久记忆和上下文的方案。

| Project | Stars | Description |
|---|---|---|
| [Mem0](https://github.com/mem0ai/mem0) | 25k+ | Self-improving memory layer for AI agents and assistants. |
| [Letta](https://github.com/letta-ai/letta) | 15k+ | Stateful agents with long-term memory and portable agent format (.af). |
| [Zep](https://github.com/getzep/zep) | 3k+ | Long-term memory for AI assistants and agents. |
| [Memary](https://github.com/kingjulio8238/memary) | 2k+ | Memory architecture for autonomous agents. |
| [Cognee](https://github.com/topoteretes/cognee) | 3k+ | Memory management via knowledge graphs for AI apps. |

> **Learn more | 深入学习**: [AgentWay — Memory](https://agentway.dev/learn/docs/memory) covers context window strategies and session management patterns.

### Prompt Engineering | 提示词工程

Tools and libraries for systematic prompt management.

系统化提示词管理的工具和库。

| Project | Stars | Description |
|---|---|---|
| [DSPy](https://github.com/stanfordnlp/dspy) | 25k+ | Programming (not prompting) LMs — auto-optimizing prompts with compilers. |
| [Promptfoo](https://github.com/promptfoo/promptfoo) | 5k+ | Test, evaluate, and compare LLM prompts systematically. |
| [LMQL](https://github.com/eth-sri/lmql) | 4k+ | Programming language for constrained LLM interaction. |
| [Guidance](https://github.com/guidance-ai/guidance) | 20k+ | Constrained generation and structured output from LLMs. |
| [Instructor](https://github.com/instructor-ai/instructor) | 10k+ | Structured outputs from LLMs using Pydantic models. |
| [Outlines](https://github.com/dottxt-ai/outlines) | 10k+ | Structured text generation with regex/JSON schema constraints. |

> **Learn more | 深入学习**: [AgentWay — Prompts](https://agentway.dev/learn/docs/prompts) teaches prompt design patterns specific to agent systems.

---

## Stage 3: Advanced Patterns | 高级模式

> Design sophisticated agent systems. Multi-agent orchestration, RAG pipelines, and evaluation.
>
> 设计复杂 Agent 系统。多 Agent 编排、RAG 管道和评估体系。

### Multi-Agent Systems | 多 Agent 系统

Frameworks and patterns for coordinating multiple agents.

协调多个 Agent 的框架和模式。

| Project | Stars | Description |
|---|---|---|
| [AutoGen](https://github.com/microsoft/autogen) | 40k+ | Flexible multi-agent conversations with human-in-the-loop. |
| [CrewAI](https://github.com/crewAIInc/crewAI) | 25k+ | Role-based agent teams with delegation and collaboration. |
| [OWL](https://github.com/camel-ai/owl) | 5k+ | GAIA benchmark winner. Browser + terminal + MCP multi-agent. |
| [MetaGPT](https://github.com/geekan/MetaGPT) | 50k+ | Multi-agent framework mimicking a software company structure. |
| [ChatDev](https://github.com/OpenBMB/ChatDev) | 30k+ | Communicative agents simulating a software development company. |
| [OpenClaw](https://openclaw.ai) | — | Persistent agent orchestrator with multi-channel routing. |

> **Learn more | 深入学习**: [AgentWay — Multi-Agent](https://agentway.dev/learn/docs/multi-agent) covers orchestration patterns, delegation, and consensus.

### RAG & Knowledge | RAG 与知识库

Retrieval-Augmented Generation and knowledge management for agents.

Agent 的检索增强生成和知识管理。

| Project | Stars | Description |
|---|---|---|
| [LlamaIndex](https://github.com/run-llama/llama_index) | 40k+ | Data framework for LLM apps — indexing, querying, RAG. |
| [Haystack](https://github.com/deepset-ai/haystack) | 20k+ | End-to-end NLP framework with production RAG pipelines. |
| [RAGFlow](https://github.com/infiniflow/ragflow) | 35k+ | Deep document understanding RAG engine with visual chunking. |
| [Kotaemon](https://github.com/Cinnamon/kotaemon) | 20k+ | Open-source RAG-based document QA tool with clean UI. |
| [GraphRAG](https://github.com/microsoft/graphrag) | 25k+ | Graph-based RAG using knowledge graph extraction from Microsoft. |
| [Chonkie](https://github.com/bhavnicksm/chonkie) | 5k+ | Lightweight, blazing-fast text chunking library for RAG. |
| [Unstructured](https://github.com/Unstructured-IO/unstructured) | 10k+ | ETL for unstructured documents (PDF, images, HTML → LLM-ready). |

> **Learn more | 深入学习**: [AgentWay — Agentic RAG](https://agentway.dev/learn/docs/agentic-rag) teaches how to build agents that reason over retrieved knowledge.

### Evaluation & Testing | 评估与测试

Evaluate agent performance, quality, and safety systematically.

系统化评估 Agent 性能、质量和安全。

| Project | Stars | Description |
|---|---|---|
| [Promptfoo](https://github.com/promptfoo/promptfoo) | 5k+ | LLM evaluation with test cases, assertions, and CI integration. |
| [Ragas](https://github.com/explodinggradients/ragas) | 10k+ | Evaluation framework specifically for RAG pipelines. |
| [DeepEval](https://github.com/confident-ai/deepeval) | 5k+ | Unit testing framework for LLM outputs. |
| [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) | 3k+ | Framework for LLM evaluation from UK AISI. |
| [GAIA Benchmark](https://huggingface.co/spaces/gaia-benchmark/leaderboard) | — | Real-world assistant benchmark for AI agents. |
| [AgentBench](https://github.com/THUDM/AgentBench) | 3k+ | Multi-dimensional benchmark for evaluating LLM-as-Agent. |
| [SWE-bench](https://github.com/princeton-nlp/SWE-bench) | 3k+ | Benchmark for evaluating code-generation agents on real GitHub issues. |

> **Learn more | 深入学习**: [AgentWay — Evaluation](https://agentway.dev/learn/docs/evaluation) covers building evaluation harnesses and systematic testing.

### Coding Agents | 编程 Agent

AI agents that write, review, and debug code.

编写、审查和调试代码的 AI Agent。

| Project | Stars | Description | Pricing |
|---|---|---|---|
| [Claude Code](https://docs.anthropic.com/en/docs/claude-code) | — | Anthropic's agentic coding tool. Terminal-first, deep codebase understanding. **4.02M npm weekly, 24.5x YoY.** | Pay per use |
| [TRAE](https://www.trae.ai) | — | ByteDance's AI coding agent (formerly Marscode). End-to-end AI-native IDE. | Free / Pro |
| [Cursor](https://cursor.com) | — | AI-native IDE with multi-file editing, Chat, and Composer. | Free / $20/mo |
| [Aider](https://github.com/paul-gauthier/aider) | 30k+ | Terminal-first pair programming with git integration. | Free (OSS) |
| [OpenHands](https://github.com/All-Hands-AI/OpenHands) | 50k+ | Open-source AI software developer agent platform. | Free (OSS) |
| [Devin](https://devin.ai) | — | Autonomous AI software engineer by Cognition. | Enterprise |
| [Cline](https://github.com/cline/cline) | 25k+ | Autonomous coding agent for VS Code. | Free (OSS) |
| [Continue](https://github.com/continuedev/continue) | 25k+ | Open-source AI code assistant for VS Code and JetBrains. | Free (OSS) |
| [Windsurf](https://codeium.com/windsurf) | — | AI-native IDE by Codeium with Cascade agentic flow. | Free / $15/mo |
| [Copilot](https://github.com/features/copilot) | — | GitHub's AI pair programmer. Agent mode in VS Code. | Free / $10/mo |

> **Learn more | 深入学习**: [AgentWay — Claude Code Guide](https://agentway.dev/claudecode) covers best practices for working with agentic coding tools.

---

## Stage 4: Production & Operations | 生产部署

> Ship it. Deploy, monitor, secure, and scale your agents in production.
>
> 上线吧。在生产环境中部署、监控、保障和扩展你的 Agent。

### Agent Deployment & Hosting | 部署与托管

Platforms and infrastructure for deploying agents at scale.

大规模部署 Agent 的平台和基础设施。

| Project | Stars | Description |
|---|---|---|
| [Modal](https://modal.com) | — | Serverless cloud for AI/ML workloads. GPU on demand. |
| [E2B](https://github.com/e2b-dev/e2b) | 5k+ | Secure sandboxed environments for running AI-generated code. |
| [Fly.io](https://fly.io) | — | Edge deployment for low-latency agent APIs. |
| [Railway](https://railway.app) | — | One-click deployment for agent backends. |
| [Trigger.dev](https://github.com/triggerdotdev/trigger.dev) | 15k+ | Background jobs and long-running agent tasks. |
| [Inngest](https://github.com/inngest/inngest) | 5k+ | Durable workflow engine for multi-step agent operations. |

### Observability & Monitoring | 可观测与监控

Track agent behavior, costs, and performance in production.

在生产中追踪 Agent 行为、成本和性能。

| Project | Stars | Description |
|---|---|---|
| [Langfuse](https://github.com/langfuse/langfuse) | 10k+ | Open-source observability for LLM apps. Traces, evals, prompt mgmt. |
| [LangSmith](https://smith.langchain.com) | — | LangChain's managed platform for tracing and evaluation. |
| [Arize Phoenix](https://github.com/Arize-ai/phoenix) | 10k+ | Open-source observability for LLM apps with tracing and evals. |
| [Helicone](https://github.com/Helicone/helicone) | 3k+ | Open-source LLM observability with request logging and analytics. |
| [Portkey](https://github.com/Portkey-AI/gateway) | 7k+ | AI gateway with observability, routing, and guardrails. |
| [Opik](https://github.com/comet-ml/opik) | 5k+ | Open-source LLM evaluation and tracing platform. |

### Safety & Guardrails | 安全与护栏

Protect your agents from misuse, hallucination, and security threats.

保护 Agent 免受滥用、幻觉和安全威胁。

| Project | Stars | Description |
|---|---|---|
| [NeMo Guardrails](https://github.com/NVIDIA/NeMo-Guardrails) | 5k+ | NVIDIA's toolkit for adding safety rails to LLM apps. |
| [Guardrails AI](https://github.com/guardrails-ai/guardrails) | 5k+ | Input/output validation framework for LLM applications. |
| [Rebuff](https://github.com/protectai/rebuff) | 1k+ | Prompt injection detection and prevention. |
| [LLM Guard](https://github.com/protectai/llm-guard) | 2k+ | Security toolkit for LLM interactions. |
| [Invariant Analyzer](https://github.com/invariantlabs-ai/invariant) | 1k+ | Static analysis and runtime monitoring for AI agents. |

> **Learn more | 深入学习**: [AgentWay — Agent Security](https://agentway.dev/learn/docs/agent-security) covers red teaming, guardrails, and security patterns for agents.

### LLM Serving & Inference | 模型服务与推理

Self-host and optimize LLM inference for agent workloads.

自托管和优化 Agent 工作负载的大模型推理。

| Project | Stars | Description |
|---|---|---|
| [vLLM](https://github.com/vllm-project/vllm) | 50k+ | High-throughput LLM serving with PagedAttention. `Production` |
| [Ollama](https://github.com/ollama/ollama) | 120k+ | Run LLMs locally with simple CLI. macOS/Windows/Linux. |
| [llama.cpp](https://github.com/ggerganov/llama.cpp) | 80k+ | C++ inference of Meta's LLaMA models. CPU/GPU optimized. |
| [TGI](https://github.com/huggingface/text-generation-inference) | 10k+ | Hugging Face's production-grade LLM serving toolkit. `Production` |
| [SGLang](https://github.com/sgl-project/sglang) | 10k+ | Fast serving framework for LLMs and VLMs. |
| [LocalAI](https://github.com/mudler/LocalAI) | 30k+ | Drop-in OpenAI-compatible local API for running LLMs. |

---

## Learning Resources | 学习资源

> Level up your skills with structured courses, books, and communities.
>
> 通过系统课程、书籍和社区提升技能。

### Structured Courses | 系统课程

| Course | Language | Cost | Highlights |
|---|---|---|---|
| [AgentWay](https://agentway.dev/learn) | EN / 中文 | Freemium | Gamified learning with XP, exercises, capstone projects. 16 paths from basics to production. |
| [DeepLearning.AI — AI Agents](https://www.deeplearning.ai/courses/) | EN | Free | Short courses by Andrew Ng on agent design patterns. |
| [LangChain Academy](https://academy.langchain.com) | EN | Free | Official LangChain/LangGraph courses and certifications. |
| [Hugging Face Agents Course](https://huggingface.co/learn/agents-course) | EN | Free | Community-driven agent development course. |
| [AI Agents in Practice (Packt)](https://github.com/PacktPublishing/AI-Agents-in-Practice) | EN | Paid | Production-focused LangChain/LangGraph guide. |
| [Building Agentic AI Systems (Packt)](https://github.com/PacktPublishing/Building-Agentic-AI-Systems) | EN | Paid | Enterprise agentic systems architecture. |
| [30 Agents Every AI Engineer Must Build](https://github.com/PacktPublishing/30-Agents-Every-AI-Engineer-Must-Build) | EN | Paid | 30 production-ready agent patterns. |

### Tutorials & Guides | 教程与指南

| Resource | Topic | Description |
|---|---|---|
| [AgentWay — Claude Code Guide](https://agentway.dev/claudecode) | Coding Agents | Best practices for Claude Code: CLAUDE.md, hooks, skills, MCP. |
| [AgentWay — OpenClaw Guide](https://agentway.dev/openclaw) | Agent Orchestration | Getting started with OpenClaw multi-agent orchestration. |
| [Anthropic Agent Documentation](https://docs.anthropic.com/en/docs/agents-and-tools) | Agent Fundamentals | Official guide to building agents with Claude. |
| [OpenAI Agent Guide](https://platform.openai.com/docs/guides/agents) | Agent Fundamentals | Official guide to building agents with GPT models. |
| [Google Agent Development](https://ai.google.dev/gemini-api/docs/agentic) | Agent Fundamentals | Building agents with Gemini and Google ADK. |
| [LangGraph Tutorials](https://langchain-ai.github.io/langgraph/tutorials/) | Frameworks | Step-by-step LangGraph agent tutorials. |

### Books | 书籍

| Book | Author | Year | Focus |
|---|---|---|---|
| *Building LLM Powered Applications* | Valentina Alto | 2024 | End-to-end LLM app development. |
| *AI Engineering* | Chip Huyen | 2025 | Production AI systems design. |
| *Prompt Engineering for Generative AI* | James Phoenix, Mike Taylor | 2024 | Systematic prompt engineering. |
| *Designing Autonomous AI* | Kailash Nadh | 2025 | Agent architecture patterns. |
| *LLMs in Production* | Various | 2024 | Deploying LLMs at scale. |

### Podcasts & Videos | 播客与视频

| Resource | Format | Description |
|---|---|---|
| [Latent Space](https://www.latent.space/podcast) | Podcast | AI engineering interviews and deep dives. |
| [The AI Engineering Podcast](https://www.aiengineering.fm/) | Podcast | Focused on building production AI systems. |
| [AI Jason](https://www.youtube.com/@AIJasonZ) | YouTube | Agent tutorials and framework comparisons. |
| [Matt Shumer](https://www.youtube.com/@MattShumer) | YouTube | Agent design and multi-agent patterns. |
| [Dave Ebbelaar](https://www.youtube.com/@daveebbelaar) | YouTube | LangChain/LangGraph practical tutorials. |

### Newsletters | 订阅通讯

| Newsletter | Frequency | Focus |
|---|---|---|
| [The Batch](https://www.deeplearning.ai/the-batch/) | Weekly | AI news by Andrew Ng / DeepLearning.AI. |
| [Ahead of AI](https://magazine.sebastianraschka.com/) | Bi-weekly | Research-focused AI engineering by Sebastian Raschka. |
| [AI Engineering](https://aiengineering.substack.com/) | Weekly | Practical AI engineering tips and tutorials. |
| [Latent Space](https://www.latent.space/) | Weekly | AI engineering community newsletter. |

---

## Career & Jobs | 职业发展

> Turn your agent skills into a career. Explore roles, prep for interviews, and build your portfolio.
>
> 将 Agent 技能转化为职业优势。探索岗位、准备面试、构建作品集。

### Top Companies Are Hiring — Agent Is Real | 头部团队正在大规模招聘 —— Agent 不是概念

More and more top tech companies are putting Agent into real engineering requirements. Here's what the hiring landscape looks like in March 2026:

越来越多头部团队已经把 Agent 放进真实工程需求里。以下是 2026 年 3 月的招聘实况：

#### ByteDance | 字节跳动 — 18 Agent Positions

ByteDance has **18 core Agent positions** across 5+ product lines, spanning tech R&D, product design, algorithms, and business strategy. Key product lines hiring:

字节跳动开放了 **18 个 Agent 核心岗位**，覆盖技术研发、产品设计、算法优化、商业分析等多个维度：

| Product Line | Example Roles | Focus |
|---|---|---|
| **TRAE** (端到端 AI 编程) | Agent 框架优化专家, AI Coding 产品经理, 战略商业分析师 | AI coding agent, 月活超100万 |
| **火山引擎** | HiAgent 交付专家 | 企业级 Agent 平台 |
| **剪映 CapCut** | 高级 AI Agent 开发工程师, 移动端研发工程师(即梦AI) | 视频创作 + AIGC |
| **生活服务** | AI 应用开发工程师 | 游玩助手 Agent（Prompt/RAG/MCP） |
| **TikTok Shop** | 资深前端研发工程师(AI方向) | 国际电商 + AIGC |
| **Seed 研究院** | 大语言模型 AI 搜索 Agent 算法工程师 | 前沿 AI 研究 |
| **开发者服务** | Dev Agent 后端开发, AI Agent 研发实习生 | 研发工具全链路 |

> Data source: [jobs.bytedance.com](https://jobs.bytedance.com) — [Full report | 完整报告](https://youmind.com/s/ao2k8w2erLeFpZ)

#### Tencent | 腾讯 — 6 Pages of Agent Positions

Tencent's careers page returns **6 full pages** of Agent-related positions, spanning domestic (Beijing, Shanghai, Guangzhou, Shenzhen, Chengdu) and overseas (Palo Alto, Bellevue). Key directions:

腾讯招聘官网搜索 "Agent" 返回**满满当当6页岗位**，覆盖国内北上广深成都及海外硅谷：

| Direction | Example Roles | Salary Range |
|---|---|---|
| **Coding Agent** (北美) | Sr. AI Software Engineer – Coding Agent | $116K - $269K/yr |
| **企业微信 Agent** | 深度学习算法工程师 - Agent 应用 | 30K-60K/月 |
| **AI 搜索 Agent** | 大模型算法研究员（Agent 方向） | 30K-80K/月 |
| **多模态 Agent** | 多模态大模型算法研究员 | 50K-80K/月 |

> Data source: [careers.tencent.com](https://careers.tencent.com) — [Full report | 完整报告](https://youmind.com/s/6T00tMDDGETWef)

#### What This Tells Us | 这说明什么

The hiring data from ByteDance and Tencent reveals **which skills matter most** in real Agent engineering jobs:

字节和腾讯的招聘数据揭示了 Agent 工程岗位**真正需要的技能**：

1. **Agent framework design** (框架设计) — Tooling, Memory, Planning, Workflow orchestration
2. **LLM engineering** (大模型工程化) — Prompt engineering, RAG, fine-tuning, multi-model support
3. **Production engineering** (生产工程) — High availability, observability, cost control, MCP protocol
4. **Cross-domain skills** (跨领域能力) — Business understanding + technical depth

> **These skills map directly to our 4-stage learning path** — and to the [AgentWay curriculum](https://agentway.dev/zh) that covers 90% of the skills required by top-tier Agent positions.
>
> **这些技能直接对应我们的4阶段学习路径** —— 以及涵盖头部团队 Agent 应用开放岗位90%技能需求的 [AgentWay 大纲](https://agentway.dev/zh)。

### In-Demand Roles | 热门岗位

The agent economy is creating new roles. Here are the most in-demand positions in 2026:

Agent 经济正在创造新的岗位。以下是 2026 年最热门的职位：

| Role | Salary Range (USD) | Core Skills | Learning Path |
|---|---|---|---|
| **AI Agent Engineer** | $150k - $250k | Agent frameworks, MCP, tool integration, prompt eng | [AgentWay Track 1-3](https://agentway.dev/learn) |
| **Agent Platform Engineer** | $160k - $280k | Infrastructure, deployment, scaling, monitoring | [Stage 4 resources](#stage-4-production--operations--生产部署) |
| **AI Security Engineer** | $180k - $300k | Red teaming, guardrails, prompt injection defense | [AgentWay — Agent Security](https://agentway.dev/learn/docs/agent-security) |
| **RAG Engineer** | $140k - $240k | Vector DBs, chunking, retrieval, knowledge graphs | [AgentWay — Agentic RAG](https://agentway.dev/learn/docs/agentic-rag) |
| **Multi-Agent Architect** | $180k - $320k | Orchestration, delegation, consensus, workflows | [AgentWay — Multi-Agent](https://agentway.dev/learn/docs/multi-agent) |
| **LLM Ops / MLOps** | $150k - $260k | Model serving, inference optimization, cost mgmt | [Stage 4 resources](#stage-4-production--operations--生产部署) |
| **AI Product Manager** | $140k - $250k | Agent UX, product strategy, evaluation metrics | Cross-cutting skills |

### Job Boards | 招聘平台

| Platform | Focus | Region |
|---|---|---|
| [ByteDance Agent Jobs](https://jobs.bytedance.com) | 18+ Agent roles across TRAE/CapCut/TikTok | China / Global |
| [Tencent Agent Jobs](https://careers.tencent.com/search.html?keyword=agent) | 6 pages of Agent positions | China / US |
| [AI Jobs](https://aijobs.net) | AI/ML roles | Global |
| [MLOps Jobs](https://mlops.jobs) | MLOps & AI Eng | Global |
| [Wellfound (AngelList)](https://wellfound.com) | Startup AI roles | Global |
| [Y Combinator Work at a Startup](https://www.ycombinator.com/jobs) | YC company roles | US-focused |
| [RemoteOK](https://remoteok.com/remote-ai-jobs) | Remote AI roles | Global |
| [AI 研习社招聘](https://job.yanxishe.com) | AI 岗位 | 中国 |
| [Boss 直聘](https://www.zhipin.com) | 全品类 | 中国 |
| [牛客网](https://www.nowcoder.com/recommend) | 技术岗位 + 面试 | 中国 |

### Interview Prep | 面试准备

Common interview topics for AI Agent roles:

AI Agent 岗位常见面试主题：

**System Design | 系统设计**
- Design an agent that can browse the web and answer research questions
- Design a multi-agent code review system
- Design a RAG pipeline with 10M documents
- Design an agent monitoring and alerting system

**Technical Deep-Dives | 技术深度**
- How does the ReAct (Reason + Act) pattern work?
- Compare agent memory strategies: buffer, summary, vector, knowledge graph
- How do you evaluate agent quality without ground truth?
- Explain the MCP protocol and when to use it vs direct function calling

**Behavioral | 行为面试**
- Describe a time you debugged an agent that was hallucinating
- How do you handle a situation where the agent's cost is too high?
- How would you roll out an agent feature with safety in mind?

### Portfolio Projects | 作品集项目

Build these projects to demonstrate your agent engineering skills:

构建这些项目来展示你的 Agent 工程能力：

| Project | Difficulty | Skills Demonstrated |
|---|---|---|
| CLI Agent with tool use | Beginner | Agent loop, function calling, structured output |
| MCP Server for a SaaS API | Intermediate | MCP protocol, tool design, error handling |
| RAG chatbot over your docs | Intermediate | Chunking, embedding, retrieval, generation |
| Multi-agent research assistant | Advanced | Orchestration, delegation, synthesis |
| Agent eval harness | Advanced | Testing frameworks, metrics, CI integration |
| Production agent with monitoring | Advanced | Deployment, observability, guardrails, cost control |

> **Hands-on practice | 动手实践**: [AgentWay Exercises & Capstones](https://agentway.dev/learn) provide guided agent projects with automated grading.

---

## Community | 社区

> Connect with other agent builders. Share, learn, and collaborate.
>
> 与其他 Agent 开发者连接。分享、学习、协作。

### Discord & Slack Communities | Discord 与 Slack 社区

| Community | Platform | Focus | Members |
|---|---|---|---|
| [LangChain Discord](https://discord.gg/langchain) | Discord | LangChain/LangGraph ecosystem | 50k+ |
| [Anthropic Discord](https://discord.gg/anthropic) | Discord | Claude, agent development | 30k+ |
| [OpenAI Discord](https://discord.gg/openai) | Discord | GPT, assistants, agents | 100k+ |
| [Hugging Face Discord](https://discord.gg/huggingface) | Discord | Open-source AI/ML | 50k+ |
| [AgentWay Discord](https://discord.gg/agentway) | Discord | Agent learning community | Growing |
| [MLOps Community](https://mlops.community) | Slack | MLOps, AI engineering | 20k+ |
| [AI Engineer Foundation](https://discord.gg/ai-engineer) | Discord | AI engineering practice | 10k+ |

### Conferences & Meetups | 会议与活动

| Event | When | Where | Focus |
|---|---|---|---|
| [AI Engineer Summit](https://www.ai.engineer/) | Annual | SF / Virtual | AI engineering practice |
| [NeurIPS](https://neurips.cc) | Dec | Annual | ML research including agents |
| [LangChain Days](https://www.langchain.com/events) | Quarterly | Virtual | LangChain ecosystem |
| [AgentCon](https://agentcon.ai) | Annual | SF | Agent-focused conference |

### Chinese Community | 中文社区

| 社区 | 平台 | 专注领域 |
|---|---|---|
| [AI 研习社](https://www.yanxishe.com) | Web | AI 技术学习与交流 |
| [机器之心](https://www.jiqizhixin.com) | Web / 公众号 | AI 新闻与深度报道 |
| [量子位](https://www.qbitai.com) | Web / 公众号 | AI 产业与技术 |
| [掘金 AI 板块](https://juejin.cn/tag/AI) | Web | 开发者技术社区 |
| [V2EX AI 节点](https://www.v2ex.com/go/ai) | Web | 开发者讨论 |
| [知乎 AI Agent 话题](https://www.zhihu.com/topic/27361817) | Web | 深度问答 |

---

## Contributing | 贡献指南

We welcome contributions! Please read our [Contributing Guide](CONTRIBUTING.md) before submitting a PR.

欢迎贡献！提交 PR 前请阅读我们的[贡献指南](CONTRIBUTING.md)。

Ways to contribute | 贡献方式:
- Add a new project or resource | 添加新项目或资源
- Update outdated information | 更新过时信息
- Improve descriptions or translations | 改善描述或翻译
- Fix broken links | 修复失效链接
- Suggest new categories | 建议新分类

---

## License | 许可

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, the curators have waived all copyright and related rights to this work.

在法律允许的范围内，策划者已放弃本作品的所有版权和相关权利。
