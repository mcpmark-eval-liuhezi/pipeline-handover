# Pipeline

This repository holds the handover package for the pipeline side project.

## Handover owner

**Handover owner:** Hezi Liu (@HeziLiu)

Hezi Liu is the current owner of this pipeline side project and is responsible for
the handover to the incoming maintainer. Any questions about the project's current
state, open work, or history should be directed to him until the handover is
complete.

## Where the project stands

The pipeline is in a stable, working state and ready to be picked up:

- The core pipeline behavior is unchanged and considered stable.
- A changelog ([CHANGELOG.md](../CHANGELOG.md)) is maintained with an `Unreleased`
  section that tracks pending changes.
- Continuous integration is in place at
  [`.github/workflows/build.yml`](../.github/workflows/build.yml). It runs on every
  push and can also be triggered manually; each run uploads a short text build
  manifest as the `build-manifest` artifact.
- Release readiness is tracked in the "Release readiness checklist" issue, with
  sub-issues for documentation and CI work.
- The legacy export path has been **descoped** and the associated cleanup task has
  been unlinked from the release checklist.
- No release has been cut yet; the incoming owner will cut the first release
  (planned as `v0.1.0`) themselves once they are comfortable with the state of the
  project.

## What the new owner should do next

1. Read this page and the `CHANGELOG.md` `Unreleased` section.
2. Verify CI is green on the default branch (`main`) and inspect the
   `build-manifest` artifact.
3. Review the "Release readiness checklist" issue and its remaining sub-issues.
4. Cut the first release (`v0.1.0`) when ready, moving the `Unreleased` changelog
   entries into the new version.
