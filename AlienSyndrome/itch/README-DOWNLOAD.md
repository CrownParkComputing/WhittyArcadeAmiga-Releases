# Alien Syndrome (Sega System 16B) for Amiga

Sega's 1987 arcade run-and-rescue classic running natively on your Amiga: the
original 68000 game code executed on your machine, the original System 16B
video model, and the arcade soundtrack — music, SFX and speech — through
Paula. Two players alternate; rescue 10 comrades per stage, then find the
exit before the time bomb detonates.

## What's in the bundle

| File | What it is |
|---|---|
| `AlienSyndrome` | AGA executable — real A1200/A4000, Amiberry AGA configs |
| `AlienSyndromeRTG` | RTG/Picasso96 executable — Pimiga and other RTG-first setups |
| `BuildPack` | One-time tool that renders the soundtrack from your ROMs |
| `AlienSyndrome.info` | Workbench icon |
| `docs/ROM_FILES.txt` | Exact ROM filenames with SHA-256 checksums |
| `roms/aliensyn/` | Empty — you fill this with your own ROM files |
| `README.md` | The bundle's own readme |

**No ROMs and no ROM-derived data are included.** You must own the game's
arcade ROMs.

## Requirements

- AGA Amiga (A1200/A4000 class) with a **68040-level CPU** and **64 MB fast
  RAM** — Amiberry, PiStorm and emulator setups qualify; a stock A1200 does
  not.
- Kickstart 3.0+.
- The Alien Syndrome arcade ROMs (merged MAME `aliensyn.zip` set) — **not
  included**.
- Best experienced at 60 Hz (NTSC-capable display or emulator).

## Install

1. **Extract the bundle** into a drawer on any Amiga drive (or mount the
   folder as a directory in your emulator).
2. **Supply your ROMs.** From your legally obtained merged MAME
   `aliensyn.zip`, copy these 21 files — the unprotected set 4 members —
   into `roms/aliensyn/` next to the executables. Flattened, by filename,
   regardless of the zip's internal subfolders (some live under clone-set
   member paths); the full list with checksums is in `docs/ROM_FILES.txt`:

   ```
   epr-11080.a1  epr-11081.a2  epr-11082.a3  epr-11083.a4  epr-11084.a5
   epr-11085.a6                                            (68000 program)
   epr-10702.b9  epr-10703.b10 epr-10704.b11               (tiles)
   epr-10709.b1  epr-10710.b2  epr-10711.b3  epr-10712.b4
   epr-10713.b5  epr-10714.b6  epr-10715.b7  epr-10716.b8  (sprites)
   epr-10723.a7                                            (Z80 sound program)
   epr-10724.a8  epr-10725.a9  epr-10726.a10               (uPD7759 speech)
   ```

3. **Run `BuildPack` once** (Shell or Workbench). It renders the entire
   soundtrack from YOUR ROMs — the same Z80 + YM2151 + uPD7759 sound board
   program the arcade ran — and writes `aliensyn.pcm` next to the game.
   Takes several minutes; it never needs to run again.
4. **Run the right executable** for your system:
   - `AlienSyndrome` — AGA machines and emulators showing native screens.
   - `AlienSyndromeRTG` — RTG/Picasso96 environments where native screens
     are not shown (Pimiga and similar).

## Controls

**Joystick / CD32 pad (port 2)**

- Move: stick / d-pad
- Red = shot
- L or R shoulder = insert coin, Play = start
- L + R + Play = DIP switch menu; hold the combo to quit

**Keyboard**

- Arrows = move, `Space`/`Ctrl` = shot
- `5` = insert coin, `1` = start (standard MAME-style keys)
- `F10` = DIP switch editor (lives, difficulty, timer)
- `F5` = save state, `F6` = load/resume state
- `ESC` = quit

## Troubleshooting

- **Missing-ROM message at startup** — the loader reports missing or
  mismatched ROM assets on screen. Extract from the merged `aliensyn.zip`
  so that `roms/aliensyn/` contains exactly the 21 files listed in
  `docs/ROM_FILES.txt`; each file's checksum is verified at startup.
- **Game is silent** — the game reports that no sound pack was found and
  continues without sound. Run `BuildPack` once to render the soundtrack
  from your ROMs (it writes `aliensyn.pcm`), then restart. If sound ever
  misbehaves, delete `aliensyn.pcm` and re-run `BuildPack` to regenerate
  it.
- **Very slow or won't run** — this port needs a 68040-class CPU and 64 MB
  fast RAM. A stock A1200 (68020, no fast RAM) is not enough; PiStorm,
  accelerated machines and emulators are.
- **Black/no screen on Pimiga or other RTG systems** — you ran the AGA
  build. Use `AlienSyndromeRTG` on RTG/Picasso96 environments.
