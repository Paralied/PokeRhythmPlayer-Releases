# Poke Rhythm Player

[Download PokeRhythmPlayer.exe](https://github.com/Paralied/PokeRhythmPlayer-Releases/raw/refs/heads/main/PokeRhythmPlayer.exe)

Download once and open the EXE. No ZIP or installer. This small Windows app
uses the .NET Framework runtime installed on your PC.

The app checks for updates on launch. When a newer version is published,
click **Update & restart**. Your settings are preserved. Keep the EXE in a
folder your account can write to, such as a dedicated folder under Documents.

Choose an instrument, focus Roblox, then press **F8**. **F9** stops.

## Version 1.0.20.0

- Fix approaching notes being discarded too early during a hold.
- Preserve consecutive hold-note presses while preventing duplicate presses of the current hold.
- Use **Check for updates**, then **Update & restart**.

## Version 1.0.19.0

- Fix duplicate detections interrupting long-note holds.
- Preserve independently tracked next notes until tail completion.
- Use **Check for updates**, then **Update & restart**.

## Version 1.0.18.0

- Fix automatic timing stalling during dense passages.
- Improve long-note recognition, speed tracking and release handling.
- Install through **Check for updates**, then **Update & restart**.
- [Full change notes](CHANGELOG.md).

## Version 1.0.17.0

- Single-EXE distribution and built-in update checking.
- Update download verification and replacement with a temporary backup.
- Existing black/flame interface, note detection and automatic timing.

This repository contains only public downloads and update metadata. Source is
maintained separately in a private repository. Core tests and compilation
passed; Windows update handoff/restart is not yet verified on a live desktop.
Automatic timing does not guarantee perfect scores.


Will take down upon request, small project of coding in my free time
