# Tiny Chess — a 4 KB Python chess engine (make.fun bounty tiny-chess-01)

[![make.fun](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/Setiowibowo400/tiny-chess-01/rank.svg)](https://make.fun/bounty/tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/Setiowibowo400/tiny-chess-01/reward.svg)](https://make.fun/bounty/tiny-chess-01)

Entry for the [make.fun bounty: Build the strongest chess engine in 4 KB of Python](https://make.fun/bounty/tiny-chess-01) ($500).

`main.py` is the whole engine (3,554 bytes): a 0x88 board, negamax with
alpha-beta, transposition table, quiescence search with check evasions,
killer moves, MVV-LVA ordering, null-move pruning and late-move reductions,
iterative deepening to a fixed 100,000-node budget per move, and a
material + piece-square evaluation. It plays through the env at
`MAKEFUN_ENV_URL` and searches to a fixed node count, never a clock, so
replays match. The source is packed with lzma (the unpacker and payload
are both part of the 4,096 bytes).

## License

MIT — see `LICENSE`.
