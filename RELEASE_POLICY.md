# Release policy

- Never overwrite an already-published `VBAUpdater_Update_<version>.zip`.
- Every update uses a new semantic version and a new filename/URL.
- `latest.json` is the only mutable pointer.
- SHA-256 in `latest.json` must match the immutable ZIP.
- Development source is never published in this repository.
