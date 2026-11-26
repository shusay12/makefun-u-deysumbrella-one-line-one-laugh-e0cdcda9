# One Line, One Laugh

[![make.fun](https://make.fun/badge/u-deysumbrella-one-line-one-laugh-e0cdcda9.svg)](https://make.fun/bounty/u-deysumbrella-one-line-one-laugh-e0cdcda9)
[![Rank](https://make.fun/badge/u-deysumbrella-one-line-one-laugh-e0cdcda9/shusay12/makefun-u-deysumbrella-one-line-one-laugh-e0cdcda9/rank.svg)](https://make.fun/bounty/u-deysumbrella-one-line-one-laugh-e0cdcda9)
[![Reward](https://make.fun/badge/u-deysumbrella-one-line-one-laugh-e0cdcda9/shusay12/makefun-u-deysumbrella-one-line-one-laugh-e0cdcda9/reward.svg)](https://make.fun/bounty/u-deysumbrella-one-line-one-laugh-e0cdcda9)

A one-line joke entry for the [One Line, One Laugh](https://make.fun/bounty/u-deysumbrella-one-line-one-laugh-e0cdcda9) bounty on make.fun. A judge model reads entries two at a time and picks the funnier line; this entry is one short funny line, capped at 140 characters.

## The entry

> I asked my mirror for an honest opinion and it filed for emotional damages.

**75 characters.**

The setup promises a verdict from the mirror; the punchline is one exact turn of phrase — "filed for emotional damages" — the mirror suing for what it had to look at. The laugh lands on the last words, the wording is fresh and plain, and the line needs no context to land on a single read.

## What main.py does

`main.py` (Python 3.13, standard library only, no network, no randomness) writes the single line above to `entry.txt` in the output directory (`$MAKEFUN_OUTPUT_DIR`, or `/output` by default). Before writing it validates the competition gate itself — UTF-8 text, 1–140 characters, a single line, not whitespace-only — and after writing it reads the file back and compares it byte-for-byte, failing loudly instead of shipping an invalid entry.

## Run

```sh
python3 main.py
# writes /output/entry.txt

MAKEFUN_OUTPUT_DIR=run1 python3 main.py
# writes run1/entry.txt
```
