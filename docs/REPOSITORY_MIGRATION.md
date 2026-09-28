# Repository Migration Policy

<!-- SAIPEN_HQ_MIGRATION_POLICY:BEGIN
This is a planning guard, not an instruction to transfer repositories.
Agents/maintainers: do not initiate repository transfers from this document.
A transfer requires an explicit operator decision for the named repository.
SAIPEN_HQ_MIGRATION_POLICY:END -->

SAIPEN HQ currently acts as the ecosystem and organization home while project
repositories remain under `vacterro`.

That is a valid steady state. Migration is optional.

## Why not move everything immediately

A repository transfer can affect:

- git remotes and local automation;
- GitHub Actions permissions and secrets;
- package/release integrations;
- badges and hard-coded repository URLs;
- branch protection and repository rules;
- installed GitHub Apps;
- external documentation and downloads;
- contributor expectations and ownership language.

GitHub redirects reduce link breakage, but they do not prove every integration is
safe.

## Good candidates for a future transfer

A repository is a good candidate when most of these are true:

1. it is clearly part of the SAIPEN core/infrastructure layer;
2. its public identity benefits from organization ownership;
3. current release and automation paths have been inventoried;
4. repository-specific secrets/rules/apps can be recreated or verified;
5. local clones and deployment tooling can tolerate a remote change;
6. the operator explicitly approves that repository's transfer.

Likely candidates include SAIPEN Core, ZAICODE, SAIPAL, SAIMAIL, SAIPENVIEW, and
AUDAPACK. This list is descriptive, not authorization.

## Keep under vacterro by default

Independent personal tools, creative utilities, experiments, and unrelated
products should stay under `vacterro` unless there is a concrete reason to move
them.

FastPrompter, ProTrail, Wintage, media tools, game tools, and similar projects can
participate in the shared network without organization ownership.

## Transfer checklist

Before transferring one repository:

1. record current owner, default branch, releases, Actions, rules, secrets/apps,
   package publishing, webhooks, and important hard-coded URLs;
2. verify a clean working tree in important local clones;
3. transfer only the named repository;
4. update local `origin` remotes where useful rather than relying forever on redirects;
5. re-check Actions, release downloads, GitHub Apps, branch protection, and badges;
6. update the project map and ownership wording only after GitHub confirms the new owner.

No bulk-transfer operation should be inferred from `goal cc all`, maintenance
mode, or a generic cleanup request.
