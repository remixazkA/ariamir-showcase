# Public Disclosure Policy

Ariamir separates **proof of existence and capability** from **proprietary implementation**.

## Safe to publish

Subject to normal privacy, licensing and partner-approval checks: high-level capability descriptions, boxes-and-arrows architecture diagrams, sanitized UI screenshots and demo recordings, public benchmark methodology, approved benchmark results, hardware compatibility reports, fictitious workflow examples, public roadmap items, release notes and sponsor/partner acknowledgements approved for publication.

## Keep private

- Fabric source code.
- Routing heuristics, scoring and fallback logic.
- System prompts and private worker prompts.
- Permission-engine internals.
- Private schemas and protocols where disclosure would enable reconstruction.
- Proprietary worker source.
- Secrets, credentials, tokens and production configuration.
- Private datasets, user content or customer information.
- Debug dumps containing private paths, machine identifiers or secrets.
- Unpublished partner information.
- Implementation details considered differentiating IP.
- Internal milestone plans, handoff records, validation logs and links into private product repositories.
- Runtime protocols, ownership maps and technical contracts that expose implementation architecture.

## Reporting development progress

Publish the practical capability, its reviewed date and its status: implemented in development builds, in validation, or roadmap. A milestone number may identify progress, but must not stand in for acceptance evidence. If later validation reopens a finding, an earlier passing run must not be presented as current completion.

Describe the product outcome rather than reproducing private plans or implementation diagrams. Keep the running installation's health separate from the state of a development branch. Do not expose machine-specific diagnostics, internal test totals or private repository links as promotional evidence.

## Screenshot checklist

Before adding a screenshot or video:

1. Remove usernames, email addresses and personal identifiers unless intentionally public.
2. Remove local filesystem paths that reveal private structure.
3. Remove API keys, tokens, account IDs and private endpoints.
4. Remove private prompt text and routing/debug panels.
5. Verify visible documents and filenames are redistributable.
6. Check browser tabs, notifications, taskbar items and background windows.
7. Confirm partner logos or product claims are approved for public use.

## Benchmark checklist

Before publishing a benchmark:

1. Define the metric.
2. Record hardware and relevant software versions.
3. Use repeatable workload parameters.
4. Run enough samples to avoid a one-off result.
5. Separate measured numbers from subjective impressions.
6. Do not expose private prompts or production datasets.
7. Identify sponsored/evaluation hardware where appropriate.

## Rule of thumb

> Publish what Ariamir does, the results it achieves and the hardware it works with. Do not publish the implementation that creates the project's advantage.
