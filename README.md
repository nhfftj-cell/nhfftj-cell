| [KR 한국어](./docs/locales/ko.md) | [US English](./README.md) | [JP 日本語](./docs/locales/ja.md) | [CN 简体中文](./docs/locales/zh-CN.md) | [ES Español](./docs/locales/es.md) |
| :---: | :---: | :---: | :---: | :---: |
| [FR Français](./docs/locales/fr.md) | [DE Deutsch](./docs/locales/de.md) | [RU Русский](./docs/locales/ru.md) | [SA العربية](./docs/locales/ar.md) | [IN हिन्दी](./docs/locales/hi.md) |

---

# Mateo Silva

```text
Location:    Lisbon, Portugal (UTC+0 / WET)
Focus:       Distributed Systems, Local-First Architecture, P2P Protocols
Philosophy:  Resilient systems that outlive their central servers
Work:        Staff Infrastructure Engineer @ Distributed Storage Labs
Status:      Maintaining open protocols & hacking on low-power mesh radios
```

Hi, I am Mateo. I build software designed to work under hostile network conditions, unstable links, and zero-connectivity environments. Most of my work centers around Conflict-free Replicated Data Types (CRDTs), state synchronization over constrained bandwidth, and embedded network daemons in Rust and Go.

When not profiling memory allocations or tuning TCP congestion algorithms, you will usually find me catching waves along the Costa da Caparica, roasting single-origin espresso beans, or developing 35mm black-and-white film in my darkroom.

---

## 🔭 Current Focus & Active Research

- **Local-First Synchronization**: Refining append-only log reconciliation algorithms with deterministic conflict resolution without requiring a single source of truth.
- **Constrained Bandwidth P2P**: Exploring ultra-compact serialization formats and delta-state replication over LoRa radios and Bluetooth LE.
- **Kernel-level Network Observability**: Writing eBPF tracing probes to profile tail latency spikes across high-throughput packet routing pipelines.
- **Offline Collaborative Storage**: Building local SQLite extensions that track vector clocks natively inside SQLite B-trees.

---

## 🛠️ Featured Open Source Work

| Project | Language | Role / Status | Description |
| :--- | :--- | :--- | :--- |
| **`merkle-stream`** | Rust | Creator & Maintainer | High-performance asynchronous Merkle-tree state reconciliation library designed for intermittent wireless networks. |
| **`driftwood-kv`** | Go / WASM | Core Author | Embedded, local-first key-value store with built-in state-based CRDT primitives and zero cloud telemetry. |
| **`beacon-mesh`** | C99 / Rust | Maintainer | Lightweight routing daemon for decentralized off-grid packet relay across low-power LoRa transceivers. |
| **`polaroid-cli`** | Zig | Hobby Project | Fast terminal utility that calculates chromatic film exposure curves and converts RAW camera negative scans. |
| **`sqlite-vclock`** | C / SQLite | Author | Pluggable SQLite virtual table extension enabling multi-master concurrent branch tracking. |

---

## 💻 Technical Arsenal

### Languages & Runtime Systems
- **Primary Production**: Rust (tokio, serde, async-std), Go (concurrency, netpoll, runtime internals)
- **Low-Level & Embedded**: C99, Zig, ARM Cortex-M Assembly
- **Web & Interface Layer**: Modern TypeScript, Svelte, WebAssembly (Wasm-bindgen)
- **Scripting & Tooling**: POSIX Shell, Python (data modeling & numerical simulations), Lua

### Distributed Systems & Storage
- **Protocol Engineering**: libp2p, gRPC, Protobuf, QUIC, TCP/IP stack tuning, WireGuard
- **Replication & State**: State-based & Operation-based CRDTs, Merkle DAGs, Vector Clocks, Raft consensus
- **Storage Engines**: RocksDB, LMDB, SQLite (virtual tables, WAL mode), PostgreSQL

### Systems Engineering & Infrastructure
- **Operating Systems**: Linux (Debian, Arch Linux, Alpine), FreeBSD
- **Diagnostics & Observability**: eBPF (`bpftrace`, `bcc`), `perf`, `strace`, Wireshark, Valgrind
- **Containerization & Deployment**: Docker (scratch & multi-stage), Nix / NixOS, QEMU / KVM

---

## ⚙️ Daily Driver Setup

```text
Hardware:
├── Workstation:   Custom AMD Ryzen 9 7950X, 64GB DDR5 ECC, Fedora Silverblue
├── Laptop:        ThinkPad T14s Gen 4 (AMD), Arch Linux (kernel-hardened)
├── Terminal:      Alacritty + tmux
├── Editor:        Neovim (clean custom Lua config, zero bloat)
├── Shell:         zsh + pure prompt
└── Keyboard:      Corne 36-key split mechanical (Colemak-DH layout)
```

---

## ☕ Beyond the Terminal

- **Analog Photography**: Shoots primarily with a mechanical 1957 Leica M3 and a Hasselblad 500 C/M. Self-develops Kodak Tri-X 400 and Ilford HP5+ using D-76 chemistry.
- **Coffee Craft**: Manual lever espresso profiling on a Pavoni Europiccola. Favorite origins: washed Ethiopian Yirgacheffe and Colombian Huila.
- **Ocean & Surf**: Morning sessions at Carcavelos, Guincho, and Supertubos whenever Atlantic swells roll in.
- **Vintage Audio**: Restoring 1970s Marantz stereo receivers and maintaining an eclectic collection of Bossa Nova, Post-Rock, and Minimalist ambient vinyl records.

---

## 📬 Contact & Cryptographic Verification

I value thoughtful correspondence, asynchronous discussions, and collaborations on open, resilient software protocols.

- **Email**: `mateo [at] silva-systems [dot] dev`
- **Matrix**: `@mateo:matrix.org`
- **Mastodon**: `@mateo@hachyderm.io`
- **PGP Fingerprint**: `8A4E 71F2 39D0 C56B E114  0953 2F87 63AC 9D41 B822`

```text
-----BEGIN PGP PUBLIC KEY BLOCK-----
Comment: Mateo Silva (Personal Key - Valid through 2029)

mQGNBGXR7yYBDADK1F5N8K72YvA3k9sP2hGj...[Verified OpenPGP Key]...
=4kL9
-----END PGP PUBLIC KEY BLOCK-----
```
