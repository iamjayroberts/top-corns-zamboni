# 🌽 Top Corns Zamboni

Portrait-mode arcade mini-game. Coach Al noticed you haven't paid your league fees this month — so guess who's flooding the ice tonight?

Pick your player from the Top Corns roster, then tap as fast as you can to spiral the zamboni from the outer boards in to center ice. **Fastest resurface wins.**

## Project structure

```
.
├── index.html
└── assets/
    ├── coach.png
    ├── coach_face.png
    ├── jersey.png
    ├── rink.png
    └── zamboni.png
```

## Play

Open `index.html` through a local web server (assets need HTTP, not `file://`):

```bash
python3 -m http.server 8000
# → http://localhost:8000
```

For GitHub Pages, push the whole folder to a repo and enable Pages — it works directly.

## Flow

1. **Title screen** — Top Corns jersey, "tap to start"
2. **Coach Al** — tells you to flood the ice because you didn't pay your fees
3. **Select your player** — Johnston, Quirico, Spradling, King, or Soyk
4. **Countdown** — ready, set, go
5. **Game** — top-down rink, tap rapidly to drive the zamboni in a spiral from outer edge to center
6. **Results** — your time, best time, leaderboard

## Controls

| Action            | Keyboard          | Touch / Mouse        |
|-------------------|-------------------|----------------------|
| Start / advance   | `Enter` / `Space` | Tap                  |
| Choose player     | `↑` `↓` + `Enter` | Tap a row, tap it again to confirm |
| Drive the zamboni | `Space` / `Enter` / `↑` (each press = 1 tap) | Tap rapidly anywhere |

## Roster

| #  | Player    |
|----|-----------|
| 8  | Quirico   |
| 19 | Johnston  |
| 52 | Spradling |
| 98 | King      |
| 91 | Soyk      |

Best times are saved per player in browser localStorage. Top 5 show up on the leaderboard after every run.
