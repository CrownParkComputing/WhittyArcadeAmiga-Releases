# itch.io publishing kit — Shinobi (Sega System 16B) for Amiga

Copy-paste sheet for the itch.io **Create new project** form. Each heading below
is the exact itch field name; paste the block under it into that field.

---

## Title

```
Shinobi (Sega System 16B) for Amiga
```

## Project URL

Suggested slug (itch fills `crownparkcomputing.itch.io/` + slug):

```
shinobi-amiga
```

## Short description or tagline

(itch limit is ~120 characters — this is 118)

```
Sega's 1987 arcade classic running natively on your Amiga. Original 68000 code, AGA & RTG builds. You supply the ROMs.
```

## Classification

`Game`

## Kind of project

`Downloadable`

## Release status

`Released`

## Pricing

`No payments` (Free — do not enable payments/donations unless you want them)

## Description

Paste the block below into the rich-text editor. itch accepts pasted HTML;
if it strips anything, switch the editor to HTML/source mode first.

```html
<p><strong>Joe Musashi's one-man war on the Zeed syndicate — ported straight
from the arcade board to your Amiga.</strong></p>

<p>This is not a remake. The original Sega System 16B 68000 program runs
natively on your Amiga's CPU, with the board's tile, sprite and priority model
reproduced, and the full Z80 + YM2151 + uPD7759 arcade soundtrack synthesized
from your own ROMs and played through Paula.</p>

<h2>Features</h2>
<ul>
<li><strong>Two builds in one bundle</strong> — <em>Shinobi</em> for AGA
machines (real A1200/A4000, Amiberry AGA configs) and <em>ShinobiRTG</em> for
RTG/Picasso96 systems such as Pimiga.</li>
<li><strong>The real arcade soundtrack</strong> — run the included BuildPack
tool once and it renders the entire score from your ROMs, the same sound board
the arcade ran.</li>
<li><strong>Arcade DIP switches</strong> — press F10 (or L+R+Play on a CD32
pad) for the in-game DIP switch editor: lives, difficulty, demo sounds and
more.</li>
<li><strong>Save states</strong> — F5 saves, F6 loads/resumes.</li>
<li><strong>CD32 pad support</strong> — attack, jump and magic on the face
buttons, coin and start on the shoulder buttons.</li>
</ul>

<h2>System requirements</h2>
<ul>
<li>AGA Amiga (A1200/A4000 class) with a <strong>68040-level CPU</strong> and
64 MB fast RAM — Amiberry, PiStorm and emulator setups qualify; a stock A1200
does not.</li>
<li>Kickstart 3.0+.</li>
<li>Best experienced at 60 Hz (NTSC-capable display or emulator).</li>
</ul>

<h2>You supply the ROMs</h2>
<p><strong>This bundle contains no arcade ROMs and no ROM-derived data.</strong>
You must own Shinobi's arcade ROMs. Copy the required files from your legally
obtained merged MAME <em>shinobi.zip</em> set into the bundle's
<em>roms/shinobi6/</em> folder — the exact filenames and SHA-256 checksums are
listed in the bundle's <em>docs/ROM_FILES.txt</em>, and the loader verifies
them at startup.</p>

<h2>How to install</h2>
<ol>
<li>Extract the zip onto any Amiga drive (or mount the folder as a directory
in your emulator).</li>
<li>Copy the ROM files listed in <em>docs/ROM_FILES.txt</em> from the merged
MAME <em>shinobi.zip</em> into <em>roms/shinobi6/</em> — flattened, by
filename, regardless of the zip's internal subfolders.</li>
<li>Run <strong>BuildPack</strong> once (Shell or Workbench). It renders the
soundtrack from your ROMs and writes <em>shinobi.pcm</em> next to the game.
Takes several minutes; never needs to run again.</li>
<li>Run <strong>Shinobi</strong> on AGA machines, or <strong>ShinobiRTG</strong>
on RTG/Picasso96 systems such as Pimiga.</li>
</ol>

<p>Full controls and troubleshooting are in the bundle's README.
Releases and checksums also live on
<a href="https://github.com/CrownParkComputing/WhittyArcadeAmiga-Releases">GitHub</a>.</p>
```

## Genre

`Action`

## Tags

Suggest these 8 (itch allows up to 10):

```
amiga, arcade, retro, sega, port, aga, m68k, ninja
```

## Platforms (project-level checkboxes)

Tick **NONE** of Windows / macOS / Linux / Android / iOS — these are Amiga
executables, not host-OS binaries. The description already states it runs on
real Amigas and on Amiberry/Pimiga; ticking a desktop OS would make the itch
app try to install/launch it.

## Uploads

- Upload `Shinobi-Amiga.zip` (the file from this repo's `Shinobi/` folder,
  SHA-256 `ff0ab1466f8fbd890ab16796a25ee94ae0e082577ec41f2953b5cda85e646dbf`).
- Display name: `Shinobi-Amiga.zip — AGA + RTG builds (no ROMs included)`
- Under the upload's platform checkboxes: tick **nothing** (leave it as a
  plain downloadable file).
- Optionally also upload `SHA256SUMS` with display name
  `SHA256SUMS — bundle checksum`.

## Community

`Comments` (enabled)

## Screenshots & cover — what to grab

- Gameplay screenshots: capture at the native 320x224 and scale **2x
  nearest-neighbour to 640x448** (no smoothing). Good set: title screen,
  Mission 1 gameplay, a magic (ninjutsu) blast, a boss fight, the bonus
  stage.
- Cover image: **630x500**. Title-screen logo art on a dark background works;
  keep any text inside the middle so itch's thumbnail crop doesn't cut it.
- One shot of the F10 DIP switch editor makes a nice "features" screenshot.

<!-- TODO: after publishing, put the live itch.io URL here and update the
     "coming soon" buttons in docs/index.html -->
