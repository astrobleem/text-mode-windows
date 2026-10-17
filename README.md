# Windows 3.0 text-mode display profiles (experimental)

This repository is a documentation front door for experimental 80-column Windows 3.0 text-mode profiles. The implementation, detailed design, and any future package live in the canonical [oemdisplay-tandy project](https://github.com/astrobleem/oemdisplay-tandy).

## Availability

The canonical project's [Display modes section](https://github.com/astrobleem/oemdisplay-tandy#display-modes) lists merged experimental text-mode profiles with emulator evidence, but states that no current TEXT80/C25 binary package has been released. There is no download in this repository.

The documented profiles include TEXT80 25 (80x25), TEXT80 PAN (an 80x25 view over a 640x400 desktop), TEXT80 VGA (80x50 on VGA), and the compact C25 profile. The results and limits are emulator-based; consult the detailed record before treating any profile as suitable for a particular machine. Physical hardware is not qualified.

## Source and test record

- [TEXT80 design, profiles, tests and limitations](https://github.com/astrobleem/oemdisplay-tandy/blob/main/docs/TEXT80.MD)
- [PR #133: TEXT80 80-column profiles](https://github.com/astrobleem/oemdisplay-tandy/pull/133)
- [PR #134: compact C25 profile](https://github.com/astrobleem/oemdisplay-tandy/pull/134)
- [Canonical project releases](https://github.com/astrobleem/oemdisplay-tandy/releases)
- [Canonical project issue tracker](https://github.com/astrobleem/oemdisplay-tandy/issues)

The older rc.6 TXTMODE feasibility driver is historical and separate from the current TEXT80/C25 source; it is not a released TEXT80/C25 package. This repository contains no driver binaries or duplicated implementation.