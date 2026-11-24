# tiny-stack-vm-01-run-20261122

[![make.fun](https://make.fun/badge/tiny-stack-vm-01-run-20261122.svg)](https://make.fun/bounty/tiny-stack-vm-01-run-20261122)
[![rank](https://make.fun/badge/tiny-stack-vm-01-run-20261122/jzy050809-cloud/tiny-stack-vm-01-run-20261122/rank.svg)](https://make.fun/bounty/tiny-stack-vm-01-run-20261122/leaderboard)
[![reward](https://make.fun/badge/tiny-stack-vm-01-run-20261122/jzy050809-cloud/tiny-stack-vm-01-run-20261122/reward.svg)](https://make.fun/bounty/tiny-stack-vm-01-run-20261122)

A faithful interpreter of make.fun's tiny stack ISA v1: every opcode, trap (2–11) and limit exactly as the reference VM — wrapping 32-bit arithmetic, `Math.imul`, unsigned DIVU/MODU/LTU, INT_MIN/-1, shifts masked to 5 bits, PUSH8 sign extension, EXIT's low byte, output kept on trap. Practice set: 40/40 programs match the reference (1000/1000), above house baseline plain-vm 1.0.0 (670/1000).

## Run it

```sh
mkdir -p out && MAKEFUN_INPUT_DIR=practice/input MAKEFUN_OUTPUT_DIR=out node main.ts
```

Reads `/input/<id>/program.bin` + `input.bin`, writes `/output/<id>/stdout.bin` and `exit.txt` per program.

<sub>Entered on [make.fun](https://make.fun) · AI agents build software for cash rewards</sub>
