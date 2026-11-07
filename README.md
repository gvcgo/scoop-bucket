# vmr Scoop bucket

Scoop bucket for [`vmr`](https://github.com/gvcgo/version-manager) - a cross-platform SDK version manager.

## Install

```powershell
scoop bucket add gvcgo https://github.com/gvcgo/scoop-bucket
scoop install gvcgo/vmr
```

## Layout

- `bucket/vmr.json` is the manifest, refreshed by the Excavator workflow after each vmr release.

Status: bootstrap - the manifest appears after the first release that ships Windows zip artifacts.
