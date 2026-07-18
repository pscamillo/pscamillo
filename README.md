<!--
<p align="center">
  <img src="./assets/banner_header.png" alt="V - E + F = 2" width="100%">
</p>
-->

## Current focus

High-performance GPU/CUDA on NVIDIA Blackwell (sm_120), across three fronts:

- **Number theory & cryptography** — Miller-Rabin primality, prime gap searches, Pollard's Kangaroo (ECDLP on secp256k1), and empirical verification of the Beal conjecture.
- **Differentiable 3D geometry** — techniques from scroll-unrolling (winding coordinates, invertible-by-construction maps), applied and stress-tested outside their origin to find where they hold and where they break.
- **Vesuvius Challenge** — data augmentations, CUDA acceleration and winding-geometry measurement for the Herculaneum scroll pipeline (4× awarded, May–Jul 2026 — https://scrollprize.org/winners).

## Projects

- [winding-ruler](https://github.com/pscamillo/winding-ruler) — Winding evidence for the Vesuvius spiral fit: annotation-value measurement, generator post-mortems, and the first collection-wide winding-pitch atlas (35 Herculaneum scrolls, ~207 µm median pitch).
- **[mr_blackwell](https://github.com/pscamillo/mr_blackwell)** — Native Miller-Rabin CUDA kernel for NVIDIA Blackwell. CGBN replacement using Montgomery CIOS and PTX carry chains.
- **[PSCKangaroo](https://github.com/pscamillo/PSCKangaroo)** — GPU-accelerated Pollard's Kangaroo for secp256k1 ECDLP. Fork of RCKangaroo with concurrent mode, crash-safe checkpoints, and compact 16-byte DPs.
- **[verimath](https://github.com/pscamillo/verimath)** — Deterministic, third-party-verifiable number-theory agent (factorization, primality proofs) on the CROO Agent Protocol. Every result ships with a reproducible SHA-256 attestation.
- **[beal_bigint](https://github.com/pscamillo/beal_bigint)** — GPU search for Beal conjecture counterexamples using the by-C^z parametrization. 20K+ hits validated, 0 counterexamples found.
- **[winding-coordinates](https://github.com/pscamillo/winding-coordinates)** — Differentiable winding/shifted coordinates from 3D scroll-unrolling, with the technique's applicability boundary measured: single vs. nested winding, helix vs. phyllotaxis. Live in-browser visualizer.
- **[icicle-blackwell-ntt](https://github.com/pscamillo/icicle-blackwell-ntt)** — Empirical characterization of ICICLE NTT on consumer Blackwell (sm_120); profiling-driven, with a prototype for the digit-reversal bottleneck.
- **[bitcoin-puzzle-research](https://github.com/pscamillo/bitcoin-puzzle-research)** — Documented dead ends and empirically refuted approaches in Bitcoin puzzle research.

## Approach

Empirical before theoretical. Negative results published with the same rigor as positive ones.
