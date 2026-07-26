# itch.io batch upload — one pass per game

Everything needed is in each game's `itch/` folder.  Per game (Shinobi,
AlienSyndrome):

1. itch.io -> Create new project.
2. Open `itch/PAGE.md` and copy each field into the matching form field
   (title, slug, tagline, classification, kind, pricing, description body,
   genre, tags, community).  Platforms: tick NONE.
3. Cover image: upload `itch/assets/cover-630x500.png`.
4. Screenshots: upload everything else in `itch/assets/` (screen*.png).
5. Uploads: add the game zip from this repo (`<Game>-Amiga.zip`), display
   name per PAGE.md, no platform ticks; optionally add `SHA256SUMS`.
6. Save & view; when live, paste the real itch URL over the TODO marker in
   `docs/index.html` (the "coming soon" buttons) and push.

Screenshot provenance: Alien Syndrome shots are the engine's own renderer at
2x (pixel-exact); Shinobi title shot is a Copperline cycle-accurate capture.
Add more gameplay shots any time with Amiberry's screenshot key if wanted.
