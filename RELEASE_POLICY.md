# Release policy

- GitHub Releases is the **only canonical binary distribution channel** for VBAUpdater.
- Binary installers and update ZIP files must not be committed to the `main` branch.
- Every release uses a new semantic version, exact Git tag, immutable Release assets, and SHA-256 evidence.
- `latest.json` is the only mutable self-update pointer and must reference the exact GitHub Release asset URL.
- SHA-256 in `latest.json` must match the immutable self-update ZIP attached to the GitHub Release.
- The first customer-facing release must contain both a fresh-install Setup EXE and a self-update ZIP in the same GitHub Release.
- Release publication requires an explicit artifact-bound authorization and must fail closed on tag, asset filename, SHA-256, draft/prerelease, or authorization drift.
- Release publication authority is owned by Business Platform; this repository does not contain an independent release-publishing workflow.
- Development source is never published in this repository.
- Legacy `releases/*.zip` files from the pre-GitHub-Releases migration are intentionally removed from the current branch. Their historical Git objects remain only in repository history and are not distribution endpoints.
