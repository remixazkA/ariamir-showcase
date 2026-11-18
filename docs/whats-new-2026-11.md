# What's new — November 2026

## Update — 18 November 2026

*Reviewed 18 November 2026.*

> **Status of this update.** The captures in this update are a design preview of the interface on sample data (interface text in Spanish; GPU names, models, projects and figures are examples). The capabilities they show are **in validation** on a development branch. They are **not part of the installed release**, and none of this is a benchmark result or a statement that validation is complete. See the [dated status](current-status.md).

Since 13 November the interface work has moved from how Ariamir looks to how it is set up and controlled on a real machine.

### Orchestration by team: roles and templates

An orchestration is built from **roles**. Each role shows what it does, its model and lane, the hardest task it accepts, its status and a pause button. **Templates** (office, programming, research, data, minimal) propose a set of roles and lanes, and say whether the set fits in the free GPU memory before anything is applied.

![Design preview of the orchestration templates: office, programming, research, data and minimal, each with its roles and lanes and whether it fits in free GPU memory](../media/screenshots/interface-preview/2026-11-18-orchestration-templates.png)

*Design preview. Orchestration templates (office, programming, research, data, minimal): their roles and lanes, and whether they fit in free GPU memory.*

![Design preview of the orchestration roles table: what each role does, its model and lane, the hardest task it accepts, its status and a pause button](../media/screenshots/interface-preview/2026-11-18-orchestration-roles-status.png)

*Design preview. Orchestration roles: what each one does, its model and lane, the hardest task it accepts, its status and a pause button.*

### Lanes per GPU, each with its own context

A model can serve several parallel **lanes**. Each lane has its own context, set with its own slider, and the screen shows how much of the GPU's total context the lanes use together.

![Design preview of lane settings: one context slider per lane and the share of the GPU's total context they use](../media/screenshots/interface-preview/2026-11-18-lanes-own-context.png)

*Design preview. Each lane with its own context: one slider per lane, and how much of the GPU's total context they use.*

### Fine engine settings (Advanced)

For people who want to go further, an **Advanced** area exposes 22 fine settings of the inference engine, in groups, each with the engine flag it sets and whether it has been measured on this computer.

![Design preview of the Advanced screen: 22 fine settings of the inference engine in groups, each with its flag and whether it has been measured on this computer](../media/screenshots/interface-preview/2026-11-18-advanced-engine-settings.png)

*Design preview. Advanced: 22 fine settings of the inference engine, in groups, each with its flag and whether it has been measured on this computer.*

### Test two configurations

**Test** puts two configurations side by side, with their memory and speed. It says plainly that it does not measure answer quality.

![Design preview of the Test screen: two configurations side by side with memory and speed, and a note that answer quality is not measured](../media/screenshots/interface-preview/2026-11-18-test-two-configurations.png)

*Design preview. Test: two configurations side by side, with memory and speed. It says plainly that it does not measure answer quality. Sample figures.*

### This computer

A compact panel, **This computer**, lists the running tasks, the loaded models, the memory of each GPU and of the system, and offers **Stop all**.

![Design preview of the This computer panel: running tasks, loaded models, memory of each GPU and of the system, and a Stop all button](../media/screenshots/interface-preview/2026-11-18-this-computer.png)

*Design preview. «This computer»: running tasks, loaded models, the memory of each GPU and the system, and «Stop all». Sample figures.*

### Permissions per project

Each project has one of three permission levels, a summary of what the chosen level allows, and fine adjustments.

![Design preview of project permissions: three levels, a summary of what the chosen one allows, and fine adjustments](../media/screenshots/interface-preview/2026-11-18-project-permissions.png)

*Design preview. Project permissions: three levels, a summary of what the chosen one allows, and fine adjustments.*

### Knowledge map

The **knowledge map** draws each topic as a cluster of notes joined by relations, and highlights the notes used by the last answer.

![Design preview of the knowledge map: clusters of notes joined by lines, with the notes used by the last answer highlighted](../media/screenshots/interface-preview/2026-11-18-knowledge-map.png)

*Design preview. Knowledge map: each topic is a cluster of notes, the lines are relations, and the notes used by the last answer are highlighted.*

### Office assistant

The office assistant only observes the sources the person allows, and each one can be allowed, changed or withdrawn. See [the captures below](#the-office-assistant-sources-and-consent).

### Status of the 18 November update

| Capability | Status |
| --- | --- |
| Orchestration by team: roles and templates | In validation (development branch) |
| Lanes with their own context | In validation (development branch) |
| Advanced engine settings, Test, This computer | In validation (development branch) |
| Permissions per project | In validation (development branch) |
| Knowledge map and office assistant | In validation (development branch) |

Capacity, speed and accuracy on real workloads still need validation; see the [roadmap](roadmap.md).

---

## 13 November 2026 — the new interface

*Captured 13 November 2026.*

> **Design preview.** Every image on this page comes from a navigable design prototype of the new Ariamir interface, not from an installed release. The prototype runs on sample data: project names, conversations, GPU names, memory figures, model names and times are examples. The interface text is shown in Spanish, as captured. Nothing here is a benchmark result, a guaranteed capacity or a statement that a feature has completed validation. See the [dated status](current-status.md) and the [disclosure policy](public-disclosure-policy.md).

The new interface is documented in a user manual that follows the same prototype. The pictures below show what has changed in how Ariamir looks and what it asks of you. For the whole interface, zone by zone, with full-window captures, see the [interface tour](interface-tour.md).

## The workspace

![Design preview of the workspace: sidebar with projects, a conversation with a permission card, and the conversation panel with context in tokens and a list of steps](../media/screenshots/interface-preview/workspace-overview.png)

*Design preview. The sidebar, the conversation and the conversation panel. The panel shows the context used, in tokens and by source, the steps taken so far, and the files and sources behind the conversation. When Ariamir needs permission to run a command, a card in the conversation explains what it wants and offers four choices.*

## Fabric: orchestration and roles

In Fabric, the work is done by an **orchestration**: a fixed group of **roles**, each with its own model. One role coordinates; others read, write, check or program. The word *agents* is kept for the sub-tasks of Direct mode.

![Design preview of a Fabric orchestration table: five roles, the model, lane and GPU each uses, the difficulty it receives, its current state and a pause button](../media/screenshots/interface-preview/fabric-orchestration-roles.png)

*Design preview. Each role shows the model and lane it uses and the GPU it runs on, the hardest tasks it receives, what it is doing now and a pause button. The role that coordinates carries a label, and a role can have no lane of its own.*

![Design preview of a conversation in Fabric: a summary line of roles working, queued and done, with the list of roles and what each is doing](../media/screenshots/interface-preview/fabric-roles-in-thread.png)

*Design preview. In a conversation, one live line counts the roles that are working, queued or done; unfolding it lists them with their current step.*

![Design preview of the check shown before switching a conversation to Fabric: models to load, memory per GPU and the note that it is a calculation](../media/screenshots/interface-preview/fabric-switch-fit-check.png)

*Design preview. Before switching to Fabric, Ariamir says which models it would load and what that takes from the GPU and from system memory. The figure is labelled as a calculation, and the switch happens only after you confirm.*

## Questions from Ariamir

![Design preview of a question card with four answers; one is marked Recommended and carries its reason](../media/screenshots/interface-preview/question-with-recommended-option.png)

*Design preview. When Ariamir needs a decision, it asks inside the conversation. A recommended answer comes first and gives its reason. Answering does not grant any permission, and you can also type your own reply.*

![Design preview of the second card of a three-question sequence with a counter](../media/screenshots/interface-preview/question-sequence.png)

*Design preview. Several questions in a row are shown one at a time, with a counter.*

## Response style and defaults

![Design preview of the project settings: an extension slider from Concise through Usual to Explanatory, and a tone selector](../media/screenshots/interface-preview/response-style-project.png)

*Design preview. The style of the answers is set per project: extension from Concise to Usual to Explanatory, and tone. It is a leaning, not a quota; each question is still answered on its own terms.*

![Design preview of the new-conversation defaults: mode, who answers, how much it thinks, a minimum-certainty slider and optional tools](../media/screenshots/interface-preview/new-conversation-defaults.png)

*Design preview. Defaults for new conversations: Direct or Fabric, the model that starts them, how much Ariamir thinks before answering, and a minimum-certainty setting between 40 % and 90 %. The certainty setting is a level of checking effort, not a probability that an answer is correct.*

## The office assistant: sources and consent

![Design preview of the office assistant settings: sources it may observe, each with its retention period, and what it has learned, with Approve and Discard](../media/screenshots/interface-preview/office-assistant-sources.png)

*Design preview. The office assistant lists what it may observe, what each source records and how long it keeps it. Sources that are not allowed say so. What it has learned is shown as suggestions you can approve, discard or remove, and every permission can be reviewed in a history.*

![Design preview of the consent step for work folders: what is kept and a choice of 7, 30 or 90 days](../media/screenshots/interface-preview/office-assistant-consent.png)

*Design preview. Allowing a source is an explicit step that states what is recorded and lets you choose the retention period first.*

## GPUs and models, drawn from the machine

The interface does not assume a fixed machine. GPUs, memory and models are drawn from what the computer reports: no GPU, one, or several. The names below are examples.

![Design preview of four memory meters: two GPUs, system memory and the disk used for models](../media/screenshots/interface-preview/gpu-memory-meters.png)

*Design preview. One meter per GPU, one for system memory and one for the disk that holds the models. Each splits memory into what the loaded models use, what other programs use and what is free.*

![Design preview of a compact memory list for a machine with four GPUs](../media/screenshots/interface-preview/four-gpu-machine.png)

*Design preview. A machine with four GPUs, shown as one compact row each. The same menu adapts to a machine with none.*

![Design preview of the model list: name, what each model reads, where it is loaded, lanes, engine, state and size on disk, with one model flagged as not fitting](../media/screenshots/interface-preview/model-list.png)

*Design preview. The model list shows what each model accepts (text, or text and images), the engine, its state and its size on disk. A loaded model also shows its GPU and how many lanes of how many tokens it has; a model on disk shows the largest context it supports and a link to load it. One model is marked as the default, and one that does not fit alongside the others is flagged.*

## Boundaries

- These views are a design preview. Availability in a given build depends on the build and configuration.
- Sample data and example names stand in for real projects, machines and models.
- Capacity, responsiveness and accuracy still need validation on real workloads; see the [roadmap](roadmap.md).
