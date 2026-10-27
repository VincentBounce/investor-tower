# Investor Tower

A 2D pixel-art platformer in one HTML file. You play an investor; the tower, seen in cross-section, is the metaphor: **height is wealth**, from **$0 in the basement to $1M on the top floor**, on a logarithmic scale ($100 at the ground floor, ×10 every 7.5 floors). You start at age 20; the game ends when you reach $1M or retire at 65 (10 minutes).

Play: open `index.html` in a browser.

## Controls

| Key | Action |
|---|---|
| ← → (or A/Q, D) | walk |
| ↑ or W (Z on AZERTY) | jump |
| Space | open an elevator door (knock 5 times on real estate) |
| P / Esc | pause |

## The tower

Five vertical columns, left to right, with a hallway between neighbours on every floor:

| Column | Behaviour |
|---|---|
| **Bitcoin** | like the S&P 500 with 3× the amplitude, plus rare crashes |
| **S&P 500** | fast; goes up more often and for longer than it goes down |
| **Work** (centre) | no elevator: jump from platform to platform, all the way to the top. Miss and you fall further down, stunned (injuries at work, bad management). Platforms get narrower and crumble more often higher up. |
| **Fiat** | sinks slowly and constantly, down into the basement; its doors open at once |
| **Real estate** | rises slowly and steadily, but you must knock 5 times to get in and 5 times to get out |

Each elevator column is a paternoster: a stack of cabins, one per floor, all moving together; only the rising (or sinking) side is visible. A cabin has a door on each side, which opens only when it is roughly level with a hallway floor. Being carried below the bottom of a column throws you out at its lowest floor; being carried to the top floor makes you a millionaire.

Average yearly change (one floor = ×1.36, one year = 13.3 s):

| Column | Per year |
|---|---|
| Bitcoin | +41% on average, with phases 3× wider than the S&P 500 and rare crashes |
| S&P 500 | +27% on average |
| Fiat | −18.5% |
| Real estate | +17.8% |

The top bar shows wealth, age and an age gauge from 20 to 65 with the current year highlighted; the bottom bar shows each column's trend and its change since the start of the current year.

The starting basement is reached only by the Work platforms and the Fiat elevator.

## Versions

| Version | Changes |
|---|---|
| 0.1.0 | First playable version |
| 0.2.0 | Work platforms go up to the top floor; screen twice as tall (320×360); age gauge and each column's change this year |
