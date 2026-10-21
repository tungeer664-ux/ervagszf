# Predictive Input Buffer (PgUp / PgDn version)

Original mod by lilWC. Only change: stage keys are PgUp / PgDn instead of F6, edge-detected and only while the game window is focused.

Stages: 0 = OFF (raw input), 1 = 2 ticks (wave 2), 2 = 4/4, 3 = 8/8, 4 = 16 (wave 8).
PgUp = next stage, PgDn = previous. A console window prints "SAVED +N TICKS" whenever a click was held back.

## Build (easiest: GitHub Actions, nothing to install)
1. Create a GitHub repo and upload everything in this folder (keep the .github folder).
2. Actions tab -> "Build Geode Mod" -> Run workflow.
3. Download the build artifact, copy the .geode file to `...\Geometry Dash\geode\mods\`.

## Build locally
`geode sdk install`, `geode sdk install-binaries`, then `geode build` in this folder.

## Notes
- mod.json uses gd "*" so Geode does not reject your GD version. The code is compiled against whatever GD version your Geode SDK supports; if the SDK has no bindings for your GD build, the build fails or the hooks won't match.
- Offline practice only. Do not use it on submitted records.
