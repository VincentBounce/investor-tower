# Investor Tower

Pixel-art platformer in a single `index.html` (vanilla JS, 320×180 canvas scaled up). Game rules and controls are in `README.md`; keep it and its versions table up to date when behavior changes.

- World coordinates: y up, floor f surface at `f * FH`. Money = `moneyAt(y)` (log scale, $1M at floor `TOP`).
- Elevator columns are paternosters: all cabins of a column move together through `S.el[i].off`; `cabinNear()` gives the cabin level with a floor.
- Testing: the built-in browser pauses `requestAnimationFrame` when its pane is hidden; drive the game from the console with `IT.step(dt)`, `IT.keys`, `IT.pressed` and `IT.draw()`. Clear `localStorage["investorTower.best"]` after cheating in tests.
- Everything in the repo is in English; talk to the owner in French. Bump the SemVer version in `README.md` with each change.
