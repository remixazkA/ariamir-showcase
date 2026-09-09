# Knowledge, Graph Workspace and Learning

> **Active development, not a finished system.** Knowledge and its related workflows still need intensive QA, end-to-end validation and interface polish. This page describes product scope without publishing proprietary implementation.

## Knowledge as a project workspace

Knowledge gives Ariamir a dedicated place for durable project information: notes, sources, decisions and relationships. The goal is to make useful information editable, discoverable and traceable across tasks.

Development work includes:

- Markdown note editing and organization.
- Search and retrieval of relevant notes and source passages.
- Relationships between notes, claims, decisions and supporting material.
- Source references, uncertainty and contradiction awareness.
- Multiple knowledge profiles and authorized federated views.
- Import/export, storage portability and synchronization workflows.
- Reviewable proposals for changes and maintenance.

These capabilities have different validation needs. A feature existing in a development build does not establish that every storage, synchronization or retrieval scenario is reliable.

## Graph Workspace

Graph Workspace makes connected information explorable through a visual map. Users can inspect a node, follow relationships, filter the view and return to useful saved views.

Knowledge is the central view. Optional views can bring in tasks, code and Fabric activity to help users understand work in context. Viewing another system's information does not turn it into an accepted Knowledge note.

The interface is being refined to keep authored relationships, inferred connections and uncertain information distinguishable. Readability, keyboard access, large-graph interaction and cross-system views remain ongoing QA and usability work.

## Retrieval with context

Knowledge can supply relevant project information to Ariamir's work, including prior decisions and supporting sources. The aim is to help answer questions such as “What did we decide?” or “Which source supports this claim?” with traceable context.

Retrieval can still miss relevant information, surface stale material or rank an imperfect match. An answer should remain assessable against its sources; finding a note does not prove its contents are correct.

## Learning through proposals

Knowledge Learning develops a path from selected observations and reviewed task outcomes to proposed additions or corrections. Users can inspect proposed learning before accepting changes to project knowledge.

Feedback and consolidation work helps identify useful material, potential contradictions and maintenance needs. These functions are still being tested. They are not a claim of unrestricted autonomous learning, automatic truth verification or base-model retraining.

Repeated claims, model-generated answers and frequent retrieval are not independent evidence. A suggestion needs appropriate source context and review before it should be treated as trusted knowledge.

## Knowledge and Memory have different roles

| System | Intended role | Illustrative example |
| --- | --- | --- |
| Knowledge | Durable project information and supporting sources | A project decision with a reference to its rationale |
| Memory | Conversational continuity and user preferences | A preference for concise answers |
| Graph Workspace | Exploration of information and relationships | A view of notes connected to a decision |
| Knowledge Learning | Proposed knowledge improvements | A suggested correction for review |

The examples are fictitious. Separation between these roles is an active validation area, not a claim that mistakes are impossible.

## What still needs work

Current priorities include retrieval relevance, proposal quality, source traceability, contradictory or stale information, synchronization consistency, recovery, performance and accessibility. Integration with Fabric, tasks, code and document workflows also needs continued end-to-end testing.

Public demonstrations will use synthetic or redistributable notes. Private vaults, personal memories, customer data, internal schemas, prompts and learning rules are excluded from this showcase. See the [public disclosure policy](public-disclosure-policy.md).
