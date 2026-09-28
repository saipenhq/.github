# SAIPEN HQ Public Setup — Current State

<!-- SAIPEN_HQ_PUBLIC_STATE:BEGIN
Durable checkpoint for the current public-identity/community setup.
Agents/maintainers: read this before repeating organization/profile/README cleanup.
Only update facts after verifying GitHub's live state.
SAIPEN_HQ_PUBLIC_STATE:END -->

## Status

**Phase:** CURRENT / STABLE

The public structure is established and intentionally split:

- **SAIPEN HQ** — organization / ecosystem identity: https://github.com/saipenhq
- **vacterro** — author and current owner of the project repositories: https://github.com/vacterro
- **SAIPEN Community** — Discord discussion layer: https://discord.gg/SEYaYkuVgN

## Completed

- `saipenhq/.github` exists and is public.
- Organization profile is published from `profile/README.md`.
- Shared organization defaults exist for contributing, support, security,
  community conduct, pull requests, and issue routing.
- Canonical project map, branding/link contract, organization settings,
  migration policy, and maintenance contract exist under `docs/`.
- Every active public `vacterro` repository has an intentional project-network
  bridge to SAIPEN HQ / SAIPEN Core / ZAICODE / FastPrompter / Discord.
- Archived repositories were intentionally left archived and were not revived
  for branding.
- `vacterro/vacterro` acts as the personal/public project index and links to
  SAIPEN HQ.
- The former staged SAIPEN HQ profile copy now points to the live canonical
  organization source instead of competing with it.
- ChatGPT Codex Connector is installed for both `vacterro` and `saipenhq`;
  SAIPEN HQ installation is configured for all organization repositories.

## Canonical files

- [Project map](PROJECTS.md)
- [Branding and links](BRANDING.md)
- [Organization settings](ORG_SETTINGS.md)
- [Repository migration policy](REPOSITORY_MIGRATION.md)
- [Public metadata maintenance](MAINTENANCE.md)

## Remaining operator-only gate

GitHub repository **Description** and **Topics** are repository settings, not file
content. The currently available connector can read them but does not expose the
repository-settings write endpoint.

Desired values are already prepared at:

- https://github.com/vacterro/vacterro/blob/main/docs/repository-metadata.json

Safe preview/apply helper:

- https://github.com/vacterro/vacterro/blob/main/tools/apply-repository-metadata.ps1

Run from a local clone of `vacterro/vacterro` with authenticated GitHub CLI:

```powershell
powershell -ExecutionPolicy Bypass -File .\tools\apply-repository-metadata.ps1
powershell -ExecutionPolicy Bypass -File .\tools\apply-repository-metadata.ps1 -Apply
```

The first command is preview-only. The second applies the prepared descriptions
and topics.

This is the only known broad public-metadata item left unapplied at this
checkpoint. Do not redesign the ecosystem because this one GitHub settings
surface still needs an operator-capable API/CLI.

## Not currently authorized

The following are intentionally **not** implied by this setup:

- bulk transfer of repositories into SAIPEN HQ;
- renaming independent products to SAIPEN-prefixed names;
- enabling organization bureaucracy merely because GitHub offers it;
- publishing private contact information;
- reviving archived repositories.

Future work should be driven by a concrete need, not by the existence of another
settings page.
