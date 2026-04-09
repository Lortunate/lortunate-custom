# lortunte-custom

A custom Scoop bucket for personal use.

## Usage

```powershell
scoop bucket add lortunte https://github.com/lortunate/lortunate-custom
scoop install lortunte/<app>
```

## Path policy

Manifest `persist` entries define the real data location under `scoop\\persist\\<app>`.
If a path is exposed from `scoop\\apps\\<app>\\current`, it may be a junction into `persist`.
For app-level data/cache environment variables, this bucket prefers explicit `$persist_dir` paths.
