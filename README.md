# Windows 3.0 in text mode

**[Download TEXT80.ZIP](https://raw.githubusercontent.com/astrobleem/oemdisplay-tandy/main/downloads/experimental/TEXT80/TEXT80.ZIP)**

Run Windows applications through an 80-column text display. Start with **C25**
for compact controls on an 80x25 screen and a 640x200 logical desktop.
You need an existing Windows 3.0 real-mode installation, DOS, 640 KB and a
CGA-compatible color text adapter. Python is not needed on the XT.

## Install

Extract the complete `TEXT80` folder to `C:\TEXT80`. Exit Windows to plain DOS:

```bat
C:
CD \TEXT80
T80ON C:\WINDOWS C25
```

Use your actual Windows directory. Continue only after the setup success
message, then change to Windows before starting:

```bat
C:
CD \WINDOWS
WIN /R
```

Keep using any machine-specific memory guard required by your system before
every Windows start. TEXT80 does not reserve RAM.

## Change profiles or undo

Exit Windows, then run from the extracted folder:

```bat
C:
CD \TEXT80
T80OFF C:\WINDOWS
```

To choose another profile, run T80OFF first, then T80ON with **25** (ordinary
80x25), **PAN** (80x25 view over a 640x400 desktop) or **VGA** (VGA-only 80x50).
PAN needs about 100 KB more Windows memory; Alt+PgUp/PgDn or pointer-edge dwell
pans the view. No manual INI edits are needed. Keep SYSTEM.T80, WIN.T80 and
T80SET.STA until undo succeeds. The included INSTALL.TXT covers recovery.

## Known limits and technical details

Scrolling is slow; graphics and larger fonts become block approximations.
C25 controls fit exactly only on the text-cell grid. C25 matches the recorded
54/54 Windows GUI session on an emulated XT/CGA. Current 25/PAN/VGA builds
have host and presenter checks but await a fresh Windows run; physical adapter
coverage is unqualified. Windows 3.1 is not supported.

![Notepad using C25 in the XT/CGA emulator](https://raw.githubusercontent.com/astrobleem/oemdisplay-tandy/main/docs/text80/RUN_c3/c80w3/notepad.png)

[Detailed behavior](https://github.com/astrobleem/oemdisplay-tandy/blob/main/docs/TEXT80.MD) ·
[Package source and optional test records](https://github.com/astrobleem/oemdisplay-tandy/blob/main/downloads/experimental/TEXT80/README.MD) ·
[Development and issues](https://github.com/astrobleem/oemdisplay-tandy).
Component notices are in the packet.
