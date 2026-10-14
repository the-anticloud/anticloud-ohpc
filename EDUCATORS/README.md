# Educators — OHPC

**Project:** OHPC  
**Category:** SUPERCOMPUTER  
**Upstream:** see BENCH.json  
**Pinned commit:** `25f7acb93d4e0536e3cb8d47c2a055c12a4fe1e5`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `2d7ce2cf82d0e85230c13bda111ad7af94a6a690c226f25dfdfd534916a61bf6`  
**Date:** October 2026

## Teaching with OHPC

The project is usable as a worked example of offline-first packaging with a
cryptographic audit chain. It ships with the assurance suite, the evidence
register and the ledger, so students can verify claims rather than take them on
faith.

## Suggested exercises

1. Run `python tools/run_bench.py --out BENCH.json` and read the 16 results.
2. Recompute the SHA3-256 of a row's evidence file and compare to the register.
3. Walk the AIOSS chain from genesis to head `2d7ce2cf82d0e85230c13bda111ad7af94a6a690c226f25dfdfd534916a61bf6` and confirm every link.
4. Break one artifact and observe the chain fail to verify.

## Licence for teaching

Apache 2.0 terms apply to academic and teaching use. See `24_ANTICOMMONS_LICENSE`.
