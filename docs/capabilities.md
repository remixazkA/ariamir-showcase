# Capabilities

This page describes Ariamir at a product-capability level. It intentionally avoids internal algorithms, private prompts and implementation-specific routing logic.

## Fabric

Fabric is Ariamir's coordination layer. Publicly, its role can be described as receiving a task and coordinating the model, worker, tool and runtime resources needed to complete it.

Not public: scoring rules, routing heuristics, fallback policies, private schemas, internal prompts or implementation source.

## Local model orchestration

Ariamir is designed to operate with multiple local model backends and model sizes. The goal is to match workload characteristics to available compute rather than assume one model is optimal for every task.

## Workers

Workers are bounded task executors used to divide larger workflows into understandable units of work. Public examples may show roles such as research, document generation, validation or media processing; production worker source and private prompts remain internal.

## Tools and permissions

Ariamir exposes capabilities through tools and permission boundaries. Public materials describe the categories of operations and their observable results, not the internal policy implementation.

## Retrieval and RAG

Retrieval workflows allow Ariamir to work against local or connected information sources. Public demos should use sanitized or synthetic datasets unless the underlying material is already public and redistribution is permitted.

## Document Engine

The Document Engine focuses on turning structured AI work into usable artifacts and on analysing document content. Public benchmarks should measure fidelity and utility rather than disclose private templates or hidden processing logic.

## Local image and video

Ariamir includes local media-generation work. Image workflows are available in development builds; local video generation is in integration and validation. Public demos should identify the model/backend used when licensing permits and should avoid implying performance figures that have not been measured.

## Hardware-aware execution

Ariamir is developed on constrained local hardware, making VRAM, RAM, latency and thermal behaviour first-class engineering concerns. The Hardware Compatibility Lab records how workloads behave on actual systems.

## Heterogeneous acceleration

CPU and GPU are not assumed to be the only useful execution resources. FPGA and other accelerator evaluation focuses on workload classes where deterministic pipelines, streaming, specialised kernels or low-latency processing can provide value.

## Enterprise environment

**Status: Research / architecture exploration.**

Ariamir is exploring a specialized environment for business and professional use cases. Areas under consideration include controlled organizational deployments, organizational security, permission governance, auditable workflows, enterprise infrastructure integration, multi-user workflows and scalable heterogeneous compute.

These are exploration goals, not claims of an available Enterprise edition or validated enterprise capabilities. Public updates will describe scope and validation outcomes without exposing private deployment configuration, permission internals, customer data or proprietary implementation details.
