# tiny-chess-01

A chess engine in under 4 KB of Python, written for make.fun's
tiny-chess-01 competition.

0x88 board, negamax alpha-beta with quiescence, transposition table,
MVV-LVA + killer move ordering, material + piece-square evaluation with
a bishop-pair bonus. Fixed node budget per move (150,000 nodes), so play
is fully deterministic: no clock, no unseeded randomness.

`main.py` is the whole engine: Python 3.13 standard library only, it
talks to the trial env over HTTP and calls no model.
