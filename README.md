# SweepBar — Releases

Public downloads and the [Sparkle](https://sparkle-project.org) auto-update feed
for **SweepBar**, a menu-bar utility for safe, scan-first macOS cleanup.

## Download

**[Download the latest release →](https://github.com/jjnicolas/sweep-releases/releases/latest)**

Unzip and move `SweepBar.app` to `/Applications`. It's Developer ID signed and
notarized by Apple, and updates itself from here via Sparkle.

## What's in this repo

| File | Purpose |
|------|---------|
| `appcast.xml` | The Sparkle feed (`SUFeedURL`) the app polls for updates. |
| `SweepBar-X.Y.Z.zip` | Notarized app builds, one per version. |
| `SweepBarN-M.delta` | Sparkle binary deltas (build *M* → *N*) for smaller updates. |

Each download in the appcast is signed with an EdDSA key; the app verifies the
signature against its embedded public key before installing.

## Source & docs

Source code, the `sweep` CLI, and full documentation live in
**[jjnicolas/sweep](https://github.com/jjnicolas/sweep)**.

---

*These files are generated and pushed by `make release` in the source repo —
they aren't edited by hand.*
