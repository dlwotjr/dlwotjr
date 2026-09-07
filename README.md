# Jaeseok Lee

Cryptography hardware/software engineer focused on efficient implementations of post-quantum and symmetric cryptography.

I work across RTL accelerator architecture, FPGA/software integration, CUDA parallelization, C cryptographic modules, profiling, and test-vector-based validation.

## RTL / Hardware

| Project | Focus |
|---|---|
| [Unified NTT — AXI4-Stream](https://github.com/dlwotjr/unified-ntt-axi-stream-mc) | Multi-radix NTT/INTT accelerator for ML-DSA, ML-KEM, HAETAE, NTRU+, and Falcon; AXI4-Stream/AXI DMA Zynq integration at 150 MHz |
| [Unified NTT — AXI BRAM](https://github.com/dlwotjr/unified-ntt-axi-bram-mc) | Memory-mapped counterpart with packed 32-bit coefficient storage and direct AXI BRAM Controller access; includes BRAM/CDMA variants and board artifacts |
| [NCC-Sign HW/SW co-design](https://github.com/dlwotjr/HW-SW-codesign-implementation-on-Ncc-Sign-algorithm) | Zynq accelerator integrating NTT/INTT, point-wise multiplication, and Keccak with embedded signing software |
| [JS_NTT](https://github.com/dlwotjr/JS_NTT) | Configurable radix-2/radix-3 NTT accelerator RTL and software-reference simulation material |
| [Ibex RISC-V custom instruction & PQC lab](https://github.com/dlwotjr/ibex-pqc-experiments) | Ibex CUSTOM-0 decoder/ALU integration, inline-assembly verification, and bare-metal ML-KEM, ML-DSA, and Falcon porting on Verilator |
| [FPGA RTL Design Experience](https://github.com/dlwotjr/FPGA-RTL-Design-Experience) | Self-authored Korean guide connecting RTL coding styles to LUT, FF, carry-chain, DSP, BRAM, timing, and routing results |
| [HDLBits practice](https://github.com/dlwotjr/HDL_Bits) | Verilog exercise solutions and Korean digital-design study notes |

The two unified-NTT repositories expose the same arithmetic direction through different system interfaces, making the data-movement and resource-cost trade-offs directly comparable.

## GPU / Parallel Computing

| Project | Focus |
|---|---|
| [Parallel AES-GCM on GPUs](https://github.com/dlwotjr/Parallel-implementation-of-GCM-on-GPUs) | CUDA implementation accompanying the 2025 *ICT Express* paper “Parallel implementation of GCM on GPUs,” including parallel GHASH and AES paths |
| [LEA block-cipher mode experiments](https://github.com/dlwotjr/LEA_GCM) | C++/CUDA experiments covering LEA-CBC, LEA-GCM, table-based GHASH, and parallel authenticated encryption |

## C / Cryptography

| Project | Focus |
|---|---|
| [ESP32-S3 ML-DSA Kronecker+](https://github.com/dlwotjr/esp32s3-mldsa-kronecker-plus) | Reuses the ESP32-S3 RSA MODMULT accelerator for ML-DSA polynomial products; covers `c·s`, `c·t1`, constant-time `c·t0`, parameter-width analysis, board benchmarks, and Xtensa CT/GS butterfly assembly |
| [Cryptographic module](https://github.com/dlwotjr/crypto_module) | Educational module combining ARIA, SHA-3/HMAC, Hash_DRBG, P-256 ECDH, ML-KEM-768, self-tests, integrity checks, and state enforcement |
| [Falcon implementation profiling](https://github.com/dlwotjr/falcon_profile) | Self-contained Falcon-512/1024 implementation and gprof analysis of KeyGen, Sign, and Verify under `-O0` and `-O3` |
| [Big-number library](https://github.com/dlwotjr/Big-number-library-Project) | C big-integer arithmetic, modular reduction/inversion, elliptic-curve operations, and educational fixed-width ECDH |

## Technical stack

- **Languages:** C, C++, CUDA, Verilog/SystemVerilog, Python
- **Hardware:** Xilinx Vivado/Vitis, Zynq, ESP32-S3/Xtensa LX7, Ibex/RISC-V, Verilator, FuseSoC, AXI4-Lite, AXI4-Stream, AXI BRAM Controller, RTL simulation and timing closure
- **Cryptography:** NTT-based PQC, Falcon, ML-KEM, ML-DSA, NCC-Sign, AES/LEA-GCM, ARIA, SHA-3
- **Engineering:** HW/SW co-design, performance profiling, reproducible builds, KAT and regression testing

Each repository README identifies whether the work is research, coursework, educational material, or a reproducibility package, together with its build and validation scope.
