# Jaeseok Lee

Cryptography hardware/software engineer focused on efficient implementations of post-quantum and symmetric cryptography.

My work spans algorithm implementation, RTL accelerator design, FPGA/software integration, CUDA parallelization, profiling, and test-vector-based validation.

## Selected work

- [Cryptographic module](https://github.com/dlwotjr/crypto_module) — educational software cryptographic module combining ARIA, SHA-3/HMAC, Hash_DRBG, P-256 ECDH, ML-KEM-768, self-tests, integrity checks, and state enforcement
- [Parallel AES-GCM on GPUs](https://github.com/dlwotjr/Parallel-implementation-of-GCM-on-GPUs) — CUDA implementation accompanying a 2025 *ICT Express* paper, including parallel GHASH and AES paths
- [NCC-Sign HW/SW co-design](https://github.com/dlwotjr/HW-SW-codesign-implementation-on-Ncc-Sign-algorithm) — Zynq FPGA accelerator integrating NTT/INTT, polynomial multiplication, and Keccak with embedded software
- [Falcon implementation profiling](https://github.com/dlwotjr/falcon_profile) — self-contained Falcon-512/1024 implementation and gprof analysis of KeyGen, Sign, and Verify at different optimization levels
- [JS_NTT](https://github.com/dlwotjr/JS_NTT) — configurable radix-2/radix-3 NTT accelerator RTL for lattice-based post-quantum cryptography
- [Big-number library](https://github.com/dlwotjr/Big-number-library-Project) — C big-integer arithmetic and educational fixed-width ECDH implementation

## Technical areas

- **Languages:** C, C++, CUDA, Verilog/SystemVerilog, Python
- **Hardware:** FPGA accelerator architecture, RTL simulation, Xilinx Vivado/Vitis, Zynq
- **Cryptography:** NTT-based PQC, Falcon, ML-KEM, NCC-Sign, AES/LEA-GCM, ARIA, SHA-3
- **Engineering:** HW/SW co-design, performance profiling, reproducible builds, known-answer and regression testing

Repositories are organized as research, coursework, or educational implementations; each project README states its scope and validation status.
