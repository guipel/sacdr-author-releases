# Changelog

## [1.1.0] - 2026-11-03

- **`DSD128` / `DSD256` / `DSD512` → `DSD64` Downsampling** — Built-in, zero-dependency 64-bit linear-phase FIR + 5th-order Scarlet Book Delta-Sigma Modulator automatically converts `DSD128` (`5.64 MHz`), `DSD256` (`11.29 MHz`), and `DSD512` (`22.58 MHz`) tracks across `.dsf`, `.dff` (`DSD` & `DST`), and `.cue` inputs to hardware-playable `DSD64` (`2.82 MHz`), while keeping native `DSD64` sources 100% bit-perfect with zero DSP.
- **`.dff` (`DSDIFF`) Support** — Native authoring and verification of `.dff` files, supporting both uncompressed `DSD` and lossless `DST`-compressed streams (including commercial Philips/Sony `DST` bitstreams), automatic channel-order normalization, and metadata extraction from embedded `ID3` and `DIIN` chunks.
- **`.cue` Sheet Support** — Direct authoring and verification of single-file `.dff`/`.dsf` album images + `.cue` (exact `75 fps` frame slicing) as well as multi-file `.cue` tracklists (`TITLE`, `PERFORMER`, `ISRC`, `CATALOG`, `REM DATE`, `REM GENRE`).
- **Transparent DSP Mode Indicator & Deterministic Verification** — Contextual studio header badge (`Native 1-Bit DSD · Zero DSP`, `SDM Downsample`, and per-zone mixed Hybrid indicators), per-track format badges (`DSD256 → DSD64`), automatic post-build verification enabled by default, **About & License** dialog, and deterministic `SDM Exact` / `Bit-Exact` source verification.
- **Native Application Icons Across Windows, macOS & Linux** — Embedded high-DPI application icons in Windows `.exe` binaries, macOS `SACDR Author.app` bundles, and Linux window manager / `.desktop` packages.

## [1.0.0] - 2026-10-30

- **Desktop App (`sacdr-author-gui`)** — Visual authoring and verification studio with **Dark** and **Light** themes, drag-and-drop `.dsf` folder loading, inline metadata editing, live single-layer `4.7 GB` DVD fit estimation, unified `0–100%` build + verify progress, and one-click update notifications.
- **Command-Line Tool (`sacdr-author-cli`)** — Batch authoring (`Stereo`, `Multi`, `Hybrid`), disc inspection (`Inspect`), and bit-for-bit audio verification (`Verify`).
- **Universal `SACD-R` Player Compatibility** — Authors `2.0 Stereo`, `5.0 / 5.1 Surround`, and **Dual-Zone** `.iso` disc images with multi-core bit-perfect lossless compression and disc-bridge compatibility for universal `SACD-R` transports.
- **Standalone Multi-OS Packages** — Self-contained downloads for **Windows (`x64`)**, **macOS (`ARM64` & `x64` `SACDR Author.app`)**, and **Linux (`x64` & `ARM64`)** with `SHA256SUMS.txt`.
