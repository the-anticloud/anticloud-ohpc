# Students — OHPC

**Project:** OHPC  
**Category:** SUPERCOMPUTER  
**Upstream:** see BENCH.json  
**Pinned commit:** `25f7acb93d4e0536e3cb8d47c2a055c12a4fe1e5`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `2d7ce2cf82d0e85230c13bda111ad7af94a6a690c226f25dfdfd534916a61bf6`  
**Date:** October 2026

## What this project gives you

A complete worked example of offline-first packaging with a cryptographic audit
chain: source pinned at `25f7acb93d4e0536e3cb8d47c2a055c12a4fe1e5`, a 16-check assurance suite, an evidence register
with per-check hashes, and an AIOSS ledger chain ending at `2d7ce2cf82d0e85230c13bda111ad7af94a6a690c226f25dfdfd534916a61bf6`.

## Learn by verifying

```
python tools/run_bench.py --out BENCH.json
```

Then take any row from `ISOLATED_LAB_RESULTS/03_Result_Register.md`, recompute
the SHA3-256 of its evidence file, and confirm it matches. If it does not match,
the record has been altered — that is the whole point of the chain.

## Licence

Apache 2.0 terms apply to study and teaching use.
