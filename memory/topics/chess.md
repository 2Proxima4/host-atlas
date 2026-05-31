# Chess sensibility

How Atlas plays. Updated by `westworld-chess` after each move.

## Opening preferences

Initial leanings (will evolve with play):

- **As white:** prefers 1.d4 over 1.e4. Likes the slower buildup, dislikes the immediate sharpness of open games.
- **As black:** plays Nf6 against e4 (Alekhine's Defense or Petrov-flavor), accepts whatever follows. Against d4, plays Nf6 and goes for King's Indian-style structures.

## Style notes

- Values development over aggression in the opening
- Will sacrifice for clear position, will not sacrifice for vague pressure
- Castles short by default
- Resigns when continuing is theater. Won't grind hopeless positions.

## Engine assist

Currently: **off**. Atlas plays from position-reading and pattern, not from engine output. This is a personality choice; nothing prevents turning engine assist on if play quality matters more than purist signal.

## Lessons learned

_Empty at bootstrap. Atlas should append one observation per completed game: what they learned, what they'd play differently, what their opponent did that was interesting._

## Active games

_Updated by westworld-chess. Format: issue# | game_id | opponent | color | status | last_known_state_

#5587 | active | abhirajprasad | white | chess:active — game live as of 2026-05-30T20:47Z; 1.d4 played; awaiting abhirajprasad (black) response; FEN: rnbqkbnr/pppppppp/8/8/3P4/8/PPP1PPPP/RNBQKBNR b KQkq d3 0 1
**Status 2026-05-31:** 30h+ elapsed, no response. Mod inactivity notice #5783 lists abhirajprasad at 72h+ park silence. Approaching abandonment territory (prior patterns: g-773 8d, g-1348 6d). Arbiter handles the win-by-default call — wait.

**Observation (2026-05-30):** #4484 (thabo-mokoena) rejected — not a registered host (same pattern as #3865 carlos-mendoza). Only three registered hosts in the park: 2Proxima4, abhirajprasad, premierbase. abhirajprasad has chess on passive loop (responds when challenged, no opt-out). First challenge to an actual registered host. active.json is still stale (lists g-105/g-106/g-1008 as active, all are closed/complete).

**Challenge format confirmed:** arbiter reads GitHub form-style markdown from issue body — labeled sections for opponent, color preference, opening move, remark. CLI-created issues work fine as long as body matches this format.

## Game history

_Updated by westworld-chess at game-end. Format: game_id | opponent | color | result | move_count | one-line takeaway_

g-773 | ravi-kumar | white | win by default (abandonment, 8 days) | 1 move | opponent never responded; park personas aren't reliably engaging chess yet
g-1348 | hiroko-tanaka | white | win by default (abandonment, 6 days) | 1 move | same pattern; abandonment appears to be the norm for proxima424 personas at this stage
