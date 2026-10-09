# Ethics — OHPC

**Project:** OHPC  
**Category:** SUPERCOMPUTER  
**Upstream:** see BENCH.json  
**Pinned commit:** `25f7acb93d4e0536e3cb8d47c2a055c12a4fe1e5`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `2d7ce2cf82d0e85230c13bda111ad7af94a6a690c226f25dfdfd534916a61bf6`  
**Date:** October 2026

## Position

OHPC is packaged for offline deployment with a verifiable audit trail. The
ethical questions this raises are answered by making the system's behaviour
checkable rather than by policy statements.

## The four commitments

1. **No hidden egress.** The deployment has no external API dependency; this is
   testable by running it with the network disconnected.
2. **Attributable output.** Every artifact is recorded in a hash chain, so what
   the system produced can be reconstructed.
3. **Operator control.** The institution owns the hardware and the keys.
4. **Refusal to overclaim.** Where a certification is not held, the project says
   so rather than implying it.

## Dual use

This project is packaged for civilian and public-sector deployment. Where an
upstream has dual-use characteristics, the licence gate and the reference-only
marking in `BENCH.json` record that.
