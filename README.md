# Seed Silo

A curated collection of **Minecraft (1.21.3)** seed banks, [Cubiomes Viewer](https://github.com/Cubitect/cubiomes-viewer) session files, and hand-picked seed lists created by **Sphagne** for finding interesting seeds for the Minecraft community.

> **At a glance:** 39 foundational seed banks · 212 specialized Cubiomes sessions · 25 curated plain-text seed selections

---

## How It Works

Finding seeds with very specific combinations of biomes, terrain, and structures from scratch can take a long time. **Seed Silo** solves this with a two-stage filtering workflow:

1. **Seed Banks (`+++`)** — Cubiomes sessions containing thousands of raw seeds that share a broad, useful set of baseline conditions (e.g., all major structures within a 2,000-block radius).
2. **Specialized Sessions (`-`)** — Follow-up Cubiomes sessions that use a seed bank as their *input source* instead of searching all 64-bit seeds. Because they only iterate over pre-filtered seeds, specialized searches run orders of magnitude faster.
3. **Seed Selections (`~`)** — Plain-text files containing curated seeds extracted from those sessions, ready to copy and paste directly into Minecraft.

---

## File Naming Convention

Every file in this repository follows a structured naming pattern:

```text
<Bank ID> <Type> [+++] <Description>.txt
```

| Token | Meaning |
| :--- | :--- |
| `<Bank ID>` | Numeric (or grouped, e.g., `100`, `212`, `401`) identifier linking specialized searches to their parent seed bank. Files sharing the same ID belong to the same family. |
| `-` | **Cubiomes Viewer session file** — contains search parameters/conditions and discovered seeds. |
| `~` | **Plain-text seed list** — contains selected seeds extracted from session files. |
| `+++` | **Seed bank** — a foundational Cubiomes session meant to be used as a source for narrower searches. |
| `0 ! about these files.txt` | Original plain-text overview note included in the repository. |

---

## Example Workflow: The `401` Series

1. **The Seed Bank:** [`401 - +++ all structures in 2k.txt`](401%20-%20%2B%2B%2B%20all%20structures%20in%202k.txt)
   - Holds **55,000+ seeds** where the player spawns inside a **Plains Village** and all of the following structures exist within a **2,000-block radius**:
     - Woodland Mansion
     - Desert Pyramid
     - Jungle Temple
     - Swamp Hut
     - Ocean Monument
     - Igloo
     - Pillager Outpost
     - Ancient City
   - *Why Plains Village?* Starting in a village narrows the search quickly, and Plains is a medium-temperature biome, increasing the odds of having both hot and cold biomes nearby.

2. **The Specialized Search:** [`401 - flat plains village peak mansion.txt`](401%20-%20flat%20plains%20village%20peak%20mansion.txt)
   - Uses `401 - +++ all structures in 2k.txt` as its seed source.
   - Searches those pre-filtered seeds for a village within 192 blocks surrounded mostly by plains, with nearby mountain peaks and a Woodland Mansion close by.
   - Every result is guaranteed to satisfy both the specialized terrain conditions **and** the parent bank's "all structures within 2k" condition.

---

## Seed Bank Categories

| Series | Theme | Included Seed Banks (`+++`) |
| :--- | :--- | :--- |
| **10 – 11** | Windswept & Desert Lake | `10 - +++ windswept plains villages+`, `11 - +++ desert village lake plus` |
| **100 – 120** | Oceans, Islands & Continents | `100 - +++ big oceans 1 & 2`, `110 - +++ central big oceans 1 & 2`, `112 - +++ central continents`, `119 - +++ central village island 128`, `120 - +++ shipwreck spawn` |
| **200 – 203** | Crater Villages | `200 - +++ crater villages`, `201 - +++ wide crater villages`, `202 - +++ wide crater villages v2.0`, `203 - +++ shore wide crater villages` |
| **210 – 212** | Wood & Multi-Villages | `210 - +++ wood villages`, `211 - +++ wood multi-villages`, `212 - +++ wood villages v2.0 & v2.1` |
| **220 – 270** | Terrain, Flat & Ice Villages | `220 - +++ hill rings`, `221 - +++ shattered villages`, `223 - +++ shattered villages v2.0`, `230 - +++ wood shipwrecks`, `240 - +++ flat villages in teresting`, `241 - +++ super flat villages`, `242 - +++ very flat villages`, `250 - +++ meadow village in river-crater`, `260 - +++ village in ice spikes`, `270 - +++ wide crater temple portal` |
| **300 – 320** | Ice Age, Deserts & Shipwrecks | `300 - +++ ice age`, `310 - +++ desert plains villages`, `320 - +++ land shipwrecks`, `320 - +++ windswept lush village` |
| **400 – 422** | All Structures, Villages & Wrecks | `400 - +++ all structures in 2048x2048`, `401 - +++ all structures in 2k`, `410 - +++ lots of villages`, `420 - +++ village in wrecks`, `421 - +++ mining villages`, `422 - +++ village with exposed shipwrecks` |
| **500 – 501** | Strongholds | `500 - +++ close strongholds`, `501 - +++ populated strongholds` |

---

## How to Use

### For Players (Just Looking for Seeds)
- Open any `~` file (e.g., [`401 ~ all structure selection.txt`](401%20~%20all%20structure%20selection.txt)) to grab curated seeds directly.
- You can also open any `-` session file in a text editor—the numeric seed IDs are listed line by line below the `#` metadata headers.

### For Seed Hunters (Using Cubiomes Viewer)
1. Download and open **Cubiomes Viewer**.
2. Load any `-` session file (or a `+++` seed bank) into Cubiomes Viewer.
3. **Important — Relink the Source File:** Local source-file directory paths were removed from the session files for portability across machines. If you want to continue or re-run a specialized search (`-`), manually point its seed source in Cubiomes Viewer to the matching `+++` seed bank file on your computer (matched by the leading ID number).

---

Hope you enjoy exploring and building on these seeds!

— **Sphagne**
