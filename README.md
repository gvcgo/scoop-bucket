# vmr Scoop bucket

Scoop bucket for [`vmr`](https://github.com/gvcgo/version-manager) - a cross-platform SDK version manager.

## Install

```powershell
scoop bucket add gvcgo https://github.com/gvcgo/scoop-bucket
scoop install gvcgo/vmr
```

The manifest ships the prebuilt Windows binaries (x64 / ARM64), so nothing is compiled locally.
Scoop only provides `vmr.exe`; vmr installs the SDK versions themselves under `%USERPROFILE%\.vmr`.

## Layout

- `bucket/vmr.json` is rendered from `vmr/packaging/scoop/vmr.json.in` in the
  [version-manager](https://github.com/gvcgo/version-manager) repository and pushed here by that
  repository's release workflow (`.github/workflows/release.yml`, job `scoop`).
  Do not edit it by hand.

## Updating

Every published vmr release rewrites `bucket/vmr.json`, including the archive hashes. Run
`scoop update` to pick up the new manifest.
