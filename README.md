# Scoop bucket for vork

This bucket installs [vork](https://github.com/voyager-so/vork), a headless 3D and VFX engine for agents, on x64 Windows from the zip in its GitHub releases. Run `scoop bucket add voyager-so https://github.com/voyager-so/scoop-bucket` and `scoop install vork`, then `vork setup`, which can take a few minutes. vork is source-available under the [vork Preview License](https://github.com/voyager-so/vork/blob/main/LICENSE), not open source; the source, docs and issues are in the [main repository](https://github.com/voyager-so/vork).

## Updating for a new release

In `bucket/vork.json`, change `version` and the version in `url`, and copy the zip's `hash` from the release's `SHA256SUMS`. Scoop's `checkver.ps1 -Update` can do this from the `checkver` and `autoupdate` sections. Then run `scoop update vork`, `vork --version`, `vork setup` and a small render on Windows.
