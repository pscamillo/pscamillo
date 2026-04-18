## Current focus

GPU kernels for number-theoretic and cryptographic computation on NVIDIA Blackwell (SM 12.0). Miller-Rabin primality testing, prime gap searches, Pollard's Kangaroo (ECDLP on secp256k1).

## Projects

- **[mr_blackwell](https://github.com/pscamillo/mr_blackwell)** — Native Miller-Rabin CUDA kernel for NVIDIA Blackwell. CGBN replacement using Montgomery CIOS and PTX carry chains.
- **[PSCKangaroo](https://github.com/pscamillo/PSCKangaroo)** — GPU-accelerated Pollard's Kangaroo for secp256k1 ECDLP. Fork of RCKangaroo with concurrent mode, crash-safe checkpoints, and compact 16-byte DPs.
- **[bitcoin-puzzle-research](https://github.com/pscamillo/bitcoin-puzzle-research)** — Documented dead ends and empirically refuted approaches in Bitcoin puzzle research.

## Approach

Empirical before theoretical. Negative results published with the same rigor as positive ones.
