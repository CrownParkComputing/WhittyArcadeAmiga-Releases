# WhittyArcadeAmiga Releases

Amiga ports of Sega System 16B arcade games: the original 68000 game code
running on your Amiga, the original board's video model, and the arcade
soundtrack rendered from your own ROMs.

## Downloads

Downloads are distributed through
[CrownParkComputing on itch.io](https://crownparkcomputing.itch.io/).
The bundles are not served from this GitHub page.

| Game | Download | Requirements |
|---|---|---|
| Shinobi (Sega, 1987) | [Get it on itch.io](https://crownparkcomputing.itch.io/shinobi-amiga) | 68040-class CPU, 64MB fast RAM, Kickstart 3.0+ |
| Alien Syndrome (Sega, 1987) | [CrownParkComputing on itch.io](https://crownparkcomputing.itch.io/) | 68040-class CPU, 64MB fast RAM, Kickstart 3.0+ |

## What's in a bundle -- and what is not

Each bundle contains the game executables (`<Game>` for AGA machines,
`<Game>RTG` for RTG/Picasso96 systems such as Pimiga), the one-time
**BuildPack** tool, documentation, and an EMPTY `roms/` directory.

**No ROMs and no ROM-derived data are included.**  You must own the game's
arcade ROMs.  The bundle README lists the exact files (with checksums) to
copy from the merged MAME ROM set into `roms/<set>/`.

## First run

1. Unpack the bundle onto any Amiga drive (or mount the folder in your
   emulator).
2. Copy your ROM files into `roms/<set>/` per the bundle README.
3. Run **BuildPack** once.  It renders the entire soundtrack from your
   ROMs -- the same Z80 + FM + ADPCM sound board the arcade ran -- and
   writes the sound pack next to the game.  Takes a few minutes.
4. Run the game executable for your system type.  Full controls and notes
   are in each bundle's README.
