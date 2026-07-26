# itch.io publishing kit — Alien Syndrome (Sega System 16B) for Amiga

Copy-paste sheet for the itch.io **Create new project** form. Each heading below
is the exact itch field name; paste the block under it into that field.

---

## Title

```
Alien Syndrome (Sega System 16B) for Amiga
```

## Project URL

Suggested slug (itch fills `crownparkcomputing.itch.io/` + slug):

```
alien-syndrome-amiga
```

## Short description or tagline

(itch limit is ~120 characters — this is 119)

```
Sega's 1987 run-and-rescue classic runs natively on your Amiga. Original 68000 code, AGA & RTG builds. You supply ROMs.
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
<p><strong>Fight through infested space stations, rescue your comrades and
get out before the time bomb detonates — Sega's 1987 run-and-rescue arcade
classic, ported straight from the board to your Amiga.</strong></p>

<p>This is not a remake. The original Sega System 16B 68000 program runs
natively on your Amiga's CPU, with the board's tile, sprite and priority model
reproduced, and the full arcade audio — music, SFX and the uPD7759 speech
samples — synthesized from your own ROMs and played through Paula. Two players
alternate; rescue 10 comrades per stage, then find the exit before the bomb
goes off.</p>

<h2>Features</h2>
<ul>
<li><strong>Two builds in one bundle</strong> — <em>AlienSyndrome</em> for AGA
machines (real A1200/A4000, Amiberry AGA configs) and <em>AlienSyndromeRTG</em>
for RTG/Picasso96 systems such as Pimiga.</li>
<li><strong>The real arcade audio, speech included</strong> — run the
included BuildPack tool once and it renders the entire soundtrack from your
ROMs, the same Z80 + YM2151 + uPD7759 sound board program the arcade ran.</li>
<li><strong>Arcade DIP switches</strong> — press F10 (or L+R+Play on a CD32
pad) for the in-game DIP switch editor: lives, difficulty, timer.</li>
<li><strong>Save states</strong> — F5 saves, F6 loads/resumes.</li>
<li><strong>CD32 pad support</strong> — shot on the red button, coin and
start on the shoulder buttons.</li>
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
You must own Alien Syndrome's arcade ROMs. Copy the 21 required files — the
unprotected set 4 members — from your legally obtained merged MAME
<em>aliensyn.zip</em> set into the bundle's <em>roms/aliensyn/</em> folder.
The exact filenames and SHA-256 checksums are listed in the bundle's
<em>docs/ROM_FILES.txt</em>, and the loader verifies them at startup.</p>

<h2>How to install</h2>
<ol>
<li>Extract the zip onto any Amiga drive (or mount the folder as a directory
in your emulator).</li>
<li>Copy the 21 ROM files listed in <em>docs/ROM_FILES.txt</em> from the
merged MAME <em>aliensyn.zip</em> into <em>roms/aliensyn/</em> — flattened,
by filename, regardless of the zip's internal subfolders.</li>
<li>Run <strong>BuildPack</strong> once (Shell or Workbench). It renders the
soundtrack from your ROMs and writes <em>aliensyn.pcm</em> next to the game.
Takes several minutes; never needs to run again.</li>
<li>Run <strong>AlienSyndrome</strong> on AGA machines, or
<strong>AlienSyndromeRTG</strong> on RTG/Picasso96 systems such as Pimiga.</li>
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
amiga, arcade, retro, sega, port, aga, rtg, shoot-em-up
```

## Platforms (project-level checkboxes)

Tick **NONE** of Windows / macOS / Linux / Android / iOS — these are Amiga
executables, not host-OS binaries. The description already states it runs on
real Amigas and on Amiberry/Pimiga; ticking a desktop OS would make the itch
app try to install/launch it.

## Uploads

- Upload `AlienSyndrome-Amiga.zip` (the file from this repo's
  `AlienSyndrome/` folder, SHA-256
  `9578f5f1c9286328c1242afc651a6794ed78d1c2a344c11fc8827f0bf4c13d56`).
- Display name: `AlienSyndrome-Amiga.zip — AGA + RTG builds (no ROMs included)`
- Under the upload's platform checkboxes: tick **nothing** (leave it as a
  plain downloadable file).
- Optionally also upload `SHA256SUMS` with display name
  `SHA256SUMS — bundle checksum`.

## Community

`Comments` (enabled)

## Screenshots & cover — what to grab

- Gameplay screenshots: capture at the native 320x224 and scale **2x
  nearest-neighbour to 640x448** (no smoothing). Good set: title screen, a
  stage-1 rescue with hostages on screen, the exit countdown, an end-of-stage
  boss, the two-player alternating score screen.
- Cover image: **630x500**. Title-screen logo art on a dark background works;
  keep any text inside the middle so itch's thumbnail crop doesn't cut it.
- One shot of the F10 DIP switch editor makes a nice "features" screenshot.

<!-- TODO: after publishing, put the live itch.io URL here and update the
     "coming soon" buttons in docs/index.html -->

## Assets (in this folder)

- `assets/cover-630x500.png` — upload as the project cover image.
- `assets/screen*.png` — upload as the screenshots, in number order.
