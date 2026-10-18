# Windows 3.0 text-mode display profiles

**[Download TEXT80.ZIP](https://raw.githubusercontent.com/astrobleem/oemdisplay-tandy/main/downloads/experimental/TEXT80/TEXT80.ZIP)** · [Install and rollback guide](https://github.com/astrobleem/oemdisplay-tandy/blob/main/downloads/experimental/TEXT80/README.MD) · [Detailed behavior and limits](https://github.com/astrobleem/oemdisplay-tandy/blob/main/docs/TEXT80.MD)

TEXT80.ZIP is an experimental **repository-file download**, not a GitHub Release asset. It is a 389,919-byte package (SHA-256 `cd892a48db2973e7c99f4d6a00977cfe7e2466699baa5afcd4baf977aa2a30b9`) for Windows 3.0 real mode on 8086/8088 systems with 640 KB. It includes TEXT80 80×25, a 640×400 panning desktop, VGA 80×50, and compact C25 profiles.

Extract the complete `TEXT80` folder to `C:\\TEXT80`. From plain DOS, run `T80ON C:\\WINDOWS C25` (substitute your Windows directory), then start Windows with `WIN /R` after setup succeeds. Exit Windows and run `T80OFF C:\\WINDOWS` from the extracted folder to undo. Keep the state files until rollback completes; the guide covers recovery and profile changes.

[![86Box capture of Windows 3.0 Notepad in TEXT80 C25 80×25 on an IBM XT/CGA](https://raw.githubusercontent.com/astrobleem/oemdisplay-tandy/1dc95619dde79663d0e1d9e1c7d251b00978b7ed/docs/text80/RUN_c3/c80w3/notepad.png)](https://github.com/astrobleem/oemdisplay-tandy/blob/1dc95619dde79663d0e1d9e1c7d251b00978b7ed/docs/text80/RUN_c3/c80w3/notepad.png)

86Box 6.0 build 9001 · emulated IBM XT/CGA, 8088 at 4.77 MHz · Windows 3.0 C25 at 80×25. This screenshot is from the recorded 54/54 Windows GUI session; the tested evidence is pinned to [commit 1dc9561](https://github.com/astrobleem/oemdisplay-tandy/commit/1dc95619dde79663d0e1d9e1c7d251b00978b7ed). Emulator evidence only; physical hardware is not qualified.

**Test scope:** C25 in the download is byte-identical to the recorded GUI-tested driver. The current 25, PAN and VGA driver bytes have fresh build/link audits and presenter checks, but were not booted in Windows for this package. Scrolling is slow; graphics and larger fonts appear as block approximations. C25 compact controls align exactly only on the text-cell grid. This package does not replace Windows XT rc.6 or its historical TXTMODE experiment.

[Canonical development repository](https://github.com/astrobleem/oemdisplay-tandy) · [source snapshot](https://github.com/astrobleem/oemdisplay-tandy/tree/997e7b910eb4623226b676c1c229aa0dd4e81661/src/text80) · [package build and qualification](https://github.com/astrobleem/oemdisplay-tandy/blob/main/tools/EXPPUB/QUALIFY.JSN) · [issue tracker](https://github.com/astrobleem/oemdisplay-tandy/issues)

Windows/DOS media, Microsoft fonts, retail grabber, ROMs, compilers and emulators are not included. Display-driver derivative notices apply; the included XT Pixels fonts are original MIT-licensed work.
