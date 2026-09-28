# SAIPEN HQ Branding and Link Contract

<!-- SAIPEN_HQ_BRANDING:BEGIN
Canonical naming/link contract for public SAIPEN HQ documentation.
Agents/maintainers: preserve these identities unless the operator explicitly changes them.
Do not mechanically rename independent products to SAIPEN-prefixed names.
SAIPEN_HQ_BRANDING:END -->

This is intentionally small. Branding should make projects easier to understand,
not create another framework that needs a framework maintainer.

## Canonical identities

| Purpose | Canonical value |
|---|---|
| Ecosystem / organization display name | **SAIPEN** |
| GitHub organization handle | **saipenhq** |
| Organization URL | https://github.com/saipenhq |
| Core protocol repository | https://github.com/vacterro/saipen |
| Author / full project index | https://github.com/vacterro |
| Community | https://discord.gg/SEYaYkuVgN |

Use **SAIPEN HQ** when referring specifically to the GitHub organization.
Use **SAIPEN** when referring to the protocol/ecosystem brand in prose.

## Product names

Existing product names stay product names:

- SAIPEN
- ZAICODE
- FastPrompter
- LIMISAW
- SAITULS
- ProTrail
- AUDAPACK
- SAIPAL
- SAIMAIL
- SAIPENVIEW

Do not rename independent products simply to make every repository start with
`SAI`. Consistent navigation matters more than forced naming symmetry.

## Repository bridge

Active public repositories in the vacterro network may carry the managed
`VACTERRO_PROJECT_BRIDGE` block. Its purpose is to provide a stable route to:

- Author hub
- SAIPEN HQ
- SAIPEN Core
- ZAICODE
- FastPrompter
- SAIPEN Community
- repository-specific GitHub Issues

The block is intentional public documentation, not unexplained drift. If the
navigation scheme changes, replace it deliberately across the network rather than
allowing each agent to invent a new footer.

## Descriptions and topics

Repository descriptions should answer **what the project is** in one sentence.
Avoid slogans, version numbers, unsupported superlatives, and descriptions that
merely repeat the repository name.

Topics should be concrete search terms: platform, language/runtime, domain,
framework, and major workflow category. Do not add a `saipen` topic to an
unrelated tool solely for cross-promotion.

## Ownership language

Until a repository is actually transferred to the SAIPEN HQ organization:

- correct: “part of the SAIPEN ecosystem”
- correct: “connected to the SAIPEN / vacterro project network”
- incorrect: “owned by SAIPEN HQ”
- incorrect: “official SAIPEN HQ repository” unless GitHub ownership says so

GitHub redirects after a future transfer do not justify claiming that transfer
before it happens.

## Community routing

Use Discord for fast conversation, screenshots, rough ideas, and cross-project
discussion.

Use GitHub Issues for reproducible bugs and durable feature requests.

Use repository documentation for established behavior and contracts.

That separation is deliberately boring. Boring systems are easier to find six
months later.
