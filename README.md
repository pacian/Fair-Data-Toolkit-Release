# TU/e FAIR Data Clinic Toolkit

Public release repository for the TU/e FAIR Data Clinic Toolkit standalone proof of concept.

## Release status

The final locked standalone development baseline is **v5.9.0-dev9**. The recommended public-facing standalone artifact is **v5.9.0-dev9-public-hotfix1**.

### Important distinction between the two DEV9 artifacts

These two files have different purposes and should not be treated as interchangeable:

- **`fair-raps-researcher-toolkit_5_9_0-dev9.html` — locked historical/final standalone baseline.** This is the immutable DEV9 artifact preserved byte-for-byte for provenance, reproducibility, and development history. It intentionally remains exactly as it was released, including the dated embedded TU/e departmental Data Steward directory identified in public review. It is **not** the recommended public-facing version.
- **`fair-raps-researcher-toolkit_5_9_0-dev9-public-hotfix1.html` — recommended public-facing standalone artifact.** This is a separately versioned derivative of DEV9 created specifically to correct the embedded named-personnel directory. It removes that departmental personnel directory and replaces the corresponding directory-specific integrity tests with neutral equivalents while retaining the DEV9 assessment semantics, workflow behavior, and repository-preparation model.

The hotfix does **not** replace or rewrite the locked DEV9 provenance artifact. Conversely, locked DEV9 should not be interpreted as the preferred public deployment artifact now that the corrected derivative exists.

Neither file is the institution-neutral RORA Platform. The hotfix remains a TU/e FAIR Data Clinic standalone proof of concept; RORA is the successor architecture in which institution-specific configuration is separated from institution-neutral core behavior.

## Locked DEV9 provenance artifact

Artifact:

`fair-raps-researcher-toolkit_5_9_0-dev9.html`

SHA-256:

`3bc3d31600eaccfd37d5a11e171a9276ab0973f57e5608b8aff377b6778a0001`

DEV9 remains byte-for-byte unchanged and is preserved as the historical standalone baseline and as development provenance for successor platform work.

## Recommended public-facing standalone artifact

Artifact:

`fair-raps-researcher-toolkit_5_9_0-dev9-public-hotfix1.html`

SHA-256:

`a4426144597d0b5a36cca7f05674347c3830cc499896f71432f0d552fefe0452`

This bounded correction addresses the hard-coded Data Steward personnel directory reported during public review. It does not change the underlying DEV9 assessment model, workflow model, or repository-preparation boundaries.

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
