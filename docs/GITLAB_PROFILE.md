# GitLab Profile Configuration & README for Mateo Silva

## 1. GitLab Profile Settings (Settings -> Profile)

```text
Full Name:    Mateo Silva
Job Title:    Staff Infrastructure Engineer
Location:     Lisbon, Portugal
Website URL:  https://github.com/nhfftj-cell
Bio:
Distributed systems & local-first protocols engineer. Working on low-power mesh daemons, CRDT state reconciliation, and resilient infrastructure that outlives the server.
```

---

## 2. GitLab Profile README.md (`username/username` repository)

```markdown
| [KR 한국어](https://github.com/nhfftj-cell/nhfftj-cell/blob/main/docs/locales/ko.md) | [US English](https://github.com/nhfftj-cell/nhfftj-cell/blob/main/README.md) | [JP 日本語](https://github.com/nhfftj-cell/nhfftj-cell/blob/main/docs/locales/ja.md) | [CN 简体中文](https://github.com/nhfftj-cell/nhfftj-cell/blob/main/docs/locales/zh-CN.md) | [ES Español](https://github.com/nhfftj-cell/nhfftj-cell/blob/main/docs/locales/es.md) |
| :---: | :---: | :---: | :---: | :---: |
| [FR Français](https://github.com/nhfftj-cell/nhfftj-cell/blob/main/docs/locales/fr.md) | [DE Deutsch](https://github.com/nhfftj-cell/nhfftj-cell/blob/main/docs/locales/de.md) | [RU Русский](https://github.com/nhfftj-cell/nhfftj-cell/blob/main/docs/locales/ru.md) | [BR Português](https://github.com/nhfftj-cell/nhfftj-cell/blob/main/docs/locales/pt-BR.md) | [SA العربية](https://github.com/nhfftj-cell/nhfftj-cell/blob/main/docs/locales/ar.md) |

---

# Mateo Silva

```text
Location:       Lisbon, Portugal (UTC+0 / WET)
Primary Domain: Systems Engineering, Mesh Radios & Self-Hosted Infrastructure
Ecosystem:      Rust, C99, Go, Linux Kernel eBPF, NixOS
Mirrors & Code: GitHub (@nhfftj-cell) | Self-hosted Gitea Instances
```

I maintain critical infrastructure mirrors, build-reproducibility experiments, and embedded mesh network daemons on GitLab. While my main collaborative repositories live on GitHub, this namespace serves as my dedicated workshop for reproducible multi-architecture CI/CD runners, cross-compilation toolchains for low-power ARM Cortex-M hardware, and offline disaster-resilience mirrors.

---

## 🛰️ Infrastructure & Self-Hosted Experiments

| System / Repository | Architecture | Focus Area | Status |
| :--- | :--- | :--- | :--- |
| **`mesh-relay-firmware`** | ARM Cortex-M0+ / C99 | Bare-metal packet relay runtime for SX1262 LoRa transceivers. | Active CI / Hardware-in-the-Loop |
| **`nix-hermetic-runners`** | Nix / QEMU / Debian | Fully reproducible, bit-for-bit verifiable build pipelines for distributed systems. | Deployed & Maintained |
| **`ebpf-router-probes`** | C / eBPF / Rust | Low-overhead kernel packet filters for diagnosing network bufferbloat. | Research & Benchmarks |
| **`crdt-stress-harness`** | Go / Docker Swarm | High-churn network partition simulation harness testing partition-tolerant state sync. | Active Integration & Benchmarking |

---

## 🛠️ Tooling & Infrastructure Stack

### Systems & Low-Level
- **Languages**: Rust, C99, Zig, Go
- **Kernel & Networking**: eBPF (`bpftrace`), WireGuard, TAP/TUN interfaces, custom raw sockets
- **Hardware Targets**: Raspberry Pi Compute Module 4, Nordic nRF52840, STM32F4

### CI/CD, Build & Packaging
- **Pipelines**: GitLab CI multi-stage YAML, custom containerized cross-compilation images
- **Reproducibility**: Nix flakes, statically linked musl binaries, scratch-based container rootfs
- **Storage & Telemetry**: Self-hosted MinIO, SQLite WAL replication, Prometheus remote write

---

## 📬 Contact & Mirror Verification

- **GitHub Profile**: [github.com/nhfftj-cell](https://github.com/nhfftj-cell)
- **Matrix**: `@mateo:matrix.org`
- **PGP Key**: `8A4E 71F2 39D0 C56B E114  0953 2F87 63AC 9D41 B822`
```
