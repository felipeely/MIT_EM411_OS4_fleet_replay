# Fleet Day Replay (MIT EM.411 OS4, Task 2)

A web page that replays one simulated weekday of the autonomous shuttle and e-bike fleet on the real streets of the MIT / Kendall service area, with a custom fleet builder and a "How it works" page.

- `index.html` the replay page
- `how.html` the formulas
- `map.json` streets, buildings, river (City of Cambridge GIS open data, built by `map_build.py`)
- `map.js`, `index.js`, `runs/*.js` the same data as JavaScript so the page also opens straight from a folder
- `index.json`, `runs/*.json` recorded days of `sim_day.py` (built by `sim_replay.py`); `runs/smart_*` are the same days with smart dispatch, `runs/*paths_*` with bikes on campus footpaths (`map.json` also holds the footpath network, built by `build_paths.py`)

- Charging switch (Where it stands / At the base) and the Go charge below slider: with the base on, or the level not 20%, the page simulates the 200 days live in the browser (`index.html` holds the same simulation as `sim_day.py`). `map.json` also holds the base (Volpe site, Third St) and the distance of every node to it (built by `add_base.py`).

Run locally: just double-click `index.html` (the `.js` copies of the data files let it work without a server), or run `python3 -m http.server` and open http://localhost:8000
Host: GitHub Pages (static files, no build step).
