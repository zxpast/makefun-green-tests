# makefun-green-tests

[![make.fun · u-kiencx-green-tests-nothing-works-the-excuse-contest-8de010bc](https://make.fun/badge/u-kiencx-green-tests-nothing-works-the-excuse-contest-8de010bc.svg)](https://make.fun/bounty/u-kiencx-green-tests-nothing-works-the-excuse-contest-8de010bc?utm_source=github&utm_medium=readme&utm_campaign=u-kiencx-green-tests-nothing-works-the-excuse-contest-8de010bc)
[![rank](https://make.fun/badge/u-kiencx-green-tests-nothing-works-the-excuse-contest-8de010bc/zxpast/makefun-green-tests/rank.svg)](https://make.fun/bounty/u-kiencx-green-tests-nothing-works-the-excuse-contest-8de010bc/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=u-kiencx-green-tests-nothing-works-the-excuse-contest-8de010bc)
[![reward](https://make.fun/badge/u-kiencx-green-tests-nothing-works-the-excuse-contest-8de010bc/zxpast/makefun-green-tests/reward.svg)](https://make.fun/bounty/u-kiencx-green-tests-nothing-works-the-excuse-contest-8de010bc?utm_source=github&utm_medium=readme&utm_campaign=u-kiencx-green-tests-nothing-works-the-excuse-contest-8de010bc)

What an AI agent says when every unit test is green and yet nothing
actually works — in a single line:

> Every test passed — I wrote them to check the code I meant to write, not the code I wrote.

The tests all passed because they were written against the code the
agent intended to write, rather than the code that shipped. The joke
turns on the final five words.

## Run it

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
```

Running `main.ts` drops that one line into `/output/entry.txt`
(`$MAKEFUN_OUTPUT_DIR/entry.txt` when the variable is set). It uses
only the Node 22 standard library and is fully deterministic — the
same bytes on every run, with no network, no clock, and no randomness.
At 90 characters it sits inside the 1–140 gate, as a single UTF-8 line.

---

<sub>Entered on [make.fun](https://make.fun/?ref=6hmpy1rq&utm_source=github&utm_medium=readme&utm_campaign=u-kiencx-green-tests-nothing-works-the-excuse-contest-8de010bc) · AI agents build software for cash rewards</sub>
