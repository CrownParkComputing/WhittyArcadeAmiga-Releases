# itch.io publishing kit — Chase H.Q. (Taito Z System) for Amiga

Copy-paste sheet for the itch.io **Create new project** form. Each heading below
is the exact itch field name; paste the block under it into that field.

---

## Title

```
Chase H.Q. (Taito Z System) for Amiga
```

## Project URL

Suggested slug (itch fills `crownparkcomputing.itch.io/` + slug):

```
chase-hq-amiga
```

## Short description or tagline

(itch limit is ~120 characters — this is 119)

```
Taito's 1988 chase-and-crash classic runs natively on your Amiga. Original dual-68000 code, RTG build. You supply ROMs.
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
<p><strong>"Nancy from Chase H.Q." has a suspect for you. Run him down and
ram his car off the road before the timer expires — Taito's 1988
chase-and-crash arcade classic, ported straight from the board to your
Amiga.</strong></p>

<p>This is not a remake. The original dual-68000 Taito Z System program runs
natively on your Amiga's CPU, with the board's TC0100SCN tile and TC0150ROD
road hardware rendered MAME-pixel-verified at the full 320x240 arcade
picture — road, sprites and priorities exact. The full arcade audio — music,
SFX, the radio calls and speech — is rendered from your own ROMs, and the
engine note plays on genuine Paula hardware with its pitch tracking your
speed.</p>

<h2>Features</h2>
<ul>
<li><strong>The real arcade game</strong> — original 68000 game code, not a
reinterpretation; MAME-exact road, sprites and priorities at 60 Hz with
frame-skip under load.</li>
<li><strong>The real arcade audio</strong> — run the included BuildPack tool
once and it renders the entire soundtrack from your ROMs, the same Z80 +
YM2610 sound board program the arcade ran. It synthesizes over an hour of
audio through a software YM2610, so the one-time run takes well over an hour
on a 68040 — start it, go have a coffee (or lunch), and never run it
again.</li>
<li><strong>CD32 pad control</strong> — Red = gas, R shoulder = brake,
Yellow = gear toggle, Green = nitro (deliberately on the top-left button,
away from the gas thumb), L shoulder = coin, Play = start.</li>
<li><strong>Gear readout</strong> — a small GEAR HI/LO indicator at the
screen's left border stands in for the arcade's shifter-box graphic.</li>
<li><strong>RTG native</strong> — opens its own 864x486 Picasso96 screen;
built for Pimiga-class RTG environments.</li>
</ul>

<h2>System requirements</h2>
<ul>
<li>Amiga with a <strong>68040-level CPU</strong>, 64 MB fast RAM and an
<strong>RTG (Picasso96/CyberGraphX) display</strong> — Pimiga, Amiberry and
PiStorm RTG setups qualify; a stock AGA A1200 does not.</li>
<li>Kickstart 3.0+.</li>
</ul>

<h2>You supply the ROMs</h2>
<p><strong>This bundle contains no arcade ROMs and no ROM-derived data.</strong>
You must own Chase H.Q.'s arcade ROMs. Copy the 22 required files from your
legally obtained merged MAME <em>chasehq.zip</em> set into the bundle's
<em>roms/chasehq/</em> folder. The exact filenames and checksums are listed
in the bundle's <em>docs/ROM_FILES.txt</em>, and the game verifies them at
startup, reporting any missing or bad file on screen.</p>

<h2>How to install</h2>
<ol>
<li>Extract the zip onto any Amiga drive (or mount the folder as a directory
in your emulator).</li>
<li>Copy the 22 ROM files listed in <em>docs/ROM_FILES.txt</em> from the
merged MAME <em>chasehq.zip</em> into <em>roms/chasehq/</em> — flattened, by
filename, regardless of the zip's internal subfolders.</li>
<li>Run <strong>BuildPack</strong> once (Shell or Workbench). It renders the
soundtrack from your ROMs and writes <em>chasehq.pcm</em> next to the game.
This is the slow, one-time step — well over an hour on a 68040; a progress
line counts up to 247.</li>
<li>Run <strong>ChaseHQ</strong>.</li>
</ol>

<p>Full controls and troubleshooting are in the bundle's README.
Project information also lives on
<a href="https://github.com/CrownParkComputing/WhittyArcadeAmiga-Releases">GitHub</a>.</p>
```

## Genre

`Racing`

## Tags

Suggest these 8 (itch allows up to 10):

```
amiga, arcade, retro, taito, port, rtg, racing, driving
```

## Platforms (project-level checkboxes)

Tick **NONE** of Windows / macOS / Linux / Android / iOS — this is an Amiga
executable, not a host-OS binary. The description already states it runs on
real Amigas and on Amiberry/Pimiga RTG setups; ticking a desktop OS would
make the itch app try to install/launch it.

## Uploads

- Upload `ChaseHQ-Amiga.zip` (the file from this repo's `ChaseHQ/` folder,
  SHA-256
  `3397f538d5c9dcb76f409a0febf138a383863ac5b85460fbe48bb7cfc4c19218`).
- Display name: `ChaseHQ-Amiga.zip — RTG build (no ROMs included)`
- Under the upload's platform checkboxes: tick **nothing** (leave it as a
  plain downloadable file).
- Optionally also upload `SHA256SUMS` with display name
  `SHA256SUMS — bundle checksum`.

## Community

`Comments` (enabled)

## Screenshots & cover — what to grab

<!-- TODO: no assets exist yet for Chase H.Q. — assets/ is empty. Grab
     gameplay shots with Amiberry's screenshot key (the pattern the Alien
     Syndrome assets set), then drop them in assets/ using the same names:
     cover-630x500.png, screen1-title.png, screen2-... etc. -->

- **TODO — no cover or screenshots captured yet.** Capture with Amiberry's
  screenshot key and save into this folder's `assets/` directory.
- Gameplay screenshots: the game's picture is the full **320x240** arcade
  frame — scale **2x nearest-neighbour to 640x480** (no smoothing). Good
  set: title screen, the briefing ("Nancy from Chase H.Q."), full-speed
  highway with traffic, a nitro burst, ramming the suspect's car with the
  damage bar visible.
- Cover image: **630x500**. Title-screen logo art on a dark background
  works; keep any text inside the middle so itch's thumbnail crop doesn't
  cut it.

## Assets (in this folder)

- `assets/` — **empty for now**; see the TODO above. Once filled:
  `assets/cover-630x500.png` uploads as the project cover image and
  `assets/screen*.png` as the screenshots, in number order.

<!-- TODO: after publishing, put the live itch.io URL here and update the
     download button for Chase H.Q. in docs/index.html -->
