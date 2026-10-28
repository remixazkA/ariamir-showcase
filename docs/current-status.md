# Current development status

**Reviewed 28 October 2026 · Ariamir 0.19 · Modernization and integration**

Ariamir is modernizing how capabilities are developed and integrated while preserving the existing product. The **representative integration is complete**: a representative extension was built through the new development path, integrated into the product and accepted. The current focus is preparing a **real workload pilot** and hardening the integrated release.

Broad capability migration, macOS/Linux support and stable-release acceptance have not been completed by this work.

[Read the modernization plan](modernization-plan.md) · [See the roadmap to 1.0](roadmap.md)

## Implemented in development builds

| Area | Current scope | Boundary |
| --- | --- | --- |
| Business modules | Focused views, project data, controlled access, integrations and diagnostics. | Acceptance of a specific business module or deployment is separate from platform support. |
| Module lifecycle | Installation, updates, backup participation and supported retirement/recovery options. | Behaviour depends on the supported operation, versions and environment. |
| Modernization groundwork | Runtime and developer-tooling implementation for compatible capabilities, exercised end to end by the representative extension. | Not a completed migration or an announcement of public SDK availability. |
| Knowledge and documents | Source-aware retrieval, connected notes, document analysis and generated artifacts. | Accuracy, presentation and complete user workflows remain under QA. |
| Assistant proposals | Review, correct or accept suggested next steps. | Accepting a proposal does not authorize or execute its action. |
| Supervised tools and connections | Supported browser, desktop, workspace and code operations, with optional configured services and models. | Coverage, dependencies, accounts and permissions vary. |

Implemented means functionality exists in the reviewed development work. It does not mean every combination is available, deployed or accepted for production.

## Completed since the previous review

- **Accumulated development work merged into the main development line** in two steps (24 and 27 October 2026), each after the full regression run passed on the integrated build.
- **Context management in development builds.** Important rules and the current request are never summarized away; content recalled from memory, Knowledge or attachments informs the assistant but cannot give it instructions; expired conversation text is purged after 24 hours; long tasks keep versioned checkpoints so they can be resumed. Preparing the context for a request went from minutes to a fraction of a second in measurement.
- **Security hardening.** Errors returned to connected clients no longer include local file paths; a case where an error could reveal the beginning of a password was closed; network folders and links are handled more strictly; operations that need the person's approval no longer touch the disk before it is given.
- **Local inference in the lab.** Prompt-cache reuse now works for hybrid-architecture models, and speculative decoding roughly doubled generation throughput in early tests on the lab's data-centre GPU (see the [Hardware Lab](hardware-lab.md)).

## In validation

These changes are implemented on development branches and under independent review; they are not yet part of the main development line.

- **Model menu that reflects the machine.** The chat's model menu lists the models actually installed, with their state (loaded, installed, not checked or cloud), instead of a fixed list.
- **Configurable context window.** The person can choose the context window for each local model from the model menu; it applies the next time the model loads.
- **AMD Radeon graphics on Windows.** Ariamir detects and measures graphics cards from any vendor, uses Radeon cards through Vulkan and reports clearly when a model has no build for that card. Validation on a real Radeon card (RX 9070 XT) is pending.

## Work in progress

- Close the real workload pilot on short validation runs; a long continuous run is postponed.
- Continue the compute, Knowledge ingestion, research and agent-coordination capabilities toward their validation criteria.
- Evaluate controlling the local inference engine directly for parallel agents, keeping the current model manager for downloads during any transition.
- Extend AMD support to local image and video workflows.
- Harden the integrated release: installation, permissions, updates and platform protection.

Development builds currently target Windows 11 (64-bit). Earlier successful checks remain evidence for their revisions; they do not establish completion of later work.

## What follows

The planned sequence continues with the real workload pilot, selective modernization across further product areas, integrated release hardening, a portable foundation, selected macOS/Linux builds, public beta and a stable release. Each stage has its own completion criteria in the [roadmap](roadmap.md).

Local image/video workflows remain dependent on installed runtimes and models. Enterprise administration, Android and experimental accelerators remain separate exploration tracks.

## Evidence and availability

This snapshot was checked against current development records alongside the modernization plan. Planning documents describe intended scope; current implementation and validation records determine what can be reported as done. Internal task labels are not used as a substitute for explaining product progress.

The running installation, a development branch and a release candidate may differ. No new installer, public SDK or stable release is announced by this documentation update. Existing screenshots are historical development captures, not proof of the current integration result.

Private source documents, implementation details, internal logs and operational data are excluded under the [disclosure policy](public-disclosure-policy.md).
