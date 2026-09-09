# Systems and Capabilities

> **Ariamir is unfinished and in active development.** Many functions need intensive QA, end-to-end validation and polish. This catalog describes development scope and user-facing behaviour; it does not certify stability, security, performance or production readiness.

The systems below have functionality in development builds unless explicitly marked as exploration or future work. Individual workflows can be incomplete, configuration-dependent or limited to particular environments. Public demonstrations and measured results will be published separately when suitable for release.

## Fabric and workers

Fabric coordinates tasks across models, workers and tools. Workers handle bounded responsibilities within broader workflows, while task tracking makes progress and interruptions visible. Development continues on coordination, recovery, concurrency and behaviour across system boundaries.

The development interface supports modular configuration: describing a responsibility, selecting capability areas, choosing automatic or manual model selection and adjusting worker instances. These controls describe configuration choices, not guaranteed performance or complete coverage of every combination. See the [Fabric WIP screenshots](../README.md#inside-ariamir--work-in-progress).

Private routing criteria, worker prompts and orchestration implementation are outside this showcase.

## Local models and hardware-aware execution

Ariamir works with local model backends and different model sizes. Model management covers available models, loading and unloading, context limits and observation of CPU, GPU and memory resources. Workload suitability depends on the actual model, backend and machine; estimates and measurements must remain distinct.

Multi-model operation, resource pressure and recovery paths remain areas for QA. This is not a claim of universal model or accelerator compatibility.

## Knowledge

Knowledge organizes durable project information: notes, sources, decisions and relationships. It includes editable Markdown notes, search and retrieval, project knowledge profiles, import/export and work on synchronization and federated views.

Source context and traceability help users assess retrieved material. Contradictions, uncertain relationships and stale knowledge require review rather than being silently treated as settled facts. See [the Knowledge overview](knowledge.md).

## Graph Workspace

Graph Workspace is the visual environment for connected information. Users can explore relationships, filter the graph, inspect nodes and sources, and save useful views. Work also includes optional views of Fabric activity, tasks and code alongside Knowledge.

A visualization is not evidence that a relationship is true. Inferred relationships and other system views need to remain distinguishable from authored knowledge. Accessibility, large-graph usability, interaction and cross-system behaviour need continued validation.

## Knowledge Learning

Knowledge Learning develops a reviewable path from selected observations and task outcomes to proposed knowledge updates. Its scope includes learning proposals, feedback, consolidation suggestions and knowledge-health review.

Learning here refers to improving managed project knowledge; it does not imply retraining a base model or guaranteed autonomous self-improvement. Generated answers, repetition and retrieval frequency do not establish factual correctness. Proposal quality, provenance and review behaviour remain QA priorities.

## Memory

Memory supports conversational continuity and user preferences. It is separate from project Knowledge so that a personal preference, a project decision and a sourced claim are not treated as interchangeable information.

Development work includes relevance, correction, forgetting and consistent separation between memory and knowledge. Personal memories and user content are not public showcase material.

## Document Engine and visual artifacts

The Document Engine reads and analyses documents and produces structured outputs such as reports and PDFs. Work includes source retention, long-document continuity, tables, charts, images and layout review. Generated artifacts can be organized and inspected within project workflows.

Document fidelity, factual grounding, pagination and visual quality still require intensive QA and polish. Support depends on the format and workflow; a readable input format does not imply equivalent editable output support. Public examples must use synthetic or redistributable material.

## Code Intelligence

Code Intelligence supports code exploration, symbol and reference discovery, change-impact analysis, diagnostics and focused context retrieval. Editing workflows include previews, verification and reversible changes where supported. Optional language-service integration extends some workflows.

Language coverage, diagnostics, multi-file changes and recovery need continued validation. A generated edit or proposed test plan is not proof that a change is correct.

## Tool Lab and modules

Tool Lab manages optional tool capabilities and their dependencies. Module work covers discovery, installation, validation, promotion, updates and rollback, with capability and permission information presented to the user.

The module ecosystem is still being integrated and tested. A catalog entry does not mean a package is installed, enabled, independently verified or compatible with every environment. Private manifests, dependency environments and implementation code are not published here.

## Browser and desktop tools

Ariamir is developing observation and supervised interaction for supported browser and desktop environments. This includes working with page or application state and reviewable file-transfer workflows.

Coverage depends on the application, adapter and environment. Vision-based behaviour, complex interactions and failure recovery require intensive QA. These capabilities should not be read as universal or fully reliable computer control.

## Bridge / MCP and connectors

Bridge / MCP allows compatible clients to access Ariamir's permitted capabilities and work with tracked jobs. Connector and account management integrates selected external services when the relevant provider, account and permissions are configured.

Connector maturity varies. Listed, configured, connected and operational are different states; this showcase does not claim that every listed service works end to end. Credentials, account details and private service configuration remain private.

## Projects, tasks and artifacts

The workspace groups conversations, tasks, attached material and generated files around projects. Development includes progress visibility, resumable work and artifact management.

Task recovery, cancellation, concurrent activity and consistency between the interface and actual execution state are ongoing QA areas. A displayed action must not be confused with a verified outcome.

## Permissions and operational review

Cross-system work includes permissioned actions, previews, reviewable outcomes and verification or rollback where supported. These are product behaviours under development, not security certifications or guarantees that every operation can be reversed.

Private permission rules, security implementation and production configuration are deliberately omitted. Public demonstrations should show observable behaviour using non-sensitive examples.

## Local diagnostics

Diagnostic tools inspect system health and storage and support bounded maintenance workflows with review and verification. Maintenance coverage is limited and remains under QA; Ariamir is not presented as a general autonomous system administrator.

## Desktop application and distribution

The Windows desktop application brings the workspace and system controls together. Distribution work includes installation, launching, updates, repair and recovery while preserving user state.

Packaging, upgrade paths, interface consistency, accessibility and performance still need validation and polish. This documentation repository does not provide a finished installer or guarantee a stable public release.

## Local image and video

Image workflows exist in development builds. Local video work remains in integration and validation. Backend availability, model licensing, memory requirements and output quality vary by workflow.

Public demos and performance claims require suitable licensing and measured evidence. The showcase does not imply that both media paths are complete or equally mature.

## Hardware Compatibility Lab and heterogeneous acceleration

The lab evaluates practical compatibility, latency, memory pressure and workload suitability on real hardware. Public benchmark methodology and published measurements are kept separate.

FPGA and other accelerator work is exploratory and includes partner-validation opportunities. It should not be interpreted as a completed general-purpose acceleration backend. See [the Hardware Compatibility Lab](hardware-lab.md).

## Enterprise environment

**Research / architecture exploration.** Ariamir is exploring a specialized environment for business and professional use, including controlled deployments, organizational security, permission governance, auditability, infrastructure integration, multi-user workflows and scalable heterogeneous compute.

These are exploration goals. There is no claim here of a finished Enterprise edition, enterprise readiness, certified compliance or validated organizational scalability.

## Android portability

**Architecture / future work.** A mobile execution environment and portable capabilities are areas of exploration. Android-specific runtimes, providers and device integration require separate development and validation. This is not an announcement of a completed Android app.
