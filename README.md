# Who Said What — installer downloads

Windows desktop app that transcribes meetings on your own PC and says who said what. Everything runs locally;
nothing is uploaded.

## Download

Go to **Releases** (right-hand side of this page) and download **all files** of the latest release into one folder:

- `WhoSaidWhat-Setup-<version>.exe`
- `WhoSaidWhat-Setup-<version>-1.bin`, `-2.bin`, `-3.bin` (the installer data, about 5.6 GB in total)

Then run the `.exe`. Windows SmartScreen will say "Windows protected your PC" because this test build is not
code-signed: click **More info**, then **Run anyway**. Installation takes about two minutes and needs no internet.

## What your PC needs

- Windows 10 (1809 or newer) or Windows 11, 64-bit
- An NVIDIA GPU with at least 6 GB of VRAM (GTX 10-series or newer; RTX 30/40/50 are fastest).
  Without an NVIDIA GPU the app installs but cannot transcribe.
- NVIDIA driver 525 or newer (RTX 50-series: 580 or newer): https://www.nvidia.com/drivers
- About 9 GB of free disk space, plus room for recordings
- A microphone. To transcribe online calls (Teams, Zoom, Meet, ...) turn on "system audio" in the app's settings.

## First start

The first start takes one to two minutes; later starts take about ten seconds. RTX 50-series GPUs see a
"Setting up Who Said What" screen once, which downloads about 2 GB (the only case that needs internet).

## Reporting a problem

Send `launcher.log` and `app.log` from `%LOCALAPPDATA%\WhoSaidWhat` (paste that path into the Explorer address bar)
together with what you did. A screenshot of the "Setting up Who Said What" screen, if it appears, helps too.

## Uninstall

Settings > Apps > Installed apps > Who Said What > Uninstall. Meetings, recordings and enrolled voices stay in
`%LOCALAPPDATA%\WhoSaidWhat`; delete that folder to remove them as well.
