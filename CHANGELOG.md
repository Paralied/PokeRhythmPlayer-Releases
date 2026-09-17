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
