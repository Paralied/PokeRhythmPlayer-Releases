# Version 1.0.18.0

- Fix automatic timing feedback stalling in fast passages.
- Add smaller timing refinement steps and shorter feedback trials.
- Fix long-note release speed being overwritten by upcoming notes.
- Improve dim-tail recognition and brief dropout handling.
- Allow late hold recognition while a key is still down.

Core regression tests and recorded-frame checks passed. Live scoring accuracy
remains unverified. Open the app and choose Check for updates, then Update & restart.
