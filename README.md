# VBAUpdater Releases

Public distribution repository for VBAUpdater.

Latest: 4.18.7

- canonical binary distribution: **GitHub Releases**
- current stable tag: `v4.18.7`
- self-update manifest: `latest.json`
- self-update package: `VBAUpdater_Update_4.18.7.zip`
- SHA-256: `7308CF0E853758A92F39438AD515EF828F00483E8CD25D77380D6116B86EE5B3`
- customer-ready fresh installer: not yet; required before first external customer distribution

## Repository role

This repository is public and contains only distribution metadata and release policy. VBAUpdater development source remains in the private `tanaka456jp/VBAUpdater` repository.

Binary packages are **not stored on the main branch**. Setup EXE and self-update ZIP files are published only as GitHub Release assets.

`latest.json` is the stable self-update pointer consumed by the VBAUpdater application. Future release writes are authorized and executed through the Business Platform release workflow.
