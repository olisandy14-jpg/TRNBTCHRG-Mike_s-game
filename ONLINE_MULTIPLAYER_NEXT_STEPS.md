BTC GAME — ONLINE MULTIPLAYER MIGRATION NOTES (NOT YET IMPLEMENTED)

The v0.6 offline HTML contains all game state, random dice, deck ownership, betting and race adjudication locally in JavaScript. Local multiplayer is working, but it is not an online-authoritative architecture.

Suggested next phase:
1. Create a NEW GitHub repository and a NEW Vercel project, separate from existing BTC games.
2. Create a NEW Supabase project with isolated keys and database.
3. Build room creation, room codes, player seats, ready states and reconnect handling.
4. Move all random draws, card assignment, betting validation, dice and settlement to a server-authoritative game engine.
5. Use row-level security to protect private hands and bets; publish public board events separately.
6. Use real-time subscriptions for public moves, turn handovers, card decisions, results and reconnection.
7. Keep the current solo mode functioning locally without online dependencies.

Important: no online rooms, account management, networking or hosted services have been created in this beta.
