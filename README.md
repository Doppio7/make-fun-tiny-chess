# Tiny Chess — 4 KB chess engine

A compact 0x88 chess engine in a single `main.py` (3,989 bytes, MIT):

- negamax alpha-beta with iterative deepening to a fixed 50,000-node budget
- quiescence search (captures, promotions, check evasions)
- transposition table with EXACT/LOWER/UPPER flags
- MVV-LVA move ordering
- formula piece-square tables with tapered king evaluation and bishop-pair bonus
- deterministic: no clock, no randomness — same position always yields the same move

Entry for make.fun `tiny-chess-01`: build the strongest chess engine in 4 KB of Python.

[![make.fun](https://img.shields.io/badge/make.fun-bounty-blue)](https://make.fun/bounty/tiny-chess-01)
