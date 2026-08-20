# TU/e FAIR Data Clinic Toolkit

Public release repository for the TU/e FAIR Data Clinic Toolkit standalone proof of concept.

## Release status

The final locked standalone development baseline is **v5.9.0-dev9**.

Authoritative locked artifact:

`fair-raps-researcher-toolkit_5_9_0-dev9.html`

Authoritative SHA-256:

`3bc3d31600eaccfd37d5a11e171a9276ab0973f57e5608b8aff377b6778a0001`

DEV9 remains byte-for-byte unchanged. It is preserved as the historical standalone baseline and as development provenance for the successor platform work.

### Recommended public-facing standalone artifact

A public review identified that the locked standalone toolkit embeds a dated TU/e departmental Data Steward directory containing individual names and email addresses. Because DEV9 is immutable, that historical artifact has not been silently modified.

The recommended public-facing standalone artifact is therefore the separately versioned correction:

`fair-raps-researcher-toolkit_5_9_0-dev9-public-hotfix1.html`

SHA-256:

`a4426144597d0b5a36cca7f05674347c3830cc499896f71432f0d552fefe0452`

This bounded correction removes the embedded named departmental Data Steward directory and replaces the corresponding directory-specific integrity tests with neutral equivalents. It retains the DEV9 assessment, workflow, and repository-preparation model. It is still a TU/e FAIR Data Clinic standalone proof of concept and should not be interpreted as the fully institution-neutral RORA architecture.

## Historical predecessor

**v5.8.0-rc15 — Final stabilization candidate of the v5.8 line**

Artifact:

`fair-raps-researcher-toolkit_5_8_0-rc15.html`

RC15 is retained for release history. It is superseded by the locked v5.9.0-dev9 standalone baseline and should not be treated as the current development authority.

## What the standalone toolkit does

The toolkit supports pre-deposit Dataset Content and Reuse Readiness assessment within a combined Researcher and Data Steward workflow. It evaluates research-data package structure, documentation, metadata, provenance, software, rights, access information, and relationships before repository deposit.

It does not calculate or certify a FAIR score, does not provide institutional approval, and does not make a live repository connection. DEV9 adds a deterministic offline 4TU.ResearchData deposit-preparation adapter; it performs no live repository connection, credential handling, DOI operation, file transfer, or repository write-back.

The application is self-contained. Download the selected HTML artifact and open it in a modern browser.

SHA-256 checksums for all public HTML artifacts are maintained in `SHA256SUMS.txt`.

## Successor development

The standalone FAIR Data Clinic lineage is being succeeded by the institution-neutral **RORA Platform — Research Object Readiness and Assessment Platform**. RORA Core separates institution-neutral assessment behavior from optional institutional configuration and repository adapters. Historical DEV9 branding and provenance are retained rather than retroactively renamed.

This public repository contains curated public artifacts. Active platform development, development branches, CI materials, and unreleased development versions are maintained separately.

## License

Released under the MIT License. See `LICENSE`.

Copyright © 2026 Richard Dennis.
