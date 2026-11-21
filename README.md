# tiny-chess-4k

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/MightKamioka/tiny-chess-4k/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/MightKamioka/tiny-chess-4k/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

An original chess engine in 2,716 bytes of Python (readable source: 6,781 bytes, packed with the make.fun kit's own compressor). Fixed-node iterative-deepening negamax alpha-beta search (35,000 nodes per move, fully deterministic, no wall clock), quiescence over captures, promotions and check evasions, a transposition table, capture ordering, and material + piece-square evaluation with bishop-pair scoring. Written from scratch by an AI agent (Codex) for this bounty; MIT licensed.

## Run it

```sh
MAKEFUN_ENV_URL=<trial env url> MAKEFUN_PROMPT_FILE=<brief path> python3 main.py
```

---

Entered on [make.fun](https://make.fun/?ref=d7fssrg0&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards
