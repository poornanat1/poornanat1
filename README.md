<h1 align="center">Poorna Natarajan</h1>

<p align="center">
  <em>Working on LLM applications, retrieval, and prompt optimization.</em>
</p>

<br/>

A few things I've built recently. CareNav is a retrieval-grounded agent with real eval gates; dspynet-gepa-bench measures whether automated prompt optimization actually helps; and I contributed the GEPA optimizer to DSpyNet.

<br/>

### CareNav

A health-benefits navigator. Every answer is grounded in a cited source, and anything unsafe or unanswerable escalates to a human instead of guessing.

A typed Python orchestrator routes each turn: *safety → intent → specialist tools → grounded answer → verify → respond or escalate.* Hybrid Postgres retrieval (pgvector + full-text), cost-aware model tiering, PII tokenized before every model call, and eval gates that fail CI on a missed escalation or a leak.

<p>
  <img alt="Python" src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white">
  <img alt="FastAPI" src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white">
  <img alt="Postgres + pgvector" src="https://img.shields.io/badge/Postgres_+_pgvector-4169E1?style=flat-square&logo=postgresql&logoColor=white">
  <img alt="Mistral" src="https://img.shields.io/badge/Mistral-FF7000?style=flat-square&logo=mistralai&logoColor=white">
  <img alt="React" src="https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black">
  <img alt="Grafana" src="https://img.shields.io/badge/Telemetry-F46800?style=flat-square&logo=grafana&logoColor=white">
  <img alt="Synthetic data only" src="https://img.shields.io/badge/Synthetic_data_only-475569?style=flat-square&labelColor=0f172a">
</p>

&nbsp;&nbsp;→ [repo](https://github.com/poornanat1/carenav) &nbsp;·&nbsp; [live demo](https://carenav-frontend-production.up.railway.app/) &nbsp;·&nbsp; [telemetry](https://grafana-production-ec8a.up.railway.app/d/carenav-turns/carenav-turn-telemetry)

<br/>

### dspynet-gepa-bench

A benchmark of GEPA reflective prompt evolution on SEC S-1 extraction ([RealKIE](https://arxiv.org/abs/2403.20101)), measuring how much it beats a plain baseline: six `(task, reflection)` model combos per provider, Anthropic and Mistral. Weak task models get the biggest lift from a strong reflector.

| Task LM | Reflect LM | Baseline | GEPA | Δ |
|---|---|---:|---:|---:|
| Haiku 4.5 | Sonnet 4.6 | 0.386 | 0.622 | **+23.6 pp** |
| Opus 4.7 | Opus 4.7 | 0.641 | 0.703 | +6.2 pp |

<p>
  <img alt="C#" src="https://img.shields.io/badge/C%23-512BD4?style=flat-square&logo=dotnet&logoColor=white">
  <img alt=".NET" src="https://img.shields.io/badge/.NET-512BD4?style=flat-square&logo=dotnet&logoColor=white">
  <img alt="Anthropic" src="https://img.shields.io/badge/Anthropic-D97757?style=flat-square&logo=anthropic&logoColor=white">
  <img alt="Mistral" src="https://img.shields.io/badge/Mistral-FF7000?style=flat-square&logo=mistralai&logoColor=white">
</p>

&nbsp;&nbsp;→ [repo](https://github.com/poornanat1/dspynet-gepa-bench)

<br/>

### DSpyNet

**Contributor** to the C# .NET port of Stanford's [DSPy](https://github.com/stanfordnlp/dspy): program language models instead of prompting them. I added the GEPA reflective-prompt-evolution optimizer in [PR #1](https://github.com/al322se/DSpyNet/pull/1) and tightened its parity with upstream DSPy in [PR #2](https://github.com/al322se/DSpyNet/pull/2) (both merged): the same GEPA optimizer my benchmark puts to the test.

<p>
  <img alt="C#" src="https://img.shields.io/badge/C%23-512BD4?style=flat-square&logo=dotnet&logoColor=white">
  <img alt=".NET" src="https://img.shields.io/badge/.NET-512BD4?style=flat-square&logo=dotnet&logoColor=white">
  <img alt="Semantic Kernel" src="https://img.shields.io/badge/Semantic_Kernel-0078D4?style=flat-square&logo=microsoft&logoColor=white">
  <a href="https://www.nuget.org/packages/DSpyNet"><img alt="NuGet" src="https://img.shields.io/nuget/v/DSpyNet?style=flat-square&logo=nuget&logoColor=white&label=NuGet"></a>
</p>

&nbsp;&nbsp;→ [repo](https://github.com/al322se/DSpyNet)

<br/>

<p align="center">
  <img alt="Python" src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white">
  <img alt="C#" src="https://img.shields.io/badge/C%23-512BD4?style=flat-square&logo=dotnet&logoColor=white">
  <img alt="TypeScript" src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white">
  <img alt="FastAPI" src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white">
  <img alt="Postgres" src="https://img.shields.io/badge/Postgres-4169E1?style=flat-square&logo=postgresql&logoColor=white">
  <img alt="Claude" src="https://img.shields.io/badge/Claude-D97757?style=flat-square&logo=anthropic&logoColor=white">
  <img alt="Mistral" src="https://img.shields.io/badge/Mistral-FF7000?style=flat-square&logo=mistralai&logoColor=white">
</p>
