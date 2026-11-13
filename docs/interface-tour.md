# Interface tour — design preview, November 2026

*Captured 13 November 2026.*

> **Design preview.** Every image on this page comes from a navigable prototype of the new Ariamir interface running on sample data. It is not an installed release. Project names, conversations, model names, GPU names, memory figures, times and prices are examples. The interface text is shown in Spanish, as captured. Nothing here is a benchmark result, a guaranteed capacity or a statement that a feature has completed validation. See the [dated status](current-status.md), the [roadmap](roadmap.md) and the [disclosure policy](public-disclosure-policy.md).

The tour goes through the interface zone by zone. Each zone opens with a full-window capture and continues with close-ups of its details. For a shorter summary of what changed, see [What's new — November 2026](whats-new-2026-11.md).

**Zones:** [Conversation](#conversation) · [Fabric](#fabric) · [Starting and searching](#starting-and-searching) · [Projects](#projects) · [Knowledge](#knowledge) · [Automations](#automations) · [Pending](#pending) · [Browser and video](#browser-and-video) · [Models](#models) · [Extensions](#extensions) · [This computer](#this-computer) · [Settings, office assistant and statistics](#settings-office-assistant-and-statistics) · [Documents next to the conversation](#documents-next-to-the-conversation) · [Themes](#themes)

## Conversation

![Design preview: a conversation in Direct mode with a numbered answer, a delivered file, a permission card and the conversation panel on the right](../media/screenshots/interface/01-conversation-direct-steps-permission.png)

*Full window, Direct mode. Left: projects and chats, with a branched conversation. Centre: the answer, a delivered file with an Open button, and a card where Ariamir asks permission to run a command, with four choices. Right: the conversation panel, with the context used (in tokens, by source) and the steps taken so far; the last step is waiting for the decision.*

![Design preview: the same conversation with the panel showing agents, changes, files, sources and automations](../media/screenshots/interface/02-conversation-side-panel.png)

*The conversation panel with its blocks collapsed to one line each: In progress, Agents (working, queued, done), Changes (3 files), Files, Sources and Automations. Under the card, one live line counts the agents.*

Details:

![The composer: a text box, an attached Knowledge source, the context meter and the model name](../media/screenshots/interface-preview/composer-controls.png)

*The writing box: add something, a Knowledge source attached to this message, the context meter, the model name and the send/stop button.*

![The model menu: Who answers, with two local models and one cloud model marked as leaving the computer](../media/screenshots/interface-preview/model-menu-who-answers.png)

*The menu of the model name. Each local model says where it is loaded and the context per lane; the cloud option says it asks permission before sending and is labelled as leaving the computer.*

![How much it thinks and a minimum-certainty slider set to 85 percent](../media/screenshots/interface-preview/thinking-and-confidence-slider.png)

*How much Ariamir thinks, in five levels from Quick to Maximum, and a minimum-certainty slider between 40 % and 90 %. The text beneath says that higher certainty means more checks before stating something, and that what cannot be reached is said so.*

![A live thinking line, unfolded to show the reasoning notes](../media/screenshots/interface-preview/live-thinking-line.png)

*While Ariamir thinks, the line says so; unfolded, it shows the notes it has made so far, with a link to see them all.*

![An unfolded work line listing each step, with one step opened to show what, input, result, duration and tool](../media/screenshots/interface-preview/steps-expanded.png)

*An unfolded work line: each step with its time, and one step opened to show what it was about, the result and the tool used.*

![A step that failed and was retried, listed with both attempts](../media/screenshots/interface-preview/step-failure-retry.png)

*A step that fails: the line says so, the retry is shown as attempt 2 and both attempts stay in the list.*

![The permissions menu of a conversation: the level of the project and what each setting allows](../media/screenshots/interface-preview/permissions-menu.png)

*The Permissions menu: the project's level (here Prudent), and what it means for commands, files, instructions and internet, with a button to change the project's permissions.*

![The context block: a bar split by source, token counts, a Summarize button and applied memory](../media/screenshots/interface-preview/context-breakdown.png)

*The Context block: a bar and the parts that make it up, in tokens (conversation, Knowledge, files, instructions), a button to summarize what came before and the number of memories applied.*

![The Changes block: one new file and two changed files with their added and removed lines, View and Undo buttons](../media/screenshots/interface-preview/changes-panel.png)

*The Changes block: one new file and two changed ones, with their added and removed lines, a View button and an Undo button for each, and Undo all.*

![The Agents block: each agent with its state, its model, its lane and its GPU, and a Stop button](../media/screenshots/interface-preview/agents-panel.png)

*The Agents block (Direct mode): each agent with its state, its model, its lane and GPU, and a Stop button.*

## Fabric

![Design preview: a conversation in Fabric with an orchestration of four parts, shown in the panel with roles and models](../media/screenshots/interface/03-conversation-fabric-roles.png)

*A conversation in Fabric. The switch at the top is set to Fabric, one live line in the thread counts the roles, and the panel shows the orchestration: each numbered part with its state, its difficulty, the role that handles it and, when relevant, why it waits.*

![Design preview: the Edit orchestration window with memory per GPU and a table of five roles](../media/screenshots/interface/04-fabric-orchestration.png)

*The Edit orchestration window. Top: the memory of each place (two GPUs and the system memory), split into models, lanes and other programs. Below: the five roles, each with its model, where it runs, its lanes and the size of task it receives. Nothing changes until Apply changes.*

Details:

![The check before switching to Fabric: models to load, memory on the GPU and a Load and switch button](../media/screenshots/interface-preview/fabric-does-not-fit.png)

*Before switching to Fabric: which models would be reloaded and with how many lanes, what that takes from the GPU and from system memory, labelled as a calculation, and the choice to load and switch or cancel.*

![Three ways to resolve Fabric not fitting on the GPU, and the other programs using the computer](../media/screenshots/interface-preview/fabric-gpu-options.png)

*If Fabric does not fit on the GPU: use only the GPU (what does not fit waits its turn), also use system memory, or keep the roles as they are. Below, the other applications using the computer.*

![A request to load a model on a second GPU that reports it does not fit, with the option to load with a smaller context](../media/screenshots/interface-preview/load-model-does-not-fit.png)

*Asking in conversation to load a model on a second GPU: the card does the sum, says that 1.2 GB are missing and offers a smaller context instead of loading it as asked.*

## Starting and searching

![Design preview: the start screen with a project selector, a writing box and four ideas](../media/screenshots/interface/05-new-conversation.png)

*A new conversation: which project it will go to, the writing box with the context meter and the model, and four ideas to start.*

![Design preview: the first-run screen listing models that can be downloaded and whether they fit this computer](../media/screenshots/interface/06-first-run-model-choice.png)

*First run, with no model on the computer: Ariamir lists the models it can download, with their size and whether each one fits, and says that the download comes from the internet once.*

![Design preview: the search window with a typed word, results in conversations and keyboard hints](../media/screenshots/interface/07-search.png)

*Search with a word typed: each result says which project and day it comes from and highlights the match. The footer lists the keys.*

## Projects

![Design preview: a project page with a writing box and a list of deliverables with their versions and states](../media/screenshots/interface/08-project-page.png)

*A project page, on its Deliverables tab: the project's counts and permissions, a box to start a chat, and each deliverable with its version, its time, its state (draft, reviewed, published, archived) and an Open button.*

![A claim from a research under review: its citations, a note field and Accept and Reject](../media/screenshots/interface-preview/claim-review.png)

*Reviewing a claim from a research: the sentence, how it was reached, the two sources that support it, an optional note, and Accept and Reject.*

## Knowledge

![Design preview: the Knowledge home with a paused import, folders and recent notes](../media/screenshots/interface/09-knowledge-home.png)

*Knowledge home: a search box, the number of changes waiting for review, four tabs (Notes, To review, Map, Memory), a paused import with a Resume button, six folders and the latest notes with their state.*

![Design preview: the Knowledge map showing clusters of notes joined by lines, with a legend](../media/screenshots/interface/10-knowledge-map.png)

*The Knowledge map: each topic is a cluster of notes and the lines are relations. The legend tells the line styles apart: text link, named relation, contradicts, deduced. The notes the last answer used are marked.*

Details:

![A proposed correction to a note: what changes shown in red and green, and Save the change](../media/screenshots/interface-preview/knowledge-proposed-correction.png)

*A proposed correction: why it is proposed, what would change (the removed line in red, the added one in green) and the buttons Save the change, Reject and Open the note. The text says that once saved there is no undo, and that the earlier version stays in the note's history.*

![The Memory tab: remembered preferences, each with its origin and a Forget button](../media/screenshots/interface-preview/knowledge-memory.png)

*The Memory tab: what Ariamir remembers about the person and the project, each item with where it came from and a Forget button.*

## Automations

![Design preview: the Missions tab of Automations, with five missions and their progress](../media/screenshots/interface/11-automations-missions.png)

*The Missions tab: each mission is an errand with several tasks, shown with how many are done and its state (working, waiting for permission, ready to close, paused, finished). The text says that Ariamir does the tasks and tells the person if it needs something. The other tabs are Scheduled and History.*

![Design preview: the History tab of Automations, with runs grouped by day](../media/screenshots/interface/11-automations-history.png)

*The History tab: every run grouped by day, with its time and duration. One is running, one is waiting for review, one failed and offers Retry.*

Details:

![Asking for two automations in plain words, correcting the request and confirming](../media/screenshots/interface-preview/automation-by-chat.png)

*Created by asking: the request is corrected with a second message, Ariamir changes both and, after the person says yes, creates them and gives the next run.*

![An open automation: what it does, last run and its actions](../media/screenshots/interface-preview/automation-open.png)

*An open automation: what it does, the next and last runs and the actions Run now, Edit, Simulate, Download log and Delete.*

![The run history grouped by day, with one failed run opened to show its steps](../media/screenshots/interface-preview/automation-run-history.png)

*History: each run by day, with its time and duration, and a failed one opened to show which step could not complete and a Retry button.*

## Pending

![Design preview: the Pending screen with permission requests and a request to sign in, followed by proposals](../media/screenshots/interface/12-pending.png)

*Pending: what is waiting for a decision across all projects, answered in place. Cards for a command permission, a permission to read a folder, and a request for the person to sign in on a website; below, proposals without hurry.*

![Two proposals from the office assistant, each with four buttons, and a row of notes to review](../media/screenshots/interface-preview/pending-proposals.png)

*Proposals: each says where it comes from and why, and offers Accept, Correct…, Not now and Reject.*

## Browser and video

![Design preview: a conversation while Ariamir browses a website, with the browser panel on the right](../media/screenshots/interface/20-browser-panel.png)

*While Ariamir browses, the thread lists the pages it opened and reads, and the browser panel on the right shows the page as Ariamir sees it, with a Take control button. The page shown is an example.*

![A card saying Ariamir needs the person to sign in, with Open the browser and Cancel the task](../media/screenshots/interface-preview/browser-handoff-card.png)

*When Ariamir needs the person, it says so in the conversation: it neither has the password nor asks for it, and it waits until the person finishes.*

![The browser panel with the person in control: Ariamir paused and a button to hand back control](../media/screenshots/interface-preview/browser-user-control.png)

*With the person in control, Ariamir is paused and does not see what is typed; a button hands control back.*

![A video delivered as a file with a thumbnail and an Open button](../media/screenshots/interface-preview/video-ready.png)

*A finished video is one more delivery, with a thumbnail and an Open button.*

![A video being generated with a progress bar and a Stop button](../media/screenshots/interface-preview/video-generating.png)

*While a video is generated, the message carries a card with progress and a Stop button.*

## Models

![Design preview: the Models screen with four meters, a download in progress and a list of models](../media/screenshots/interface/13-models.png)

*Models, tab In this computer: one meter per GPU, one for system memory and one for the disk that holds the models; parallel agents; a download in progress with a Cancel button; and the model list with state and size on disk. Other tabs: Catalog, Cloud, Fabric.*

Details:

![The sum for a loaded model: memory per GPU and system memory split by source, with a measured note](../media/screenshots/interface-preview/model-fit-calculation.png)

*How a model is loaded: the sum, measured on the computer, for each GPU and for system memory, split into this model, other models, other programs and free space, with the speed measured on the last tests.*

![Engine and where to load a model: two engines and three places, with free memory shown for each](../media/screenshots/interface-preview/model-placement.png)

*Engine and place: the model can be served by either of two engines and loaded on a GPU or on the CPU, each place showing its free memory.*

![A pre-load sum for a second GPU, with a shortfall of memory and a warning that the lanes no longer fit](../media/screenshots/interface-preview/model-does-not-fit.png)

*Before loading, the sum is labelled as a calculation. Here the GPU is over its memory by 0.3 GB, and a warning says that the context given to the lanes no longer fits and that a lane should be lowered; the Load button is greyed out.*

![Two speed tests side by side with their difference](../media/screenshots/interface-preview/model-test-compare.png)

*Test: two runs side by side with their difference in memory and in tokens per second. The text notes that it measures speed and memory, not how correct the answers are.*

![Cloud models: a warning that the conversation leaves the computer, and the limits of each](../media/screenshots/interface-preview/cloud-models.png)

*Cloud models: the warning that the conversation leaves the computer, and for each one its limits and use this month.*

## Extensions

![Design preview: the Extensions screen with modules and their switches](../media/screenshots/interface/14-extensions.png)

*Extensions, Modules tab: each module with what it does and a switch. One has an update available and one is marked as in testing.*

Details:

![An open module: version, tools and what it can do, with Update and Remove](../media/screenshots/interface-preview/module-open.png)

*An open module: its version, its tools and what it is allowed to do, with Update and Remove.*

## This computer

![Design preview: the This computer menu listing tasks, loaded models and memory of four GPUs](../media/screenshots/interface/15-this-machine-four-gpus.png)

*The menu of the sidebar's This computer row, for an example machine with four GPUs: running tasks, loaded models with their lanes, and memory per GPU and for the system. The menu adapts to the number of GPUs the computer reports.*

![A warning that a GPU has little memory left and that another program is using part of it](../media/screenshots/interface-preview/machine-memory-warning.png)

*A warning says which GPU is running out of space and that another program is using part of it.*

## Settings, office assistant and statistics

![Design preview: the General settings with language, theme, text size and notifications](../media/screenshots/interface/16-settings-general.png)

*Settings, General: language, theme (four themes), text size, keyboard shortcuts, notifications and start-up. The left menu has two groups: For you, and Of this computer.*

![Design preview: the office assistant settings, with sources, retention and learned suggestions](../media/screenshots/interface/17-office-assistant.png)

*Settings, Office assistant: what it may observe (mail and desktop, each with its detail, retention period, Change and Withdraw buttons), what it has learned (suggestions to approve or discard) and the history of permissions.*

![Privacy settings: cloud models, always-allowed internet sends and saved browser sessions](../media/screenshots/interface-preview/privacy-settings.png)

*Settings, Privacy: whether cloud models are never, asked each time or allowed; what the office assistant observes; sends to the internet that are always allowed, with Revoke; and saved browser sessions, each with a Forget button. Addresses are examples.*

![Design preview: usage statistics with four figures, a bar chart per day and a split by model](../media/screenshots/interface/18-statistics.png)

*Statistics: four figures (tokens, conversations, active days and the measured median speed), a bar per day split into read and written tokens, and where the use went, by model.*

## Documents next to the conversation

![Design preview: a document opened beside the conversation with a comparison between versions in green and red](../media/screenshots/interface/19-document-compare.png)

*A delivered document opened next to the conversation, here comparing version 1 with version 2: the header says how many lines were added and removed, added lines are green and removed ones red.*

![Selecting text in a document and asking for a change in the box below](../media/screenshots/interface-preview/ask-change-on-selection.png)

*Asking for a change on a selection: the chosen passage is quoted in the writing box and the request is typed underneath.*

## Themes

The interface has four themes: a dark neutral one, a light one and two dark ones with an accent colour. The captures below show three of them.

![Design preview: a conversation in the light Paper theme](../media/screenshots/interface/21-theme-paper.png)

*Paper, a light theme.*

![Design preview: the start screen in the dark Ember theme with an amber accent](../media/screenshots/interface/22-theme-ember.png)

*Ember, a dark theme with an amber accent.*

![Design preview: a conversation in the dark Midnight theme with a mint accent](../media/screenshots/interface/23-theme-midnight.png)

*Midnight, a very dark theme with a mint accent.*

## Boundaries

- These views are a design preview. Availability in a given build depends on the build and configuration.
- Sample data and example names stand in for real projects, machines, models, addresses and figures.
- Capacity, responsiveness and accuracy still need validation on real workloads; see the [roadmap](roadmap.md).
