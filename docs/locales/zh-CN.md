| [KR 한국어](./ko.md) | [US English](../../README.md) | [JP 日本語](./ja.md) | [CN 简体中文](./zh-CN.md) | [ES Español](./es.md) |
| :---: | :---: | :---: | :---: | :---: |
| [FR Français](./fr.md) | [DE Deutsch](./de.md) | [RU Русский](./ru.md) | [BR Português](./pt-BR.md) | [SA العربية](./ar.md) |

---

# 马特奥·席尔瓦 (Mateo Silva)

```text
常驻地:      葡萄牙里斯本 (UTC+0 / WET)
技术专长:    分布式系统、本地优先架构 (Local-First)、点对点协议 (P2P)
工程哲学:    打造生命周期超越中央服务器的高韧性软件
当前职位:    Distributed Storage Labs 资深基础设施架构师
当前状态:    维护开放网络协议，探索低功耗无线网状网络 (Mesh)
```

你好，我是马特奥。我致力于设计并开发在严苛网络环境、不稳链路甚至完全离线条件下依然能够稳定运行的软件系统。我的工作主要集中于无冲突复制数据类型 (CRDT)、极度受限带宽下的状态同步机制，以及使用 Rust 和 Go 构建高效的轻量级嵌入式网络守护进程。

在不分析内存分配细节或调优 TCP 拥塞控制参数时，你通常可以在卡帕里卡海岸 (Costa da Caparica) 看到我冲浪的身影，或者在暗房中冲洗 35 毫米黑白胶片、烘焙单一产地的浓缩咖啡豆。

---

## 🔭 当前关注方向与活跃研究

- **本地优先 (Local-First) 状态同步**：优化纯追加式日志 (Append-only Log) 状态调和算法，在无需单一权威数据源的前提下实现确定性冲突解决。
- **超低带宽 P2P 通信**：探索基于 LoRa 无线电设备与低功耗蓝牙 (BLE) 的超紧凑序列化数据格式与增量状态 (Delta-state) 复制机制。
- **内核级网络可观测性**：编写 eBPF 追踪探针，精确定位高吞吐数据包路由链路中的长尾延迟 (Tail Latency) 尖峰。
- **离线协作式存储引擎**：开发能在 SQLite B 树底层原生跟踪向量时钟 (Vector Clocks) 的 C 语言虚拟表扩展。

---

## 🛠️ 精选开源项目

| 项目名称 | 开发语言 | 角色 / 状态 | 详细介绍 |
| :--- | :--- | :--- | :--- |
| **`merkle-stream`** | Rust | 作者 & 维护者 | 专为间歇性无线通信网络设计的高性能异步默克尔树 (Merkle-tree) 状态调和算法库。 |
| **`driftwood-kv`** | Go / WASM | 核心设计者 | 内置基于状态的 CRDT 原语且零云端遥测的嵌入式本地优先键值数据库。 |
| **`beacon-mesh`** | C99 / Rust | 维护者 | 运行在低功耗 LoRa 射频硬件上、适用于脱网极端环境的去中心化数据包中继路由守护程序。 |
| **`polaroid-cli`** | Zig | 个人业余项目 | 用于精确计算胶片感光曲线并转换相机 RAW 负片扫描件的高性能终端工具。 |
| **`sqlite-vclock`** | C / SQLite | 作者 | 赋予 SQLite 原生支持多主节点并发分支版本追踪能力的可插拔虚拟表模块。 |

---

## 💻 技术储备与工程工具箱

### 编程语言与底层运行时
- **核心生产力**：Rust (tokio, serde, async-std), Go (高并发调度, netpoll 机制, 运行时内核)
- **底层与嵌入式**：C99, Zig, ARM Cortex-M 汇编
- **前端与交互层**：现代 TypeScript, Svelte, WebAssembly (Wasm-bindgen)
- **脚本与自动化**：POSIX Shell, Python (数据建模与数值模拟), Lua

### 分布式通信与存储架构
- **网络协议工程**：libp2p, gRPC, Protobuf, QUIC, TCP/IP 内核栈调优, WireGuard
- **数据复制模型**：状态型/操作型 CRDT, Merkle DAG, Vector Clock, Raft 一致性协议
- **嵌入式存储引擎**：RocksDB, LMDB, SQLite (虚拟表, WAL 模式), PostgreSQL

### 系统底层剖析与基础设施
- **操作系统平台**：Linux (Debian, Arch Linux, Alpine), FreeBSD
- **性能剖析与诊断**：eBPF (`bpftrace`, `bcc`), `perf`, `strace`, Wireshark, Valgrind
- **容器与环境配置**：Docker (多阶段与 scratch 构建), Nix / NixOS, QEMU / KVM

---

## ⚙️ 个人开发环境与硬件配置

```text
硬件与工作台:
├── 主力工作站:   AMD Ryzen 9 7950X, 64GB DDR5 ECC 内存, Fedora Silverblue
├── 移动笔电:     ThinkPad T14s Gen 4 (AMD), Arch Linux (内核加固版)
├── 终端模拟器:   Alacritty + tmux
├── 代码编辑器:   Neovim (基于 Lua 的纯净轻量定制配置)
├── Shell 环境:  zsh + pure 提示符
└── 键盘外设:     Corne 36键 分体式机械键盘 (Colemak-DH 键位配列)
```

---

## ☕ 终端之外的生活

- **胶片摄影**：主力使用 1957 年产机械旁轴相机徕卡 M3 (Leica M3) 以及哈苏 500 C/M 中画幅相机。坚持在暗房中用 D-76 配方手工冲洗柯达 Tri-X 400 与伊尔福 HP5+ 黑白胶卷。
- **咖啡冲煮**：使用经典手动拉杆意式机 La Pavoni Europiccola 精确控制变压萃取。钟情于水洗埃塞俄比亚耶加雪菲与哥伦比亚慧兰产区的风味。
- **大西洋冲浪**：每当大西洋涌起风浪的清晨，便前往卡尔卡维卢什 (Carcavelos)、金舒 (Guincho) 或超管浪海滩 (Supertubos) 逐浪。
- **中古音频设备修复**：热爱修复 20 世纪 70 年代的马兰士 (Marantz) 模拟功放，并收集波萨诺瓦 (Bossa Nova)、后摇与极简氛围黑胶唱片。

---

## 📬 联系方式与密码学身份验证

欢迎针对开放去中心化协议、韧性网络设计进行深入的技术交流与异步沟通。

- **电子邮箱**: `mateo [at] silva-systems [dot] dev`
- **Matrix**: `@mateo:matrix.org`
- **Mastodon**: `@mateo@hachyderm.io`
- **PGP 指纹**: `8A4E 71F2 39D0 C56B E114  0953 2F87 63AC 9D41 B822`

```text
-----BEGIN PGP PUBLIC KEY BLOCK-----
Comment: Mateo Silva (Personal Key - Valid through 2029)

mQGNBGXR7yYBDADK1F5N8K72YvA3k9sP2hGj...[Verified OpenPGP Key]...
=4kL9
-----END PGP PUBLIC KEY BLOCK-----
```
