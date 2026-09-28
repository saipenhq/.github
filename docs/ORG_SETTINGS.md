# SAIPEN HQ Organization Settings

<!-- SAIPEN_HQ_ORG_SETTINGS:BEGIN
Canonical desired public organization settings.
Some values live in GitHub account settings rather than repository files and may
require manual application. This document records intent so later agents do not guess.
SAIPEN_HQ_ORG_SETTINGS:END -->

## Public identity

- **Organization handle:** `saipenhq`
- **Display name:** `SAIPEN`
- **Short description:** `Practical infrastructure for long-running AI-agent work.`
- **Website:** `https://github.com/vacterro/saipen`
- **Community:** `https://discord.gg/SEYaYkuVgN`
- **Public profile source:** `.github/profile/README.md`

## Repository policy

- Keep `saipenhq/.github` public.
- Repository-local community files override organization defaults.
- Do not transfer repositories into the organization without explicit per-repository approval.
- Do not publish private contact addresses merely to fill an organization field.

## Shared defaults currently maintained here

- organization profile;
- contribution guide;
- support routing;
- security policy;
- community conduct;
- pull-request template;
- bug/feature issue forms.

## GitHub App access

The ChatGPT Codex Connector is intentionally installed for the SAIPEN HQ
organization with access to all organization repositories. Removing or narrowing
that installation can prevent automated maintenance of organization-owned
repositories.

This file records desired state; GitHub's live settings remain authoritative.
