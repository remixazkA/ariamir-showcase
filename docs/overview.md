# Overview

> **Ariamir is unfinished and under active development.** Many functions require intensive QA, end-to-end validation and polish. This showcase is not a declaration of product readiness.

Ariamir is a local-first AI systems project built around orchestration rather than a single monolithic model. Its public product concept is a coordination layer that can combine local models, bounded workers, tools, retrieval, document processing and hardware resources behind one user-facing system.

## Connected systems

The project includes Fabric and workers, local model management, Knowledge, Graph Workspace, Knowledge Learning, conversational Memory, Document Engine, Code Intelligence, Tool Lab and modules, browser and desktop tools, Bridge / MCP, connectors, projects and artifacts, local diagnostics, and desktop distribution.

Hardware validation and local media workflows are also active work areas. Enterprise deployment, Android portability and FPGA acceleration have exploratory components and should not be confused with finished editions or completed platform support.

See the [system catalog](capabilities.md) and [Knowledge overview](knowledge.md) for scope and limitations.

## Design goals

1. **Local-first execution** — use local compute where it is practical and valuable.
2. **Model plurality** — allow different models to serve different workload classes.
3. **Bounded workers** — decompose complex work into explicit responsibilities.
4. **Permissioned tools** — make external effects intentional and reviewable.
5. **Document-native workflows** — retrieve, analyse and produce useful artifacts rather than only chat text.
6. **Hardware awareness** — evaluate performance against real CPU, GPU, memory and accelerator constraints.
7. **Maintainability** — keep interfaces modular enough to evolve models and backends over time.

## What this repository documents

This repository exists to provide a verifiable public surface for the project: current scope, high-level architecture, development activity, sanitized media, compatibility testing and benchmark methodology.

Proprietary implementation is not published. Suitable demonstration evidence can include reproducible outputs, sanitized screenshots, videos, benchmark runs and compatibility reports. Much of that public evidence is still pending; capability descriptions and methodology alone do not establish reliability or measured performance.

## Intended audiences

- Hardware vendors evaluating sponsorship or engineering collaboration.
- Developers and technical reviewers assessing project seriousness.
- Prospective users following Ariamir's capabilities and roadmap.
- Partners interested in validating components against local AI workloads.
