# 🟩 VitroxCraft

**ViTrox Campus 2.0, rebuilt as a browser-based Minecraft-Education-style world.**

VitroxCraft is a standalone, single-file 3D voxel world — [play it live](https://sclim999.github.io/vitroxcraft/) —
that recreates [ViTrox Campus 2.0 by CYC Architect](https://www.cycarch.com/vitrox-campus-20)
(Batu Kawan, Penang): a central circular courtyard, radial layout, circular
landscape ramp, a ring building whose internal corridor is a full block wider
on every floor than the original design and free of the radial support columns
that used to stand in the middle of the walkway, doorless entrances on all four
sides (E/S/W/N), a mostly-paved (no planters) roof terrace — cleared of paving across a wide
band from the stair tower around to the northeast, dropping one level down
to the slab below there (only the southeast stretch facing the courtyard
keeps its original paving) — and the ring's inner glass curtain wall restored
to its original, fully continuous design (the gardener NPC Kumar was moved
off the wall's boundary onto open terrace so he's no longer boxed in). The
stair tower's own roof-level doorways (north and south) used to be only
3 blocks wide, narrower than the skybridge itself, making the tower feel
like a wall blocking the terrace walkway — both were widened to match the
skybridge's 5-block width, and a second door was cut straight through the
skybridge's own side wall partway along, opening directly onto the ring's
terrace so players don't have to walk all the way to the tower. Restoring the inner/outer curtain walls to their full original design had
left their parapet caps sitting a block proud of the terrace wherever the
paving was dropped (reading like scattered raised grey boxes) — the
parapet is now dropped to match everywhere, so the terrace is one flat,
uniform level all the way around. The terrace's ring corridor was later
widened by another full block on both the inner and outer sides, with
the entrance's 2nd-floor skybridge moved out to match. A thin,
single-block steel safety fence now runs both the inner and outer edges
of the terrace, placed by stepping through angles and bridging the
diagonal corners so it forms one unbroken loop, with gaps only at the
stair tower, the skybridge's side door, the VITROX atrium connection,
and around Kumar — the stair tower and VITROX atrium gaps were
originally several blocks wider than the actual doorway, since
tightened to match the real door width exactly, and the fence's outer
ring was originally only excluded from the width of those two doors,
so the rest of it cut straight through the skybridge corridor and the
VITROX building's interior, leaving stray fence segments floating
inside both — now excluded from each building's full footprint
instead, so the fence no longer clips through walls. The stair
tower's own exclusion zone had a similar one-block margin beyond its
actual footprint, leaving a visible sliver gap between the fence and
the tower wall; tightened to match the tower's exact bounds so the
fence now runs flush against it on both sides. The four-storey skybridge used to open a door
into the tower on its top floor too, but the tower doesn't reach that
high — there was nothing on the other side — so that floor now dead-ends
at the skybridge's own solid glass wall instead, connecting to the lab
building only — (with a wide door
straight across to the VITROX-lettered building's 3rd floor, a widened 2nd-floor
entrance skybridge, and a wide four-storey glass skybridge from the stair
tower to the lab building), and rectangular production/office blocks punching
through the circular form, plus the Campus 3.0 expansion and a ViTrox
Education building. It's built for teaching — architecture concepts,
company history, and now a full **C/C++ programming curriculum** — through
free exploration rather than a fixed lesson sequence.

No installation, no build step, no server: `index.html` is the entire project,
rendered with [Three.js](https://threejs.org) (loaded from a CDN) and generated
entirely from code — every block, texture, and character is procedural, with no
external art assets.

## Play

Open **[sclim999.github.io/vitroxcraft](https://sclim999.github.io/vitroxcraft/)**
in a desktop browser (needs internet once, to load Three.js; everything else works
offline after that). The page opens on a lock screen and won't reveal the start
menu until the correct password is entered (ask the maintainer for it) —
re-checked on every page load; only a SHA-256 hash of the password ships in the
source. Walk with `WASD`, fly with `F`, break/place blocks with the mouse, and
press `E` near anything interactive.

## What's inside

- **10 golden info blocks** — walk up and press `E` to read short architecture
  lessons on the campus's design concepts (radial layout, solid vs. void, green
  roof, geometric juxtaposition, industry × campus culture, and the computer
  lab, and more).
- **21 NPCs** — a tutorial Game Master, guards, receptionists, engineers,
  gardeners, chefs, students, the three real ViTrox co-founders, an architect,
  lecturers, and a marketing officer — walk up and press `E` to talk. Dialogue
  is voiced with the browser's text-to-speech, using a voice that matches each
  character (male/female). The Game Master stands just outside the
  basketball court's south gate and explains the controls — WASD to move,
  mouse to look, Space to jump, `F` to fly, number keys/scroll wheel to pick
  a block, left-click to break, right-click to place, `E` to interact, `Q`
  for quests. **Talking to the Game Master isn't quite enough on its own** —
  every other NPC and golden info block stays locked (the on-screen prompt
  and the reminder toast both point you to the basketball court's south
  gate) until you also complete his hands-on practice: a yellow tile right
  next to him where you place a block, and a plank block you break.
  Do both and a "🎉 Practice complete" toast unlocks everything, so the
  exploration quest can't be finished before that either. Progress is saved
  to `localStorage`, so it only has to happen once.
- **DataMine IT quiz stations**: inside the VITROX-lettered building's
  4th-floor computer rooms, all 10 quiz computers are concentrated in the
  first room — the one Ts Dr Lim SC is stationed in — 5 per row, facing each
  other across the aisle he stands in. Each has a *different screen colour*
  and a *single* multiple-choice question on a different computing topic —
  Introduction to Computing, C++ Programming, Database, Information Technology,
  Data Science, Artificial Intelligence, Networking & Internet, Operating
  System, HTML, and Software Design. Questions are short and fun, aimed at
  primary/secondary-school level. Correct answers are scored live in the HUD
  (1 point per question, 10 points total), saved to `localStorage`. The second
  computer room is now just décor — two rows of plain computers, no quiz. A
  big blackboard mounted between the two rooms (visible from both sides) — the
  classroom dashboard — shows live progress per topic and total score, plus a
  live leaderboard of every connected player's score whenever a multiplayer
  room is active. Four Computing School lecturers staff the rooms and teach
  Software Engineering, Data Science, Mobile App Development (Flutter), and
  Artificial Intelligence. Ms Syira (Data Science) is a Malay Muslim woman,
  shown wearing a hijab and long dress. Two of them offer a "▶ Watch teaching
  animation" button in their dialogue: Ms Syira shows a data packet
  bouncing between a client and a server, labeled Request/Response, for the
  Networking & Internet topic; Mr Eng YK (AI) shows a CPU box cycling
  round-robin through four processes (P1–P4), for the Operating System
  topic. Scattered through the ground-floor pilotis of the
  ViTrox Education college building — well apart from each other and from Dr
  Janaka Low (its Principal) — are 7 wooden mailbox-style kiosks — a post, a
  crate and a coloured icon plaque, Minecraft-signpost style — grouped by
  qualification type along the walkway: 4 diplomas first (💻 Computer Science,
  📈 Business Studies, ⚙️ Mechatronics Engineering, ⚡ Electrical and Electronic
  Engineering), then 3 bachelor's degrees (🎓 Mechatronics Engineering Hons
  with UCSI University, 🔌 Electronic Engineering Hons and 🤖 Computer Science
  (Intelligent Computing) Hons — both marked *Coming Soon* — with Universiti
  Sains Malaysia). Marketing officer Cindy wanders that floor to point
  visitors to them. Just south of the building, across a stretch of lawn, is
  a small **sakura garden**: a cross-shaped stone path around a central
  lantern, four benches, and a ring of 8 pink cherry-blossom trees with
  fallen-petal tiles scattered underneath — pure scenery, free to wander
  through. On the left side of the main entrance roundabout stand 5 stone
  pillars capped in ViTrox blue, each labelled with one of the company's
  I.A.C.T.G. core values — Integrity, Accountability, Courage, Trust &
  Respect, and Gratitude & Care — per the official core-values page. Walk
  up to one and press `E` to read (and hear, via text-to-speech) the
  official story behind that value, in the selected language.
- **HUD minimap, compass and play timer**: a small top-down minimap (top-left)
  shows the central courtyard as a reference circle, gold/green dots for
  unvisited/visited info points, blue dots for NPCs, and a white arrow for
  the player's position and facing. A scrolling compass tape (top-center)
  shows N/E/S/W sliding past a fixed center pointer as you turn, so it's
  always obvious which way you're facing and where to walk next. A play
  timer next to the explore/DataMine chips counts actual play time (paused
  while a menu or dialogue is open).
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
each info point's location, the full DataMine question list, multiplayer setup,
and classroom suggestions for teachers.

## Hosting your own copy

It's a single static file — clone the repo and open `index.html` directly, or
host it anywhere static (GitHub Pages, Netlify, your own server). No backend,
API keys, or build tooling required.

## Credit

Architectural prototype: [ViTrox Campus 2.0 — CYC Architect](https://www.cycarch.com/vitrox-campus-20)
· Phase 1 ≈ 450,000 sq ft. This is an educational block-style interpretation
built for teaching purposes, not a to-scale model.
