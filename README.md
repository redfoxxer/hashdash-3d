# HashDash 3D

A first-person voxel puzzle game that teaches **CBSE Class XI Computer Science (083) Python dictionaries**.
Every block in the world is an entry in a Python dictionary, `world_data["x,y,z"] = "BlockType"`. Scan the magenta nodes, solve each diagnostic, and reshape the dictionary to escape.

## Chambers
Each chamber picks one of 3 CBSE-style questions at random.
1. **The Key Validation Wall**: immutable keys, `dict()` construction (a hurdle teaches the jump)
2. **The Missing Registry Alert**: `KeyError`, `get()` with a default, `in` checks keys only. Solving it builds a zig-zag jumping bridge.
3. **The Mutation Engine**: assigning to keys, `update()`, `setdefault()`
4. **The Traversal Network**: `len()`, looping over keys, `max()` / `sorted()` on dictionaries
5. **The System Flush Portal**: `clear()`, `pop()`, `copy()` vs a second name for the same object

**Firewall:** once a diagnostic opens, a firewall closes in from behind. If it reaches you, you get shoved into the void or crushed, with a +15 s penalty and a respawn at the checkpoint.

## Controls
| Action | Keys |
| --- | --- |
| Move | W A S D / arrow keys (Shift to sprint) |
| Jump | Space |
| Look | Mouse (click to lock the pointer) or drag |
| Scan | E / click / SCAN button |
| Answer | 1 to 4, Enter to resume |
| Pause | Esc / P |

Progress saves automatically and a top-10 leaderboard is kept in the browser's `localStorage`.

## Run / deploy
It's a single static file (`index.html`) with no build step. Three.js r128 is loaded from cdnjs.
- **Locally:** open `index.html`, or run `python3 -m http.server` and visit http://localhost:8000
- **Vercel:** import this repo (framework preset: *Other*) or drag the folder onto vercel.com/new
