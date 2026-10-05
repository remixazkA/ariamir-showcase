# Systems and Capabilities

> **Ariamir is unfinished and in active development.** Many functions need intensive QA, end-to-end validation and polish. This catalog describes development scope and user-facing behaviour; it does not certify stability, security, performance or production readiness.

**0.19 development line · Reviewed 5 October 2026.** The systems below have functionality in development builds unless marked as exploration or future work. Availability depends on the build, configuration and workflow. Ariamir's modular transformation is at M7, with validation still open; the [current status](current-status.md) distinguishes implemented work from completed acceptance.

## Business modules and the 0.19 transformation

**Implemented in 0.19 candidates; transformation and integration in progress.** Business modules can provide focused workspace views and project data, with controlled access, supported service integrations and module diagnostics. Lifecycle work covers installation, updates, backup participation and retirement with data-preservation or export options.

The transformation builds on this foundation to make capabilities more consistent to develop and maintain. Runtime and SDK work has implementation and technical evidence; this is not an announcement of a public SDK release or a completed migration. M7 is validating a representative capability, and its latest records retain an incomplete attempt and open prerequisite validation.

The intended result is a clearer extension path and better-tested continuity as capabilities evolve. Actual availability and acceptance must be assessed per module and deployment.

## Human Assistant Loop

**Implemented in the candidate; end-to-end validation ongoing.** Ariamir separates answering a question, proposing a next step and carrying out an explicitly requested operation. The assistant inbox lets a person accept, correct, reject, dismiss or let a proposal expire. Accepting a proposal creates a plan awaiting authorization; it does not perform the proposed action.

Observations require consent with scope, purpose and validity. Revoking consent purges the observed material. Repeated corrections or rejections can suggest preferences, which require human review before activation. This is reviewable workflow assistance, not continuous desktop recording or base-model retraining. Proposal quality, evidence availability and workplace deployment remain validation and review areas.

## Resource governance

**Implemented for supported Knowledge and workspace operations; integration QA ongoing.** Users can review supported changes, inspect operation history and identify conflicts or unauthorized actions. This scope does not imply enterprise certification, universal rollback or control over every external application that can modify a file.

## Fabric and workers

Fabric coordinates tasks across models, workers and tools. Workers handle bounded responsibilities within broader workflows, while task tracking makes progress and interruptions visible. Development continues on coordination, recovery, concurrency and behaviour across system boundaries.

The development interface supports modular configuration: describing a responsibility, selecting capability areas, choosing automatic or manual model selection and adjusting worker instances. These controls describe configuration choices, not guaranteed performance or complete coverage of every combination. See the [Fabric WIP screenshots](../README.md#inside-ariamir--work-in-progress).

Private routing criteria, worker prompts and orchestration implementation are outside this showcase.

## Local models and hardware-aware execution

Ariamir works with local model backends and different model sizes. Model management covers available models, loading and unloading, context limits and observation of CPU, GPU and memory resources. Workload suitability depends on the actual model, backend and machine; estimates and measurements must remain distinct.

Multi-model operation, resource pressure and recovery paths remain areas for QA. This is not a claim of universal model or accelerator compatibility.

**Optional cloud models are implemented in development builds.** Remote inference requires explicit model selection and data-transfer consent, with configured usage limits. It may transfer data and incur provider charges. End-to-end provider validation remains separate from configuration support.

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

Ariamir implements observation and supervised interaction for supported browser and Windows desktop environments, including page or application state, reviewable file transfers and action evidence. Existing acceptance evidence is limited to specific environments; broader display configurations, dialogs and protected system surfaces need separate validation.

Coverage depends on the application, adapter and environment. Vision-based behaviour, complex interactions and failure recovery require intensive QA. These capabilities should not be read as universal or fully reliable computer control.

## Bridge / MCP and connectors

Bridge / MCP allows compatible clients to access Ariamir's permitted capabilities and work with tracked jobs. Connector and account management integrates selected external services when the relevant provider, account and permissions are configured.

Connector maturity varies. Listed, configured, connected and operational are different states; this showcase does not claim that every listed service works end to end. Credentials, account details and private service configuration remain private.

**External MCP is a separate candidate capability.** Ariamir can discover tools on explicitly configured remote servers and prepare an operation for human review. Execution requires authorization of that operation. Supported connection modes are limited; a compatible client or listed server does not establish complete integration. Legacy Ariamir bridge tool names remain unchanged.

## Projects, tasks and artifacts

The workspace groups conversations, tasks, attached material and generated files around projects. Development includes progress visibility, resumable work and artifact management.

Task recovery, cancellation, concurrent activity and consistency between the interface and actual execution state are ongoing QA areas. A displayed action must not be confused with a verified outcome.

## Permissions and operational review

Cross-system work includes permissioned actions, previews, reviewable outcomes and verification or rollback where supported. These are product behaviours under development, not security certifications or guarantees that every operation can be reversed.

Private permission rules, security implementation and production configuration are deliberately omitted. Public demonstrations should show observable behaviour using non-sensitive examples.

## Local diagnostics

Diagnostic tools inspect system health and storage and support bounded maintenance workflows with review and verification. Maintenance coverage is limited and remains under QA; Ariamir is not presented as a general autonomous system administrator.

Development builds include local health checks and explicitly requested diagnostic reports. A successful health check does not certify a full user workflow or establish that a newer development branch is deployed.

## Desktop application and distribution

The Windows desktop application brings the workspace and system controls together. Distribution work includes installation, launching, updates, repair and recovery while preserving user state.

Packaging, upgrade paths, interface consistency, accessibility and performance still need validation and polish. This documentation repository does not provide a finished installer or guarantee a stable public release.

Backup/restore and interruption-recovery work is implemented in the candidate and continues to receive fixes. Stable release still requires broader session testing, whole-application accessibility review, installer signing, a complete runtime software inventory and dependency analysis. Simulated failures do not prove physical power-loss durability.

## Local image and video

Image workflows exist in development builds. Local video work remains in integration and validation. Backend availability, model licensing, memory requirements and output quality vary by workflow.

Workflow files and a visible media option alone do not establish operational video generation. Installation-specific diagnostics are kept separate from public product status.

Public demos and performance claims require suitable licensing and measured evidence. The showcase does not imply that both media paths are complete or equally mature.

## Hardware Compatibility Lab and heterogeneous acceleration

The lab evaluates practical compatibility, latency, memory pressure and workload suitability on real hardware. Public benchmark methodology and published measurements are kept separate.

FPGA and other accelerator work is exploratory and includes partner-validation opportunities. It should not be interpreted as a completed general-purpose acceleration backend. See [the Hardware Compatibility Lab](hardware-lab.md).

## Enterprise environment

**Research / architecture exploration.** Ariamir is exploring a specialized environment for business and professional use, including controlled deployments, organizational security, permission governance, auditability, infrastructure integration, multi-user workflows and scalable heterogeneous compute.

The 0.19 module platform already includes controlled access for named users in supported module workflows. That implemented scope is narrower than these exploration goals: it does not establish a finished Enterprise edition, certified compliance or validated organizational scalability.

## Android portability

**Architecture / future work.** A mobile execution environment and portable capabilities are areas of exploration. Android-specific runtimes, providers and device integration require separate development and validation. This is not an announcement of a completed Android app.
