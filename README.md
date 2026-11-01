# HashDash 3D

A first-person voxel puzzle game that teaches **CBSE Class XI Computer Science (083) Python dictionaries**.
Every block in the world is an entry in a Python dictionary, `world_data["x,y,z"] = "BlockType"`. Scan the magenta nodes, solve each diagnostic, and reshape the dictionary to escape.

## Chambers
1. **The Key Validation Wall**: keys must be immutable (`{[1, 2]: ...}` raises `TypeError`)
2. **The Missing Registry Alert**: a missing key raises `KeyError`
3. **The Traversal Network**: `len()` counts distinct key-value pairs
4. **The System Flush Portal**: `.clear()` empties the dictionary and leaves `{}`

## Controls
| Action | Keys |
| --- | --- |
| Move | W A S D / arrow keys (Shift to sprint) |
| Look | Mouse (click to lock the pointer) or drag |
| Scan | Click / E / SCAN button |
| Answer | 1 to 4, Enter to resume |
| Pause | Esc / P |

Progress saves automatically and a top-10 leaderboard is kept in the browser's `localStorage`.

## Run / deploy
It's a single static file (`index.html`) with no build step. Three.js r128 is loaded from cdnjs.
- **Locally:** open `index.html`, or run `python3 -m http.server` and visit http://localhost:8000
- **Vercel:** import this repo (framework preset: *Other*) or drag the folder onto vercel.com/new
