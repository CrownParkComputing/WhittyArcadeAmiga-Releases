# Chase H.Q. (Taito Z System) for Amiga

Taito's 1988 arcade chase-and-crash classic running natively on your Amiga:
the original dual-68000 game code executed on your machine, the TC0100SCN/
TC0150ROD video model rendered MAME-exact at the full 320x240 arcade
picture, and the arcade soundtrack — music, SFX, radio speech and the
pitch-tracking engine note — through Paula. Nab the criminal's car: ram it
until its damage bar fills before the timer runs out. Nitro (3 per stage)
is your friend on the straights.

## What's in the bundle

| File | What it is |
|---|---|
| `ChaseHQ` | The game — RTG/Picasso96 executable |
| `BuildPack` | One-time tool that renders the soundtrack from your ROMs |
| `ChaseHQ.info` | Workbench icon |
| `docs/ROM_FILES.txt` | Exact ROM filenames with SHA-256 checksums |
| `roms/chasehq/` | Empty — you fill this with your own ROM files |
| `README.md` | The bundle's own readme |

**No ROMs and no ROM-derived data are included.** You must own the game's
arcade ROMs.

## Requirements

- Amiga with a **68040-level CPU**, **64 MB fast RAM** and an **RTG
  (Picasso96/CyberGraphX) display** — Pimiga, Amiberry and PiStorm RTG
  setups qualify; a stock AGA A1200 does not.
- Kickstart 3.0+.
- The Chase H.Q. arcade ROMs (merged MAME `chasehq.zip` set) — **not
  included**.

## Install

1. **Extract the bundle** into a drawer on any Amiga drive (or mount the
   folder as a directory in your emulator).
2. **Supply your ROMs.** From your legally obtained merged MAME
   `chasehq.zip`, copy these 22 files into `roms/chasehq/` next to the
   executables. Flattened, by filename, regardless of the zip's internal
   subfolders (some may live under clone-set member paths); the full list
   with checksums is in `docs/ROM_FILES.txt`:

   ```
   b52-130.36  b52-136.29  b52-131.37  b52-129.30   (68000 A program)
   b52-132.39  b52-133.55                           (68000 B program)
   b52-137.51                                       (Z80 sound program)
   b52-29.27                                        (tiles)
   b52-28.4                                         (road)
   b52-38.34                                        (sprite map)
   b52-34.5    b52-35.7    b52-36.9    b52-37.11    (sprites A)
   b52-30.4    b52-31.6    b52-32.8    b52-33.10    (sprites B)
   b52-115.71  b52-114.72  b52-113.73               (ADPCM-A)
   b52-116.70                                       (ADPCM-B)
   ```

3. **Run `BuildPack` once** (Shell or Workbench). It renders the entire
   soundtrack from YOUR ROMs — the same Z80 + YM2610 sound board program
   the arcade ran — and writes `chasehq.pcm` next to the game.
   **This is slow**: it synthesizes more than an hour of audio through a
   software YM2610, so expect well over an hour on a 68040. A progress line
   per command counts up to 247. Start it and go have a coffee — it never
   needs to run again.
4. **Run `ChaseHQ`.** The game opens its own 864x486 8-bit RTG screen and
   holds the arcade's 60 Hz pacing, with frame-skip under load.

## Controls

**CD32 pad (port 2)**

- D-pad left/right = steer
- Red = gas (hold to drive)
- R shoulder = brake
- Yellow = gear toggle (LOW/HIGH)
- Green = nitro turbo (deliberately on the top-left button, away from the
  gas thumb)
- L shoulder = insert coin, Play = start

**Keyboard**

- Arrows = steer / gas / brake, `Space`/`LCtrl` = gas
- `X` = gear toggle, `LAlt` = nitro
- `5` = insert coin, `1`/`Return` = start
- `P` = pause, `F1` = cycle the frame-skip cap, `ESC` = quit

A small `GEAR HI/LO` readout is drawn at the screen's left border: the
arcade's LOW/HIGH shifter-box graphic is one HUD element the port does not
draw yet, so the text readout covers it.

## Troubleshooting

- **"CHASE H.Q. ROM FILES MISSING OR BAD" at startup** — the game and
  BuildPack verify every ROM's presence and size at startup and list any
  missing or bad file on screen. Extract from the merged `chasehq.zip` so
  that `roms/chasehq/` contains exactly the 22 files listed in
  `docs/ROM_FILES.txt`.
- **Game is silent** — the sound pack hasn't been built. Run `BuildPack`
  once (it writes `chasehq.pcm` next to the game — slow, one-time, see
  Install step 3), then restart. If sound ever misbehaves, delete
  `chasehq.pcm` and re-run `BuildPack` to regenerate it.
- **No screen appears** — this port needs an RTG (Picasso96/CyberGraphX)
  environment; it does not open a native AGA screen. Use a Pimiga-class
  setup, or an Amiberry config with Picasso96 enabled.
- **Feels slow under load** — frame-skip holds the 60 Hz pacing; press
  `F1` to cycle the frame-skip cap. The port needs a 68040-class CPU and
  64 MB fast RAM — a stock A1200 is not enough.
