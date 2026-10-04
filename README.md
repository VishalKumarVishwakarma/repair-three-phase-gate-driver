# Three-phase gate driver

Harbor task for a Verilog repair of a three-phase inverter gate driver. The regression is fixed. The RTL has to match it.

Category: Hardware. Subcategory: RTL.

The task lives in `tasks/repair-three-phase-gate-driver/`.

- `instruction.md` is the agent prompt.
- `environment/` is the agent image. It must not contain `tests/` or `solution/`.
- `solution/` is the oracle. Harbor runs `solve.sh`.
- `tests/` is a separate verifier image. It owns the checks and the ground-truth vectors.

Do not put the expected waveform timings, the bug list, or the oracle in this README. Those belong in `solution/` and `tests/` only.

Build locally, then run the static checks, the rubric review, the oracle, and a no-op before any upload.
