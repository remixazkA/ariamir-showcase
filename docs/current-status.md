# Current development status

**Reviewed 16 October 2026 · Ariamir 0.19 · Modernization and integration**

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

- **Representative integration accepted (10 October 2026).** The representative extension runs through the new development path inside the product.
- **24-hour continuous run completed and approved.** Follow-up checks on long-run resource use continue as part of normal hardening.
- **Core regression suite passing on the integrated build** (1,204 of 1,204 checks, 16 October 2026).

## Work in progress

- Prepare the real workload pilot as a capability on the new development path.
- Harden the integrated release: installation, permissions and platform protection.
- Demonstrate continuity through updates, interruption, cancellation and restoration.
- Continue cross-system QA, usability, accessibility and supported-environment testing.

Development builds currently target Windows 11 (64-bit). Earlier successful checks remain evidence for their revisions; they do not establish completion of later work.

## What follows

The planned sequence continues with the real workload pilot, selective modernization across further product areas, integrated release hardening, a portable foundation, selected macOS/Linux builds, public beta and a stable release. Each stage has its own completion criteria in the [roadmap](roadmap.md).

Local image/video workflows remain dependent on installed runtimes and models. Enterprise administration, Android and experimental accelerators remain separate exploration tracks.

## Evidence and availability

This snapshot was checked against current development records alongside the modernization plan. Planning documents describe intended scope; current implementation and validation records determine what can be reported as done. Internal task labels are not used as a substitute for explaining product progress.

The running installation, a development branch and a release candidate may differ. No new installer, public SDK or stable release is announced by this documentation update. Existing screenshots are historical development captures, not proof of the current integration result.

Private source documents, implementation details, internal logs and operational data are excluded under the [disclosure policy](public-disclosure-policy.md).
