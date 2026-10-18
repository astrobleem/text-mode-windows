# Windows 3.0 text-mode display profiles (experimental)

This repository is a documentation front door for experimental 80-column Windows 3.0 text-mode profiles. The implementation, detailed design, and any future package live in the canonical [oemdisplay-tandy project](https://github.com/astrobleem/oemdisplay-tandy).

## Availability

The canonical project's [Display modes section](https://github.com/astrobleem/oemdisplay-tandy#display-modes) lists merged experimental text-mode profiles with emulator evidence; no current TEXT80/C25 binary package has been released. There is no download or install route yet. This page links to the published test evidence, but emulator results do not qualify physical hardware.

The documented profiles include TEXT80 25 (80x25), TEXT80 PAN (an 80x25 view over a 640x400 desktop), TEXT80 VGA (80x50 on VGA), and the compact C25 profile. The results and limits are emulator-based; consult the detailed record before treating any profile as suitable for a particular machine. Physical hardware is not qualified.

[![86Box capture of Windows 3.0 Notepad in TEXT80 80×25 on an IBM XT with CGA](https://raw.githubusercontent.com/astrobleem/oemdisplay-tandy/94e513fd1b00025acdaba95c3d87ef6db828a33e/docs/text80/RUN_r1/t80w3/notepad.png)](https://github.com/astrobleem/oemdisplay-tandy/blob/94e513fd1b00025acdaba95c3d87ef6db828a33e/docs/text80/RUN_r1/t80w3/notepad.png)

86Box 6.0 build 9001, IBM XT/CGA, 8088 at 4.77 MHz, Windows 3.0 TEXT80 80×25. The recorded session passed 51/51 checks; the screenshot, [session results](https://github.com/astrobleem/oemdisplay-tandy/blob/94e513fd1b00025acdaba95c3d87ef6db828a33e/docs/text80/RUN_r1/t80w3/T80WIN.JSN), driver identity ([T80PREP.JSN](https://github.com/astrobleem/oemdisplay-tandy/blob/94e513fd1b00025acdaba95c3d87ef6db828a33e/docs/text80/RUN_r1/t80w3/T80PREP.JSN)) and [evidence commit 94e513f](https://github.com/astrobleem/oemdisplay-tandy/commit/94e513fd1b00025acdaba95c3d87ef6db828a33e) are linked. This is emulator-only evidence; no physical hardware is qualified.

[![86Box capture of Windows 3.0 Notepad in TEXT80 C25 80×25 on an IBM XT/CGA](https://raw.githubusercontent.com/astrobleem/oemdisplay-tandy/1dc95619dde79663d0e1d9e1c7d251b00978b7ed/docs/text80/RUN_c3/c80w3/notepad.png)](https://github.com/astrobleem/oemdisplay-tandy/blob/1dc95619dde79663d0e1d9e1c7d251b00978b7ed/docs/text80/RUN_c3/c80w3/notepad.png)

86Box 6.0 build 9001, emulated IBM XT/CGA (8088 at 4.77 MHz), Windows 3.0 TEXT80 C25 at 80×25. The reviewed session passed 54/54 checks with exit status 0; see the [C25 test record](https://github.com/astrobleem/oemdisplay-tandy/blob/1dc95619dde79663d0e1d9e1c7d251b00978b7ed/docs/TEXT80.MD) and [tested evidence commit 1dc9561](https://github.com/astrobleem/oemdisplay-tandy/commit/1dc95619dde79663d0e1d9e1c7d251b00978b7ed). Emulator evidence only; physical hardware remains unqualified, and there is no public C25 download yet.

## Source and test record

- [TEXT80 design, profiles, tests and limitations](https://github.com/astrobleem/oemdisplay-tandy/blob/main/docs/TEXT80.MD)
- [PR #133: TEXT80 80-column profiles](https://github.com/astrobleem/oemdisplay-tandy/pull/133)
- [PR #134: compact C25 profile](https://github.com/astrobleem/oemdisplay-tandy/pull/134)
- [Canonical project releases](https://github.com/astrobleem/oemdisplay-tandy/releases)
- [Canonical project issue tracker](https://github.com/astrobleem/oemdisplay-tandy/issues)

The older rc.6 TXTMODE feasibility driver is historical and separate from the current TEXT80/C25 source; it is not a released TEXT80/C25 package. This repository contains no driver binaries or duplicated implementation.