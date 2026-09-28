# SAIPEN HQ Public-Metadata Maintenance

<!-- SAIPEN_HQ_PUBLIC_MAINTENANCE:BEGIN
Operational contract for keeping public GitHub/Discord navigation coherent.
Agents/maintainers: prefer updating canonical sources over ad-hoc per-repository prose.
Do not broaden scope into repository transfers or product rewrites without explicit approval.
SAIPEN_HQ_PUBLIC_MAINTENANCE:END -->

The goal is simple: public identity should stay coherent without becoming a second product.

## Canonical sources

1. **Organization profile:** `profile/README.md`
2. **Project taxonomy:** `docs/PROJECTS.md`
3. **Names and links:** `docs/BRANDING.md`
4. **Organization settings intent:** `docs/ORG_SETTINGS.md`
5. **Repository-transfer boundary:** `docs/REPOSITORY_MIGRATION.md`
6. **Shared contribution/security/support defaults:** repository root files

When these disagree, fix the canonical source first, then update downstream copies.

## When a project changes

For a new or materially changed public project:

1. verify the repository-local README describes the real implementation;
2. update `docs/PROJECTS.md` if taxonomy or ownership changed;
3. update the profile only if the project belongs in a visible flagship/infrastructure list;
4. update the managed project-network bridge if the global navigation contract changed;
5. update GitHub description/topics to match the repository's current purpose;
6. keep Discord as discussion routing, not the sole durable record.

## README bridge rule

The `VACTERRO_PROJECT_BRIDGE` block in active public repositories is managed
navigation. It may be refreshed mechanically when canonical links change.

Do not rewrite the rest of a repository README merely to make formatting uniform.
Repository-local technical truth matters more than cosmetic symmetry.

## Description/topic drift

The current vacterro-side desired metadata is recorded in
`vacterro/vacterro/docs/repository-metadata.json`.

The companion script
`vacterro/vacterro/tools/apply-repository-metadata.ps1` previews differences by
default and writes only with `-Apply`.

If connector capabilities later gain repository-metadata writes, the manifest
remains the desired-state input; do not invent a second source.

## Organization growth

Do not add process because a checkbox exists.

Introduce teams, branch policies, Discussions, Projects, or repository transfers
only when a concrete collaboration or maintenance need appears. A one-person
organization does not need enterprise cosplay.

## Verification

A public-metadata maintenance pass is complete when:

- `saipenhq/.github` is public;
- the organization profile renders from `profile/README.md`;
- canonical project/branding/settings documents agree;
- active repository bridges point to SAIPEN HQ and the community;
- no archived repository was revived only for branding;
- GitHub descriptions/topics have either been applied or are explicitly tracked
  in the canonical metadata manifest;
- no ownership claim exceeds GitHub's actual repository owner.
