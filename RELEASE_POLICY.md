# Release policy

- GitHub Releases is the canonical binary distribution channel for all new VBAUpdater releases.
- Every release uses a new semantic version, exact Git tag, immutable Release assets, and SHA-256 evidence.
- `latest.json` is the only mutable self-update pointer and must reference the exact GitHub Release asset URL.
- SHA-256 in `latest.json` must match the immutable self-update ZIP attached to the GitHub Release.
- Existing `releases/*.zip` files are legacy migration sources only; new versions must not be added to Git history as binary distribution files.
- The first customer-facing release must contain both a fresh-install Setup EXE and a self-update ZIP in the same GitHub Release.
- Release publication requires an explicit artifact-bound authorization and must fail closed on tag, asset filename, SHA-256, draft/prerelease, or authorization drift.
- Development source is never published in this repository.
