# Ways of working

## 2026-11-02 — Fail closed when a comparison cannot be read

A shell script using `set -uo pipefail` does not automatically stop after a failing command substitution. Check the `git diff` result explicitly before interpreting its output as an empty comparison. Keep an invalid revision trap alongside valid in-surface, forbidden-change and empty-comparison controls.
