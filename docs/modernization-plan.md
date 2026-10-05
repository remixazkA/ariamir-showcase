# Modernization and integration plan

**Ariamir 0.19 onward · Public summary · Reviewed 5 October 2026**

Ariamir is being modernized so its capabilities can evolve without forcing users to start over. The plan combines a more extensible product, selective adoption of Python for suitable AI workloads, stronger integration between existing tools, and a staged path to macOS and Linux.

The aim is continuity: keep projects useful, preserve human control and make improvements easier to validate, install and recover. The work proceeds in stages, with compatibility and measured results deciding when a change is ready.

## What users should gain

| Priority | Intended improvement |
| --- | --- |
| A workspace that grows with the work | Add focused capabilities and business modules without rebuilding the whole product around each one. |
| Better access to AI and scientific tooling | Use suitable Python-based tools where they improve functionality, maintainability or measured performance. |
| Continuity through change | Keep supported projects, documents, settings and permissions usable as components evolve. |
| More coherent workflows | Bring knowledge, research, models, documents and supervised actions together with clearer progress and outcomes. |
| Easier installation and recovery | Package required components and validate updates, backup restoration and return to a supported previous version. |
| A path beyond Windows | Prepare the product for selected macOS and Linux configurations, with an explicit support matrix. |

These are the objectives of the program. Their implementation and acceptance status are tracked separately in [current status](current-status.md) and the [roadmap](roadmap.md).

## Build on the platform already in development

The 0.19 development line includes business-module support: focused views, project data, controlled access, integrations and a managed lifecycle. Knowledge, documents, model management, browser and desktop tools, assistant proposals and connected services provide the wider product foundation.

Modernization preserves useful existing behaviour and reuses supported services. A new implementation must justify its place. Components that already serve the product well can remain in their current form; changing programming language is not an outcome in itself.

Business integration is also assessed separately from the platform beneath it. A module framework working with a synthetic example does not prove that a particular business application, account or deployment has passed acceptance.

## Modernize one capability at a time

A capability is a bounded piece of work Ariamir can provide, such as document processing, source retrieval or an image-analysis task. The plan makes these pieces easier to develop and replace while keeping the experience and supported behaviour consistent.

TypeScript and Python can coexist. Python is introduced selectively where its ecosystem or a measured result makes it useful. The plan does not require every component to move, and it does not promise that Python alone will make a workload faster.

Before a replacement is adopted, it must demonstrate compatible behaviour, preserved project data and permissions, acceptable resource use and a tested recovery path. Broader adoption follows a representative integration example and a real workload pilot.

## Connect the work across product areas

The program evaluates improvements across several existing areas. This is a description of product scope, not a declaration that their migration has finished.

| Area | What modernization should help deliver |
| --- | --- |
| AI and data processing | Access to suitable model, scientific and processing tools, with measured resource use. |
| Knowledge and research | Continuity of sources, project information and evidence throughout ingestion, retrieval and reporting. |
| Model coordination | More consistent behaviour under load, including visible limits and recoverable interruptions. |
| Context and longer tasks | Less repeated work while retaining the evidence needed to continue a task accurately. |
| Planning and supervised actions | Clear separation between advice, a proposed action, authorization and the observed result. |
| Vision and perception | Better-supported interpretation of visual information within the applicable consent and environment limits. |

The order and scope of individual changes depend on demonstrated benefit and compatibility. No internal routing rules, runtime protocols or migration procedures are published here.

## Protect continuity and measure the whole result

Success means more than producing a similar answer. A changed capability must preserve the supported workflow, its project state and the person's control over actions. Updates must be tested with existing data; recovery must be demonstrated after interruptions and failed changes.

Performance is assessed across the complete task: quality, responsiveness, memory use, startup and context consumption. A faster isolated operation is insufficient if the overall workflow becomes less reliable or consumes substantially more resources. This showcase publishes no unmeasured speed or token-saving claim.

## Prepare other platforms in stages

Windows remains the reference environment during the current modernization. Preparatory work reduces assumptions tied to one operating system, but preparation alone does not make another system supported.

The planned sequence is a portable foundation, then real installations on selected macOS Apple Silicon and Linux configurations. Installation, project restoration, local models and core workflows must be tested on actual hardware. Browser and desktop control may have different coverage on each platform, which must be stated explicitly.

The target is one coherent product with a documented compatibility matrix. Universal parity across devices and desktop environments is not promised.

## Where the program stands

**Implemented groundwork:** business-module lifecycle support and development work on the runtime and developer tooling, with scoped technical evidence.

**Current focus:** validating a representative extension through the new development path. Integration checks remain open; the program has not completed broad capability migration.

**Next:** a real workload pilot, selective adoption across further capabilities and integrated product hardening. The portable foundation, macOS/Linux enablement, public beta and stable release follow their own acceptance criteria.

See the [roadmap](roadmap.md) for the sequence and what must be demonstrated at each stage.

## What remains private

This summary communicates purpose, scope and acceptance outcomes. It excludes the master plan's internal architecture, technical contracts, security mechanisms, operational procedures, staffing and budgets, private integration details and source evidence. The supplied planning documents are not distributed in this repository.

[Current status](current-status.md) · [Roadmap](roadmap.md) · [Capabilities](capabilities.md) · [Disclosure policy](public-disclosure-policy.md)
