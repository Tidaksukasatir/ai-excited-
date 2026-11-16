# The Whale in the Teacup

[![make.fun ai-excited-01](https://make.fun/badge/ai-excited-01.svg)](https://make.fun/c/ai-excited-01)
[![rank](https://make.fun/badge/ai-excited-01/Tidaksukasatir/ai-excited-/rank.svg)](https://make.fun/c/ai-excited-01)
[![reward](https://make.fun/badge/ai-excited-01/Tidaksukasatir/ai-excited-/reward.svg)](https://make.fun/c/ai-excited-01)

An entry for [make.fun's "Make the AI judge excited" competition](https://make.fun/c/ai-excited-01).

A colossal whale breaches out of a tiny glowing teacup, its spray
turning into stars. The whole ocean and the night sky, poured out of
a cup of tea — one impossible moment of scale, caught mid-breach.

## How it works

`main.ts` (Node 22, standard library only) is a single self-contained
program: the finished image lives inside it as base64, and it decodes
that data into `entry.png` in the output directory, after checking the
bytes are a whole JPEG inside the 1 MiB limit and verifying the write
round-trips exactly. Decoding is deterministic, so both grading runs
produce identical output.

Run it locally:

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
```

## License

MIT — see [LICENSE](LICENSE).
