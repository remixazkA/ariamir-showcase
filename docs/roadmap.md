# Roadmap to a stable Ariamir workspace

**Reviewed 5 October 2026 · Current development line: 0.19**

Ariamir's next stages connect modernization, product integration and platform expansion. The goal is an extensible workspace that people can install, use, update and recover without losing project continuity or control over actions.

Version numbers below identify planned release themes. They are not delivery dates or evidence that a release is already available. The 0.19 line is under development; later stages remain planned and depend on validation of the preceding work.

[Why we are modernizing Ariamir](modernization-plan.md) · [Current implementation status](current-status.md)

## The route ahead

| Stage | Status | Outcome for users | Completion evidence |
| --- | --- | --- | --- |
| **0.19 · Capability modernization and integration** | **In development** | A more extensible workspace, with selected AI capabilities able to evolve while preserving supported behaviour and project continuity. | A real workload proves the new path; the selected changes pass compatibility, recovery and integrated release checks. |
| **0.20 · Portable product foundation** | Planned; preparatory work underway in 0.19 | Fewer dependencies on a single operating system and clearer requirements for each capability. | Core workflows can be tested independently of Windows-specific assumptions; remaining platform limits are documented. |
| **0.21 · macOS and Linux enablement** | Planned | Install and use Ariamir on selected macOS Apple Silicon and Linux configurations. | Clean installation, project restore, local models and core workflows pass on real hardware; platform coverage is published. |
| **0.22 · Public beta and integration stability** | Planned | Third parties can test the product and build against documented, sufficiently stable interfaces. | Sustained external use, supported upgrade paths and a public compatibility matrix, with issues measured and tracked. |
| **1.0 release candidate** | Planned | A complete release package focused on reliability, security, usability and support. | Reproducible packaging, signing, recovery and full release rehearsal pass; remaining fixes do not require product redesign. |
| **1.0 · Stable workspace** | Target | An installable, recoverable and extensible AI workspace with bounded autonomy and human control. | Published support scope and measurable acceptance across stability, verified actions, data continuity and resource use. |

## 0.19 — modernize capabilities and integrate the product

This phase builds on business modules, Knowledge, documents, model management and supervised tools already present in development builds. It introduces a more consistent development path and uses Python selectively where it provides a demonstrated advantage.

The work has four parts:

1. **Establish the foundation.** Preserve existing behaviour and provide the runtime and developer tooling needed to build compatible capabilities. Substantial groundwork is implemented, with validation still open.
2. **Prove integration.** Exercise a representative extension with synthetic data, then validate a real AI workload. The representative integration is the current focus; it is not yet a completed acceptance result.
3. **Adopt selectively.** Evaluate capabilities in AI/data processing, Knowledge, research, model coordination, context, planning and vision. Keep existing implementations where changing them would not provide a justified benefit.
4. **Harden the integrated release.** Validate long sessions, interruptions, installation, updates, restore and the interaction between changed and unchanged components.

**Ready to move on when:** a relevant real workload can use the new implementation without breaking the supported user experience, permissions or data continuity; selected migrations have explicit outcomes; and recovery and resource use have been tested. Completing an example or shipping an interim candidate does not finish this entire phase.

## 0.20 — complete the portable foundation

Make operating-system requirements explicit and reduce remaining Windows assumptions across the product. Capabilities should clearly report whether the required backend, hardware and permissions are available.

**Ready to move on when:** the core and its compatibility tests no longer depend on implicit Windows behaviour, and platform-specific limitations are identifiable and documented. This stage establishes portability; it does not itself announce working macOS or Linux editions.

## 0.21 — enable selected macOS and Linux configurations

Validate real product builds on macOS Apple Silicon and selected Linux environments, while retaining Windows regression coverage. The work includes installation and updates, project transfer and restore, local model use, Knowledge, workspace functions, MCP and browser workflows.

Desktop control is evaluated against the permissions and capabilities of each environment. Differences in coverage must be visible rather than hidden behind a claim of full parity.

**Ready to move on when:** a clean installation on at least one supported macOS Apple Silicon configuration and one supported Linux distribution can restore a project, use local inference and complete the defined core workflows on real hardware. Publish the tested configurations and the supported/unsupported desktop features.

## 0.22 — test with third parties and stabilize integrations

Shift from internal development to sustained use on other people's machines. Stabilize documented integration interfaces and data formats, explain compatibility and deprecations, and exercise migrations from supported versions.

The public beta also needs a clear support process, privacy information, optional diagnostic reporting and a platform/hardware matrix. New feature growth must leave room for reliability and usability work.

**Ready to move on when:** external users can install and use Ariamir over extended periods, issues are measurable, and supported upgrades and integrations behave consistently. Beta availability will be announced separately.

## 1.0 release candidate — rehearse delivery and recovery

Concentrate on defects, performance, security, accessibility, documentation and compatibility. Complete signed, reproducible distribution, dependency and license records, installation/repair/update checks, backup restoration and a full release rehearsal.

**Ready to move on when:** the remaining issues can be fixed without redesigning the product or breaking the stabilized interfaces, and the supported installation and recovery paths have been demonstrated.

## 1.0 — stable within a declared support scope

The target brings together project knowledge, documents and artifacts, model coordination, durable tasks, supervised browser/desktop work, connected services and extensible capabilities.

Stability must be supported by published criteria: session reliability, verified actions, recovery after interruption, data continuity, audit integrity, resource use and installation/update behaviour. The release should state exactly which platforms and workflows it supports, together with its known limitations.

## Work that continues through every stage

| Priority | What must remain visible |
| --- | --- |
| Quality and evidence | Regression results, complete workflow tests and representative measurements; demonstrations distinguished from simulations. |
| Security and privacy | Reviewed permissions, protected data and credentials, controlled dependencies and user choice over diagnostic sharing. |
| Data lifecycle | Export, retention, deletion, backup and tested recovery as capabilities and versions change. |
| Usability and access | Understandable progress and errors, accessibility, internationalization and clear optional-feature requirements. |
| Performance | Comparable measurements of latency, memory, model/context use and overall task quality. |
| Documentation and support | Current release notes, compatibility information and recovery guidance that matches the shipped build. |

## Separate exploration tracks

Broader enterprise administration, Android, distributed execution across machines, experimental FPGA/accelerator work and formal certifications remain separate directions. They do not block the first stable release unless the scope is explicitly changed. Existing module access controls should not be read as completion of enterprise administration.

## How progress is reported

The [status page](current-status.md) records the current phase in plain language. A stage advances on demonstrated outcomes, not on an internal task number or a target date. Technical validation, integration, release availability and whole-product acceptance remain distinct. If a check reopens, the status must reflect the remaining work.

This is a public roadmap, not a copy of the internal execution plan. Implementation designs, internal acceptance thresholds, private integrations and operational records remain private.
