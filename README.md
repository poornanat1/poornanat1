# Poorna Natarajan

I work on the engineering around language models: retrieval, evaluation, agents, structured extraction, and the deterministic systems that make probabilistic models reliable in production.

Currently a Senior Machine Learning Engineer at Latham & Watkins.

My background is in full-stack ML engineering, with a focus on ranking, retrieval, and traditional ML.

## Selected Projects

### [PodFind](https://github.com/poornanat1/podcast-retrieval) · _in progress_

Self-hosted podcast search and recommendation over a real catalog of ~800k episodes, with RSS and transcript ingestion in Go, the ML lifecycle in Python, and PostgreSQL + pgvector for storage and ANN search.

- Hybrid lexical + vector retrieval with a learned reranker and hard structured filters
- Two-tower models for personalized and "more like this" recommendations
- Voice queries parsed into intent and filters, and evaluated as part of retrieval quality
- Offline evaluation against a human-auditable relevance set, with versioned, reproducible data and models

[Source](https://github.com/poornanat1/podcast-retrieval)

### [CareNav](https://github.com/poornanat1/carenav)

A source-grounded healthcare navigator designed around a simple constraint: when the evidence is insufficient, the system should escalate rather than guess.

- Hybrid retrieval with Postgres FTS + pgvector and citation-grounded responses
- Typed pipeline separating retrieval, intent, tool execution, generation, and verification
- PII tokenization before model calls and cost-aware model routing
- Evaluation suite gating retrieval quality, grounding, and safety regressions in CI

[Source](https://github.com/poornanat1/carenav) · [Live Demo](https://carenav-frontend-production.up.railway.app/)

### [DSpyNet](https://github.com/al322se/DSpyNet)

Open-source contributions to a C#/.NET port of Stanford DSPy.

- Implemented the GEPA reflective prompt optimizer
- Added compatibility fixes aligning behavior with upstream DSPy
- Worked across optimization, evaluation, and typed .NET abstractions

[GEPA PR](https://github.com/al322se/DSpyNet/pull/1) · [Compatibility PR](https://github.com/al322se/DSpyNet/pull/2) · [NuGet](https://www.nuget.org/packages/DSpyNet)

### [Audition With Me](https://github.com/cranberrymuffin/auditionwithme)

A rehearsal app for actors that turns scripts into interactive scenes with AI voice scene partners.

- Built the guided rehearsal flow with role selection, voice casting, live speech tracking, and teleprompter playback
- Developed layered parsing for typed, scanned, bilingual, and annotated PDFs
- Added AI-directed ElevenLabs audio with contextual delivery, caching, and persisted casting
- Reworked the visual design and tightened up responsive layouts, accessibility, and auth

[Source](https://github.com/cranberrymuffin/auditionwithme) · [Live Demo](https://auditionwithme.com)

## Stack

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![C#](https://img.shields.io/badge/C%23-512BD4?style=flat-square&logo=dotnet&logoColor=white) ![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white) ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white) ![pgvector](https://img.shields.io/badge/pgvector-4169E1?style=flat-square&logo=postgresql&logoColor=white) ![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white) ![OpenShift](https://img.shields.io/badge/OpenShift-EE0000?style=flat-square&logo=redhatopenshift&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![Airflow](https://img.shields.io/badge/Airflow-017CEE?style=flat-square&logo=apacheairflow&logoColor=white)
