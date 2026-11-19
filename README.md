# TINYKNIGHT

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/leonidlouis/tinyknight/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard)
[![reward](https://make.fun/badge/tiny-chess-01/leonidlouis/tinyknight/reward.svg)](https://make.fun/bounty/tiny-chess-01)

A deterministic chess engine in 4 KB of Python 3.13, using only the standard library. Its self-contained LZMA payload implements legal chess, iterative alpha-beta search, quiescence, transpositions, null-move pruning and late-move reductions.

Tapered evaluation covers material, king safety, pawn structure and passed pawns. History-aware search avoids repetitions, while endgame guidance helps convert wins. A fixed node budget scales with game phase; search never reads a clock.

Run against the make.fun environment:

    MAKEFUN_ENV_URL=http://localhost:8080 python3 main.py
