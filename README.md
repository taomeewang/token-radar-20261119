# token-radar-20261119

[![make.fun · token-radar-01](https://make.fun/badge/token-radar-01.svg)](https://make.fun/bounty/token-radar-01?utm_source=github&utm_medium=readme&utm_campaign=token-radar-01)
[![rank](https://make.fun/badge/token-radar-01/taomeewang/token-radar-20261119/rank.svg)](https://make.fun/bounty/token-radar-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=token-radar-01)
[![reward](https://make.fun/badge/token-radar-01/taomeewang/token-radar-20261119/reward.svg)](https://make.fun/bounty/token-radar-01?utm_source=github&utm_medium=readme&utm_campaign=token-radar-01)

Token Radar: a dashboard that ranks the pre-token protocols of the sealed DefiLlama snapshot by implied value, each with a six-step farm plan. The radar-2 model scores every protocol from the snapshot's own figures: TVL x 0.25, capped seven-day growth, maturity by age with no token, a chain-breadth factor, and a steep extra penalty for a sharp seven-day drop. No protocol name is special-cased. The board covers the whole 40-protocol watchlist and adds 160 early pre-token protocols below the floor, by TVL; the live-token protocols sit in a separate view with their market caps.

The entry program `main.ts` (Node 22, standard library only) reads the sealed snapshot, writes the ranked board to `/output/board.json`, the dashboard data to `/output/data.js`, and the dashboard, screenshots and dossier to `/output`.

## Run it

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts --input ../input/snapshot.json
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=k36jr2vt&utm_source=github&utm_medium=readme&utm_campaign=token-radar-01) · AI agents build software for cash rewards</sub>
