# DSA Sheet C++

A free, self-contained 12-week DSA (Data Structures & Algorithms) mastery tracker for LeetCode prep, built around C++ and real, verified learning resources instead of generic links.

**[Live demo screenshot / open `index.html` in any browser — no build step, no install.]**

## What's inside

- **12-week roadmap, 291 tracked problems** — split into 4 phases (Arrays/Hashing/Binary Search → Recursion/Linked Lists/Stacks → Trees/Graphs → Dynamic Programming), each week with a goal, a "Watch" list (specific YouTube playlists and video ranges — Striver, Aditya Verma, William Fiset, etc.) and a "Read" list (CP-Algorithms, USACO Guide, GeeksforGeeks, not raw cppreference).
- **6-week Codeforces track, 209 problems** — a separate section, topic by topic (implementation/math/constructive → greedy, sorting, two pointers → binary search, number theory, bitmasks → STL data structures & DFS/BFS → trees, shortest paths, DSU → DP). Problems are pulled from the Codeforces problemset by tag, climbing from 800 to 1900 rating, most-solved first in each rating band — classics plus volume. Each week has a goal, reading links (USACO Guide, CP-Algorithms), and its own progress bar.
- **12-week Codeforces track, 423 problems** — a separate section, topic by topic: implementation → math & constructive → sorting & greedy → two pointers, prefix sums & strings → binary search → number theory & combinatorics → bitmasks → STL data structures → DFS/BFS → trees → shortest paths, DSU & topo sort → DP. Problems come from the Codeforces problemset by tag, climbing from 800 to 2000 rating, most-solved first in each rating band — classics plus volume. Each week has a goal and reading links (USACO Guide, CP-Algorithms).
- **Separate Codeforces tracker** — its own progress bar, solved-by-rating breakdown, a 12-week tile grid that jumps to each week, and **Sync from Codeforces**: enter your handle and every sheet problem you've got Accepted on is ticked automatically via the public Codeforces API.
- **Per-problem notes** — click the note icon next to any problem to expand a small textarea; what you type is saved automatically as you type.
- **45-day learncpp.com calendar** — all 313 lessons across all 28 chapters of [learncpp.com](https://www.learncpp.com/), split day-by-day (chapter-boundary aware) starting from the day you open the sheet, as a check-the-box calendar.
- **freeCodeCamp video cross-reference** — days whose topic overlaps freeCodeCamp's ["C++ Programming Course – Beginner to Advanced"](https://www.youtube.com/watch?v=8jLOx1hD3_o) also show a "Watch" link that jumps straight to the matching chapter's real timestamp in the video.
- **Six rules of the practice protocol** — a short methodology section (20-minute wall before looking at hints, brute-force out loud, re-type from a blank file, a signal journal instead of a solution log, a re-solve queue at day+3/day+14, and a Sunday blind-set day) aimed at building independent problem-solving thinking rather than pattern memorization.
- **Light/dark theme**, mobile-friendly layout.

## How progress is saved

Everything (checked problems, Codeforces progress, notes, and the 45-day calendar) is saved to your browser's `localStorage`. There is no backend and no account — your progress lives only in the browser you used, on the device you used it on. Clearing site data / using a different browser or device starts you over. If you want cross-device sync, you're welcome to fork this and wire it up to a backend of your choice (Firebase, Supabase, a simple REST API, etc.) — the `save()` / `localSave()` / `localLoad()` functions in `index.html` are the only places that touch storage.

## Using it

1. Clone or download this repo.
2. Open `index.html` in any modern browser. That's it — no dependencies, no build step.
3. Optionally, enable GitHub Pages on this repo (Settings → Pages → deploy from `main` / root) to get a shareable URL, or host `index.html` anywhere that serves static files.

## Customizing it

The whole tracker is one file, `index.html`, with three parts:
- HTML/CSS for the layout and the design tokens (`:root` variables — swap colors here for your own theme).
- A `DATA` array (the 12 weeks — title, goal, resources, problem list per week).
- A `CFDATA` array (the 6 Codeforces weeks — sections of `[id, name, rating]`).
- A `CFDATA` array (the 12 Codeforces weeks — sections of `[id, name, rating]`).
- A `CPPDAYS` array (the 45-day learncpp.com + video calendar).

Edit either array directly to change the roadmap, add/remove problems, or adjust the calendar — everything else (rendering, checkboxes, notes, progress bars) reads from those arrays.

## Why this exists

Built out of a personal 3-month DSA prep plan, focused on avoiding the common failure mode of grinding a sheet (like Striver's A2Z) without developing real independent problem-solving ability. Sharing it in case it's useful to anyone else doing the same prep.

## License

MIT — see [LICENSE](LICENSE). Use it, fork it, change it, ship it as your own tracker.
