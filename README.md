# EasyTier iOS build

This public repository holds only a GitHub Actions workflow (`.github/workflows/ios-build.yml`).
It builds the private EasyTier iOS source on GitHub's macOS runners. The source is checked out
with a read-only deploy key, and the build log and the unsigned IPA are uploaded encrypted, so
nothing readable is published here. The workflow is started by hand only (`workflow_dispatch`).

Secrets (set on this repository): `SOURCE_DEPLOY_KEY`, `CORE_SSH_KEY`, `ARTIFACT_KEY`.
