# What's new — November 2026

*Captured 13 November 2026.*

> **Design preview.** Every image on this page comes from a navigable design prototype of the new Ariamir interface, not from an installed release. The prototype runs on sample data: project names, conversations, GPU names, memory figures, model names and times are examples. The interface text is shown in Spanish, as captured. Nothing here is a benchmark result, a guaranteed capacity or a statement that a feature has completed validation. See the [dated status](current-status.md) and the [disclosure policy](public-disclosure-policy.md).

The new interface is documented in a user manual that follows the same prototype. The pictures below show what has changed in how Ariamir looks and what it asks of you.

## The workspace

![Design preview of the workspace: sidebar with projects, a conversation with a permission card, and the conversation panel with context in tokens and a list of steps](../media/screenshots/interface-preview/workspace-overview.png)

*Design preview. The sidebar, the conversation and the conversation panel. The panel shows the context used, in tokens and by source, the steps taken so far, and the files and sources behind the conversation. When Ariamir needs permission to run a command, a card in the conversation explains what it wants and offers four choices.*

## Fabric: orchestration and roles

In Fabric, the work is done by an **orchestration**: a fixed group of **roles**, each with its own model. One role coordinates; others read, write, check or program. The word *agents* is kept for the sub-tasks of Direct mode.

![Design preview of a Fabric orchestration table: five roles, their models, the GPU each runs on, lanes and current state](../media/screenshots/interface-preview/fabric-orchestration-roles.png)

*Design preview. Each role shows its model, where it runs (a GPU or the CPU), its lanes and what it is doing now. The role that coordinates carries a label.*

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

![Design preview of the model list: name, what each model reads, where it is loaded, lanes, engine, state and size on disk](../media/screenshots/interface-preview/model-list.png)

*Design preview. The model list shows what each model accepts, where it is loaded, how many lanes and how many tokens of context each has, the engine, its state and its size on disk. A model that does not fit alongside the others is flagged.*

## Boundaries

- These views are a design preview. Availability in a given build depends on the build and configuration.
- Sample data and example names stand in for real projects, machines and models.
- Capacity, responsiveness and accuracy still need validation on real workloads; see the [roadmap](roadmap.md).
