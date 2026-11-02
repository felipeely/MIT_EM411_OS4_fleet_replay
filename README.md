# Fleet Day Replay (MIT EM.411 OS4, Task 2)

A web page that replays one simulated weekday of the autonomous shuttle and e-bike fleet on the real streets of the MIT / Kendall service area, with a custom fleet builder and a "How it works" page.

- `index.html` the replay page
- `how.html` the formulas
- `map.json` streets, buildings, river (City of Cambridge GIS open data, built by `map_build.py`)
- `index.json`, `runs/*.json` recorded days of `sim_day.py` (built by `sim_replay.py`)

Run locally: `python3 -m http.server` in this folder, then open http://localhost:8000
Host: GitHub Pages (static files, no build step).
