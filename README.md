# The Really Nasty BTC Game

A satirical, four-horse BTC racing game. This repository starts from the playable **v0.6 beta**.

## Play locally

Open `index.html` in a modern browser. No installation, npm packages, accounts or server are required.

## Available game modes

- **Solo:** one human versus three personality-driven bots, with Infantry (Easy), REME (Medium) and AI Ninja (Hard) difficulty settings.
- **Local multiplayer:** 2–4 human players sharing one device, with bots filling unused places. Private handovers allow individual bets and card choices.

The game includes four races, eight hedges per lane, character-on-horse artwork, betting and special cards. Each lane keeps its own pip spacing while the hedges and finish line visually align.

## Hosting

This beta is a **static site**: `index.html` includes the CSS, JavaScript and game artwork. It can be deployed to Vercel as a static project, without a build step.

1. Import this repository into a new Vercel project.
2. Choose **Other** (or **No Framework**) as the framework preset.
3. Leave the build command empty. Use the repository root (`.`) as the output directory if asked.
4. Deploy. The site's root path will serve `index.html`.

Important: hosting this static build does **not** make multiplayer remote/networked. Multiplayer in v0.6 is local pass-and-play only.

## Next stage: online multiplayer

See [`ONLINE_MULTIPLAYER_NEXT_STEPS.md`](ONLINE_MULTIPLAYER_NEXT_STEPS.md) for the proposed room-code, server-authoritative game engine and private-bet architecture.

## Project isolation

Keep this game in its own repository and, when online play is implemented, its own hosting project and backend. Do not share database keys or live game state with other BTC projects.

## Status

Beta software. Use for testing and iterate on rules, AI behaviour, visual layout and multiplayer UX before launching an online service.
