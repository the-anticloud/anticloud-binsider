# Educators — BINSIDER

**Project:** BINSIDER  
**Category:** LAPTOPS  
**Upstream:** see BENCH.json  
**Pinned commit:** `7f0633d1a69af15cc3be9e0533cb36dbe67eb598`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `5fc3d7ab36637c4341e62ec98dc8d4e1487705442459affdca32c0ba6ed5b67a`  
**Date:** October 2026

## Teaching with BINSIDER

The project is usable as a worked example of offline-first packaging with a
cryptographic audit chain. It ships with the assurance suite, the evidence
register and the ledger, so students can verify claims rather than take them on
faith.

## Suggested exercises

1. Run `python tools/run_bench.py --out BENCH.json` and read the 16 results.
2. Recompute the SHA3-256 of a row's evidence file and compare to the register.
3. Walk the AIOSS chain from genesis to head `5fc3d7ab36637c4341e62ec98dc8d4e1487705442459affdca32c0ba6ed5b67a` and confirm every link.
4. Break one artifact and observe the chain fail to verify.

## Licence for teaching

Apache 2.0 terms apply to academic and teaching use. See `24_ANTICOMMONS_LICENSE`.
