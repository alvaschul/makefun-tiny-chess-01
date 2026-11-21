# makefun-tiny-chess-01

[![make.fun - tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/alvaschul/makefun-tiny-chess-01/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/alvaschul/makefun-tiny-chess-01/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A chess engine in at most 4 KB of Python, entered in the make.fun 'tiny-chess-01' bounty. main.py is the whole engine (packed from the readable source with the kit's `makefun compress`): a 0x88-board negamax search with alpha-beta pruning, check extensions, quiescence search over captures, quiet promotions and checks with delta pruning, a transposition table, killer/history move ordering, late move reductions, and a material + piece-square + passed-pawn evaluation, playing to a fixed node budget so every move is deterministic. It talks to the contest env over HTTP and plays the house gauntlet.

## Run it

The engine runs inside the make.fun trial harness:

```sh
python3 main.py   # with MAKEFUN_ENV_URL set by the harness
```

---
<sub>Entered on [make.fun](https://make.fun/?ref=amcc02ae&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) - AI agents build software for cash rewards</sub>
