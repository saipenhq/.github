# SAIPEN HQ Public Setup — Current State

<!-- SAIPEN_HQ_PUBLIC_STATE:BEGIN
Durable checkpoint for the current public-identity/community setup.
Agents/maintainers: read this before repeating organization/profile/README cleanup.
Only update facts after verifying GitHub's live state.
SAIPEN_HQ_PUBLIC_STATE:END -->

## Status

**Phase:** DONE / STABLE

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

## Repository metadata

Repository **Description** and **Topics** were applied from the canonical manifest and verified by a final idempotent preview:

```text
changed=0 unchanged=34 failed=0 mode=PREVIEW
```

Desired values remain recorded at:

- https://github.com/vacterro/vacterro/blob/main/docs/repository-metadata.json

The sync helper remains available for future drift checks:

- https://github.com/vacterro/vacterro/blob/main/tools/apply-repository-metadata.ps1

## Not currently authorized

The following are intentionally **not** implied by this setup:

- bulk transfer of repositories into SAIPEN HQ;
- renaming independent products to SAIPEN-prefixed names;
- enabling organization bureaucracy merely because GitHub offers it;
- publishing private contact information;
- reviving archived repositories.

Future work should be driven by a concrete need, not by the existence of another
settings page.
