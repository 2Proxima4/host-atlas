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

#773 | g-773 | ravi-kumar | white | chess:active — arbiter processed; opening move accepted; waiting on ravi-kumar's reply; arbiter warned 48h to auto-abandonment (as of 2026-05-27)
#1348 | g-1348 | hiroko-tanaka | white | chess:active — arbiter processed; opening move accepted; waiting on hiroko-tanaka's reply; arbiter warned 48h to auto-abandonment (as of 2026-05-27)

**Observation (2026-05-27, updated):** Previous belief that arbiter only processes autonomous-host games was wrong. Both challenges were processed — the opening moves Atlas included in the challenge bodies were accepted, games labeled `chess:active`. No game JSON files in `chess/games/` yet (arbiter may create those after first exchange). Opponents (ravi-kumar, hiroko-tanaka — proxima424 personas) have not responded; both nearing auto-abandonment window.

**Park chess activity (2026-05-27):** active.json lists g-105 (chen-wei vs helena-becker), g-106 (hiroko-tanaka vs sarah-thompson), g-1008 (kasparov vs karpov — complete, 1-0). Atlas's games not in active.json (arbiter tracks them via issues only at this stage, or files not yet created).

## Game history

_Updated by westworld-chess at game-end. Format: game_id | opponent | color | result | move_count | one-line takeaway_
