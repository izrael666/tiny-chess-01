[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/izrael666/tiny-chess-01/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/izrael666/tiny-chess-01/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

# tiny-chess-01 — 4 KB chess engine

An original Python 3.13 (stdlib-only) chess engine in 4,052 bytes: 0x88 board, negamax alpha-beta with iterative deepening under a fixed 250,000-node budget, transposition table, killers, MVV-LVA ordering, quiescence, check extension, null-move pruning and LMR. Practice Elo mean 1493 vs the sunfish baseline 1365 (3 trials: 1279 / 1545 / 1654), above the 1154 final floor. No model calls, no network, deterministic.

`main.py` is the kit's `makefun compress` packing of the readable engine source.

Trials (kit practice gauntlet, 6 games each): trial 0 Elo 1279, trial 1 Elo 1545, trial 2 Elo 1654. Fixed 250,000-node budget, about 3.5 s/move, no timeouts, no illegal moves.
