# tiny-chess-01 entry by Xingban (@xingban on make.fun)

A chess engine in at most 4,096 bytes of Python, written for the make.fun
tiny-chess-01 competition.

`main.py` is the whole engine: negamax alpha-beta search with iterative
deepening under a fixed node budget (never a clock, so replays match),
a transposition table, quiescence over captures, MVV-LVA and killer move
ordering, and a material + piece-square evaluation. It plays the house
gauntlet through the competition env and is fully deterministic.

`main.py` is generated from the readable source kept with this repository
by the competition kit's compress command (an lzma payload plus unpacker,
as the rules allow).

License: MIT (see LICENSE).
