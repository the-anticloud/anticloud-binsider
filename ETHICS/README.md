# Ethics — BINSIDER

**Project:** BINSIDER  
**Category:** LAPTOPS  
**Upstream:** see BENCH.json  
**Pinned commit:** `7f0633d1a69af15cc3be9e0533cb36dbe67eb598`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `5fc3d7ab36637c4341e62ec98dc8d4e1487705442459affdca32c0ba6ed5b67a`  
**Date:** October 2026

## Position

BINSIDER is packaged for offline deployment with a verifiable audit trail. The
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
