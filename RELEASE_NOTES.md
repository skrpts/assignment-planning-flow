# Release Notes

## v1.2.28
GH#1100 consumer wave (batch 1) — declare the data flow this workflow was resolving positionally.

Each stage below now receives its input through a declared `bindings:` entry instead of `default_from_previous`, which K-073 revoked. **The value is unchanged**: every binding names the step that immediately precedes it, which is exactly what the positional default resolved to. What changes is that the dependency is stated rather than inferred from position, so a reorder can no longer silently feed a stage the wrong artefact.

Bindings added:
  `take-notes` ← `from_step: "Study Planning"` (step 2)
  `polish-language` ← `from_step: "Note-Taking"` (step 3)

Dependency pins moved to the published versions that declare these slots:
  `critical-thinking-framework` 1.0.1 → 1.0.2
  `plan-studies` 1.0.3 → 1.0.4
  `polish-language` 1.0.1 → 1.0.7
  `practice-question-generator` 1.0.1 → 1.0.2
  `revision-timetable-template` 1.0.1 → 1.0.2
  `take-notes` 1.0.3 → 1.0.4

## v1.2.27
GH#1044 — document the inputs this workflow's prompts REQUIRE but its Inputs table never listed. A user supplying exactly what the table asked for was running with required parameters unsatisfied — a silent wrong run, not a documentation nicety. documented 3 input(s): module_name, study_material, topic. Every row is generated from the requiring prompt's own declared description, example and required flag — none invented. No behaviour change; documentation only.

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
