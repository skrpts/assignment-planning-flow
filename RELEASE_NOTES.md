# Release Notes

## v1.2.26
GH#845 — republish with American English (en-US) content, completing the source-only GH#805 flip that never reached the Hub. Copy only — no functional or behaviour change.

## v1.2.25
GH#745 — declare per-step `output: {name, type}` on every execution step (assignment_plan/text, notes/text, polished_plan/text). Lights up the #744 rich flow-map with named, typed outputs. Content-only; no bindings or logic changes.

## v1.2.24
GH#645 Row 3b — migrate to K-037 dep-referenced schema. Strip 10 inline shared-content files and declare 10 hub-shared deps (UUID id + slug name + version + checksum from `gen-dep-checksums.mjs`). Closes pre-Step-3 inline-vendoring for this bundle.

## v1.2.23
Wave 2: re-signed with canonical engine signing pipeline.

## v1.2.22
Tags migrated inline into manifest (GH#586). tags.yaml retired.

## v1.2.21
Bundle re-signed with canonical engine signing pipeline (Wave 2 migration).

## v1.2.20
Signature fix — RELEASE_NOTES.md now included in integrity checksum.

## v1.2.19
Initial catalog release with full structural and content-quality validation. All scanner checks pass.
