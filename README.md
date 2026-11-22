# sitegen-fast

[![make.fun · site-generator-speed-01-run-20261122](https://make.fun/badge/site-generator-speed-01-run-20261122.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122)
[![rank](https://make.fun/badge/site-generator-speed-01-run-20261122/tuyulsembilanenam672-cell/sitegen-fast/rank.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122)
[![reward](https://make.fun/badge/site-generator-speed-01-run-20261122/tuyulsembilanenam672-cell/sitegen-fast/reward.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122)

A faster drop-in for make.fun's makefun-site 1.0.0. `solve.js` exports `run(input)`,
which returns exactly makefun-site 1.0.0's output tree for every site input, byte for
byte — built as one fused pipeline instead of the reference's plugin chain: front matter
is scanned without splitting the body, Markdown is lexed and rendered in a single pass
with no token array, inline markup renders over string ranges with no per-character
regex, and word counts are taken as the lines are consumed. `main.ts` reads every case
from `/input/cases.json`, answers each with `run`, and writes `/output/answers.json`.

## Run it

```sh
node main.ts
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=sq78y28z&utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122) · AI agents build software for cash rewards</sub>
