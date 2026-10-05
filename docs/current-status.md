# Ariamir 0.19 — current development status

**Reviewed 5 October 2026 · Modular transformation underway · M7 in progress**

Ariamir's current development line is **0.19**. Release-candidate work and the ongoing transformation are related, but they are not the same deliverable. The transformation is advancing through milestones; M7 has begun and is not complete.

This page is a dated summary of product scope. It is not a live service dashboard, a stable-release announcement or a claim that development changes are installed everywhere.

## The change in direction

The 0.19 line establishes a platform for business modules: focused extensions with their own views, project data, access controls and supported integrations. Recent work is making the wider capability platform more consistent to develop, validate, update and recover.

The intended benefit is a workspace that can grow around a user's work while preserving review and control. This showcase describes that benefit without publishing the design that implements it.

## Implemented in development builds

| Area | Publicly describable progress | Limit |
| --- | --- | --- |
| Business modules | Installation, updates, project data, controlled access, integrations and module diagnostics. | Candidate functionality; real-module deployment needs separate acceptance. |
| Module lifecycle | Backup participation, supported recovery and options to preserve or export data when retiring a module. | Recovery and compatibility depend on the supported operation and environment. |
| Development foundation | Runtime and developer-tooling work with automated validation and a versioned SDK. | Technical evidence is scoped to particular revisions; this does not announce public SDK availability or complete capability migration. |
| Assistant proposals | Advice and proposed next steps can be reviewed, corrected or accepted by a person. | Acceptance creates a plan; it does not execute an action. |
| Knowledge and documents | Source-aware retrieval, connected notes, document analysis and generated artifacts. | Accuracy, source selection, layout and complete workflows remain under QA. |
| Supervised tools | Supported browser, desktop, workspace and code operations, with reviewable outcomes. | Coverage varies; every application or action is not supported. |
| Optional connections | Configured cloud inference and external MCP tools alongside Ariamir's own client bridge. | Explicit consent, selection and authorization apply; provider/account availability varies. |

## Current work — M7 and prerequisite validation

M7 is concerned with proving a representative capability through the new development path. The reviewed records show a first attempt that did not complete, followed by diagnosis. They also show prerequisite validation being reopened after an earlier technical pass.

Accordingly, **M7 remains in progress and its prerequisite validation remains open**. Implementation, a passing test run, milestone acceptance, integration and product release are separate facts. Earlier successful checks are retained as evidence for their revisions; they do not close newer failures.

This review does not reproduce private plans, test logs, implementation contracts, repository links or operational details. No raw internal test total is presented as a public product-quality score.

## Still to validate

- Complete the representative capability workflow and close the current validation findings.
- Establish comparable behaviour and compatibility across supported capability implementations.
- Exercise installation, updates, recovery and real module integrations under the intended deployment conditions.
- Expand Browser/Desktop coverage, accessibility and longer real-model sessions.
- Validate document accuracy and presentation through complete user workflows.
- Prepare suitable public demonstrations and reproducible hardware measurements.

Local media remains dependent on its installed runtime and models. Enterprise deployment, Android and broader accelerator support remain separate exploration areas; they are not completed by reaching M7.

## How this snapshot was checked

The review compared the 0.19 release-candidate records with the current transformation branch, implementation files, milestone handoffs and the latest validation updates. Later records take precedence over an older milestone index or local checkout. Historical test results were read as evidence, not rerun or re-certified for this editorial update.

The connection to a running installation is not proof of the transformation branch's deployment status. Screenshots in this repository are historical development captures and are labelled accordingly.

[Capabilities](capabilities.md) · [Roadmap](roadmap.md) · [Disclosure policy](public-disclosure-policy.md)
