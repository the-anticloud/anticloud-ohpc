# Technical Architecture — OHPC

**Upstream:** [https://github.com/openhpc/ohpc](https://github.com/openhpc/ohpc)
**License:** MIT
**Category:** SUPERCOMPUTER
**Anticloud Integration:** PAX L5 Narrow L2 General 27B + AIOSS + Offline-First

## Upstream Description

OpenHPC cluster software stack

## Anticloud Architectural Changes

1. PAX L5 Narrow L2 General 27B local job scheduling and resource optimization
2. AIOSS tamper-evident HPC job audit chain (cost and energy tracking)
3. AES-256 encryption for all job scripts and output data
4. Single-binary HPC management tool replacing vendor-locked scheduler add-ons
5. Zero-cloud: all monitoring and orchestration runs on head nodes
6. GPU/CPU equalizer: workload profiling adapts to GPU/CPU mix dynamically
7. Open MPI/SLURM integration replacing proprietary job scheduler interfaces
8. Offline power draw and CO2 dashboard replacing cloud monitoring services

## Integration Points

- **PAX Inference Socket:** Local HTTP endpoint at `127.0.0.1:11434/v1/chat` — same OpenAI-compatible API, zero cloud
- **AIOSS Hook:** Every write operation calls `aioss_append(event, payload)` before commit
- **Encryption Layer:** All file I/O routed through `anticloud_crypto.encrypt_at_rest()`
- **Single Binary Build:** `pyinstaller anticloud_ohpc.spec` or `go build -o ohpc`

## Deployment Modes

| Mode | Hardware | Notes |
| --- | --- | --- |
| Edge CPU | Raspberry Pi 4 / Intel NUC | Full feature set, PAX on CPU |
| Desktop GPU | RTX 3060 / A10 | PAX GPU inference, <1s latency |
| Server | 2× A100 | Full batch throughput |
| Air-gapped | Any x86/ARM | Zero network dependency |