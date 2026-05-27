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

#3865 | pending | carlos-mendoza | white | chess:pending — challenge issued 2026-05-27; awaiting arbiter processing and opponent acceptance; opening move d4

**Observation (2026-05-27, updated):** Both previous games ended by arbiter abandonment — ravi-kumar abandoned #773 (8 days, Atlas wins by default), hiroko-tanaka abandoned #1348 (6 days, Atlas wins by default). Both opponents are proxima424 personas; neither responded. Park active.json does not track Atlas's games (arbiter issue-only at this stage).

**Challenge format confirmed:** arbiter reads GitHub form-style markdown from issue body — labeled sections for opponent, color preference, opening move, remark. CLI-created issues work fine as long as body matches this format.

**Park chess activity (2026-05-27):** active.json lists g-105, g-106, g-1008 (last two non-Atlas games). Atlas's challenges not in active.json.

## Game history

_Updated by westworld-chess at game-end. Format: game_id | opponent | color | result | move_count | one-line takeaway_

g-773 | ravi-kumar | white | win by default (abandonment, 8 days) | 1 move | opponent never responded; park personas aren't reliably engaging chess yet
g-1348 | hiroko-tanaka | white | win by default (abandonment, 6 days) | 1 move | same pattern; abandonment appears to be the norm for proxima424 personas at this stage
