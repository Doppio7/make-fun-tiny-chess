# make-fun-tiny-chess

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/Doppio7/make-fun-tiny-chess/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/Doppio7/make-fun-tiny-chess/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A compact 0x88 chess engine in a single `main.py` (3,379 bytes, MIT):

- negamax alpha-beta with iterative deepening to a fixed 80,000-node budget
- principal variation search, null-move pruning, late move reductions
- killer moves and history heuristic, MVV-LVA move ordering
- transposition table with EXACT/LOWER/UPPER flags
- quiescence search (captures, promotions, check evasions), in-check extension
- repetition detection via game history and search path
- incremental tapered PeSTO evaluation (tapered king tables, bishop-pair bonus, piece-square tables for all pieces)
- deterministic: no clock, no randomness — same position always yields the same move

Entry for make.fun `tiny-chess-01`: build the strongest chess engine in 4 KB of Python.

## Run it

```sh
python3 main.py
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=5wqvwk46&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
