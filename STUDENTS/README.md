# Students — BINSIDER

**Project:** BINSIDER  
**Category:** LAPTOPS  
**Upstream:** see BENCH.json  
**Pinned commit:** `7f0633d1a69af15cc3be9e0533cb36dbe67eb598`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `5fc3d7ab36637c4341e62ec98dc8d4e1487705442459affdca32c0ba6ed5b67a`  
**Date:** October 2026

## What this project gives you

A complete worked example of offline-first packaging with a cryptographic audit
chain: source pinned at `7f0633d1a69af15cc3be9e0533cb36dbe67eb598`, a 16-check assurance suite, an evidence register
with per-check hashes, and an AIOSS ledger chain ending at `5fc3d7ab36637c4341e62ec98dc8d4e1487705442459affdca32c0ba6ed5b67a`.

## Learn by verifying

```
python tools/run_bench.py --out BENCH.json
```

Then take any row from `ISOLATED_LAB_RESULTS/03_Result_Register.md`, recompute
the SHA3-256 of its evidence file, and confirm it matches. If it does not match,
the record has been altered — that is the whole point of the chain.

## Licence

Apache 2.0 terms apply to study and teaching use.
