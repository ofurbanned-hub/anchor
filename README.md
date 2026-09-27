# Anchor RTP Bot — Minecraft 1.21.11

Client-side Fabric mod.

## Current behavior
- Toggle with `O`
- Sends `/rtp`
- Scans a 100-block spherical radius for Respawn Anchors
- Walks toward the nearest anchor and mines it
- Rescans and continues until no anchors are found
- Uses `/rtp` when the area is cleared
- Uses `/rtp` when another player is detected within 32 blocks
- Eats when hunger is 10 or lower if food is in hotbar
- Keeps the selected pickaxe equipped for Mending/XP repair

## Build

Use Java 21.

```powershell
./gradlew.bat build
```

The finished JAR will be in `build/libs/`.

## Important
This is an automation client and may be against the rules of servers that prohibit bots/macros. Test only where automation is allowed.

The movement/mining logic is intentionally simple in this starter build; it does not yet implement full collision-aware pathfinding or a dedicated XP-farm routine.
