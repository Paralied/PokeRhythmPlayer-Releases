# Version 1.0.22.0

- Replace tail presence sampling inside the round head with narrow-bar scanning above it. Predict the trailing endpoint crossing and maintain an independent release deadline per lane; missing pixels do not restart that deadline.
- Separate same-hue scenery from the stem using width and local color/brightness contrast. Hold classification requires attachment to the head.
- Restore the pre-1.0.21 tap matching and sixteen-sample timing policy. Disable adaptive head-color changes and use the saved stable tolerance (default 55).
- Keep automatic bass/four-lane selection. Stationary matching is restricted to fired hold tracks, not ordinary approaching notes.

A new head-only regression fails against 1.0.21 and passes here. Tests cover distinct lane deadlines with concurrent taps, same-hue scenery, moving endpoints, missing observations, and recorded bass tail/background frames. Live Windows scoring and recovery of 96–98% drum accuracy remain unverified.

# Version 1.0.21.0

- Detect the instrument automatically from two or four receptors; select F/J or D/F/J/K and search again when the row changes.
- Recover fragmented receptor outlines and retain known receptors while held heads hide their letters.
- Permit verified separate incoming notes during a hold, with a brief release/press and continued sustain. Keep stationary held heads associated with their original tracks.
- Learn bounded color tolerance per lane from saturated moving head cores.
- Use eight readable judgments per timing trial instead of sixteen, with faster trial settling and early rejection; one Good among otherwise Perfect feedback does not start a new search.

Core regression tests passed, including recorded two- and four-lane frames and simulated overlapping holds. Live Windows gameplay accuracy is unverified; no perfect-score guarantee.

# Version 1.0.20.0

Fix premature rejection of approaching notes during holds, introduced in 1.0.19. Consecutive-hold regression and existing core tests pass. Live game scoring remains unverified.

# Version 1.0.19.0

Fix held notes being pressed again: queued detections no longer interrupt an
active hold. Duplicate near-target detections are filtered, while a separately
tracked next note waits for tail completion. Regression tests passed; live
scoring is not verified. Use Check for updates, then Update & restart.

# Version 1.0.18.0

- Fix automatic timing feedback stalling in fast passages.
- Add smaller timing refinement steps and shorter feedback trials.
- Fix long-note release speed being overwritten by upcoming notes.
- Improve dim-tail recognition and brief dropout handling.
- Allow late hold recognition while a key is still down.

Core regression tests and recorded-frame checks passed. Live scoring accuracy
remains unverified. Open the app and choose Check for updates, then Update & restart.
