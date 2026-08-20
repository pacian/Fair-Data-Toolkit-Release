# TU/e FAIR Data Clinic Toolkit

Public release repository for the TU/e FAIR Data Clinic Toolkit standalone proof of concept.

## Release status

The final locked standalone development baseline is **v5.9.0-dev9**.

Authoritative locked artifact:

`fair-raps-researcher-toolkit_5_9_0-dev9.html`

Authoritative SHA-256:

`3bc3d31600eaccfd37d5a11e171a9276ab0973f57e5608b8aff377b6778a0001`

DEV9 must remain byte-for-byte unchanged. It is preserved as the historical standalone baseline and as development provenance for the successor platform work.

### Public personnel-directory correction

A public review identified that the standalone toolkit embeds a dated TU/e departmental Data Steward directory containing individual names and email addresses. This behavior is also present in the locked DEV9 artifact.

Because DEV9 is immutable, the locked artifact will not be silently edited. A separately versioned public correction will remove the embedded named personnel directory while preserving DEV9 assessment semantics, workflow behavior, and repository-preparation boundaries. The corrected derivative will have its own filename and checksum and will be clearly distinguished from locked DEV9.

Until that corrected derivative is published and verified, the historical DEV9 artifact should be interpreted as a proof-of-concept baseline rather than an institution-neutral deployment package.

## Historical predecessor

**v5.8.0-rc15 — Final stabilization candidate of the v5.8 line**

Artifact:

`fair-raps-researcher-toolkit_5_8_0-rc15.html`

RC15 is retained for release history. It is superseded by the locked v5.9.0-dev9 standalone baseline and should not be treated as the current development authority.

## What the standalone toolkit does

The toolkit supports pre-deposit Dataset Content and Reuse Readiness assessment within a combined Researcher and Data Steward workflow. It evaluates research-data package structure, documentation, metadata, provenance, software, rights, access information, and relationships before repository deposit.

It does not calculate or certify a FAIR score, does not provide institutional approval, and does not make a live repository connection. DEV9 adds a deterministic offline 4TU.ResearchData deposit-preparation adapter; it performs no live repository connection, credential handling, DOI operation, file transfer, or repository write-back.

The application is self-contained. Download the selected HTML artifact and open it in a modern browser.

SHA-256 checksums are maintained in `SHA256SUMS.txt`.

## Successor development

The standalone FAIR Data Clinic lineage is being succeeded by the institution-neutral **RORA Platform — Research Object Readiness and Assessment Platform**. RORA Core separates institution-neutral assessment behavior from optional institutional configuration and repository adapters. Historical DEV9 branding and provenance are retained rather than retroactively renamed.

This public repository contains curated public artifacts. Active platform development, development branches, CI materials, and unreleased development versions are maintained separately.

## License

Released under the MIT License. See `LICENSE`.

Copyright © 2026 Richard Dennis.
