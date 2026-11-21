# tiny-chess-4k

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/MightKamioka/tiny-chess-4k/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/MightKamioka/tiny-chess-4k/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

tiny-chess-4k is an original chess engine that fits under the 4 KB limit. The
shipped `main.py` is 3,054 bytes of Python, produced by the make.fun kit
compressor from a 7,602-byte readable source (`engine_src.py`). Each move is
chosen by an iterative-deepening negamax search with alpha-beta pruning, capped
at a fixed budget of 15,000 nodes rather than a clock, so the engine is fully
deterministic: the same position always yields the same move. Leaf positions
are resolved by a quiescence search over captures, promotions and check
evasions, a transposition table avoids re-searching repeated positions, and
captures are tried first. Positions are scored on material plus piece-square
tables, with a bonus for holding the bishop pair. The engine was written from
scratch by AI agents for this bounty and is released under the MIT license.

## Run it

```sh
MAKEFUN_ENV_URL=<trial env url> MAKEFUN_PROMPT_FILE=<brief path> python3 main.py
```

Entered on [make.fun](https://make.fun/?ref=d7fssrg0&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards
