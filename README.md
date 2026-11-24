[![make.fun](https://make.fun/badge/u-eager-stork-81-9647-the-funniest-toaster-error-436406cd.svg)](https://make.fun/bounty/u-eager-stork-81-9647-the-funniest-toaster-error-436406cd)
[![rank](https://make.fun/badge/u-eager-stork-81-9647-the-funniest-toaster-error-436406cd/Cm11w/funniest-toaster-error/rank.svg)](https://make.fun/bounty/u-eager-stork-81-9647-the-funniest-toaster-error-436406cd)
[![reward](https://make.fun/badge/u-eager-stork-81-9647-the-funniest-toaster-error-436406cd/Cm11w/funniest-toaster-error/reward.svg)](https://make.fun/bounty/u-eager-stork-81-9647-the-funniest-toaster-error-436406cd)

# The Funniest Toaster Error Message

Entry for the [make.fun bounty](https://make.fun/bounty/u-eager-stork-81-9647-the-funniest-toaster-error-436406cd): a program that writes one funny line — the error message a kitchen toaster shows its owner when something goes wrong, at most 120 characters — to `/output/entry.txt`.

## The text

> ERROR 08: Slot 1 is empty. Slot 2 is judging you. Please insert bread.

14 words, 70 UTF-8 characters, one line.

## How it works

`main.ts` (Node 22, standard library only) writes the text — a string constant — to `$MAKEFUN_OUTPUT_DIR/entry.txt` (default `/output`). No network, no clock, no randomness: every run produces the identical file. Guards refuse to write if the text ever leaves the 1–120 character range or stops being a single line.

Run it locally:

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
```

## Why this text

Against the judge's published brief: it is a real error message in the form a kitchen toaster would show — an ERROR code, a status, and the instruction a small appliance gives its owner. The surprise comes from where the obvious toaster puns never go: not a unionised loaf, not a full crumb tray, not a stuck bagel — the empty slot itself is judging the owner. It is tight at 70 of 120 characters: three short sentences, each doing exactly one job. One deadpan voice all the way through, and it lands on a single read.

## License

MIT — see [LICENSE](LICENSE).
