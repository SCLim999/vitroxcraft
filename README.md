# 🟩 VitroxCraft

**ViTrox Campus 2.0, rebuilt as a browser-based Minecraft-Education-style world.**

VitroxCraft is a standalone, single-file 3D voxel world — [play it live](https://sclim999.github.io/vitroxcraft/) —
that recreates [ViTrox Campus 2.0 by CYC Architect](https://www.cycarch.com/vitrox-campus-20)
(Batu Kawan, Penang): a central circular courtyard, radial layout, circular
landscape ramp, doorless entrance, green roof, and rectangular production/office
blocks punching through the circular form, plus the Campus 3.0 expansion and a
ViTrox Education building. It's built for teaching — architecture concepts,
company history, and now a full **C/C++ programming curriculum** — through
free exploration rather than a fixed lesson sequence.

No installation, no build step, no server: `index.html` is the entire project,
rendered with [Three.js](https://threejs.org) (loaded from a CDN) and generated
entirely from code — every block, texture, and character is procedural, with no
external art assets.

## Play

Open **[sclim999.github.io/vitroxcraft](https://sclim999.github.io/vitroxcraft/)**
in a desktop browser (needs internet once, to load Three.js; everything else works
offline after that). Walk with `WASD`, fly with `F`, break/place blocks with the
mouse, and press `E` near anything interactive.

## What's inside

- **9 golden info blocks** — walk up and press `E` to read short architecture
  lessons on the campus's design concepts (radial layout, solid vs. void, green
  roof, geometric juxtaposition, industry × campus culture, and more).
- **19 NPCs** — guards, receptionists, engineers, gardeners, chefs, students,
  the three real ViTrox co-founders, an architect, and lecturers — walk up and
  press `E` to talk. Dialogue is voiced with the browser's text-to-speech, using
  a voice that matches each character (male/female).
- **CodingMine — a 10-chapter C/C++ curriculum**: inside the VITROX-lettered
  building's 4th-floor computer rooms, 10 computers (green screens) are fixed
  Stations 1–10, each a direct doorway into one chapter — algorithms & syntax,
  3D coordinates, variables, arrays, `for` loops, `if/else`, `while` loops,
  functions, decomposition, and an open-ended capstone. 23 questions, 230
  points total; correct answers are scored live in the HUD and a dashboard
  (press `Q`), saved to `localStorage`. Four Computing School lecturers staff
  the rooms and teach Software Engineering, Data Science, Mobile App
  Development (Flutter), and Artificial Intelligence.
- **Trilingual**: the whole UI, every lesson, and all dialogue switch between
  中文 / English / Bahasa Melayu (top-right of the start menu; auto-detected on
  first load).
- **Multiplayer**: host a room from the start menu, share the 5-letter code,
  and classmates join over WebRTC ([PeerJS](https://peerjs.com)) — positions
  and block edits sync live, no server needed.
- **Free build mode**: 9 block types to build with; break a wall to see the
  floor/column structure underneath (the golden info blocks can't be broken).
  Edits are saved to `localStorage`, with a one-click world reset.
- **Touch controls**: fully playable on mobile/tablet with an on-screen joystick
  and action buttons.

## Full guide

[`MANUAL.md`](MANUAL.md) (Chinese) covers every system in detail — controls,
each info point's location, the full CodingMine chapter list, multiplayer setup,
and classroom suggestions for teachers.

## Hosting your own copy

It's a single static file — clone the repo and open `index.html` directly, or
host it anywhere static (GitHub Pages, Netlify, your own server). No backend,
API keys, or build tooling required.

## Credit

Architectural prototype: [ViTrox Campus 2.0 — CYC Architect](https://www.cycarch.com/vitrox-campus-20)
· Phase 1 ≈ 450,000 sq ft. This is an educational block-style interpretation
built for teaching purposes, not a to-scale model.
