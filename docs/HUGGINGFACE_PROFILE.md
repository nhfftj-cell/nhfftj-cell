# Hugging Face Profile Configuration & Bio for Mateo Silva

## 1. Hugging Face Account Settings (Settings -> Profile)

```text
Full Name:           Mateo Silva
GitHub Username:     nhfftj-cell
Homepage / Website:  https://github.com/nhfftj-cell
Interests:           Edge-Computing, Local-First, Quantization, Efficient-Inference, P2P-Sync
Bio:
Staff infrastructure engineer working on edge computing, ultra-compact embedding models, and offline-first local intelligence. Researching delta model weight sync over constrained peer-to-peer networks.
```

---

## 2. Hugging Face Profile Bio & Research Statement (Profile Overview)

```markdown
# Mateo Silva

Staff Infrastructure Engineer · Distributed Systems & Edge Inference  
Based in Lisbon, Portugal (UTC+0 / WET) · [GitHub (@nhfftj-cell)](https://github.com/nhfftj-cell)

---

## 🧭 Direction & Research Focus

My work on Hugging Face revolves around making machine learning practical in zero-cloud, high-latency, and bandwidth-constrained environments. I don't build massive cloud clusters; I focus on extreme compression, local-first embedding generation, and decentralized model distribution.

### Core Explorations
1. **Low-Power Edge Embeddings**: Optimizing sub-50MB dense semantic representation models capable of running entirely in WebAssembly and on low-spec ARM SBCs without GPU acceleration.
2. **P2P Model Weight Distribution**: Chunked, Merkle-verified delta replication protocols for quant models (GGUF / AWQ), enabling mesh nodes to distribute model updates over intermittent local networks.
3. **Local Vector Search Primitives**: Developing tiny, zero-dependency embedding index formats tailored for embedded SQLite instances and local-first CRDT stores.

---

## 📦 Artifacts & Repositories

| Type | Repository / Target | Focus | Primary Architecture |
| :--- | :--- | :--- | :--- |
| **Model** | `micro-embed-multilingual-quant` | 4-bit quantized multilingual text representation model (<38MB) for edge search. | GGUF / ONNX / Wasm |
| **Dataset** | `intermittent-network-telemetry` | Time-series packet loss & latency traces from low-power LoRa mesh field tests. | Parquet / Arrow |
| **Space** | `edge-similarity-sandbox` | Zero-backend in-browser semantic similarity demo running pure client-side WebAssembly. | Svelte / Wasm / WebGPU |
| **Model** | `lora-delta-adapter-dist` | Parameter-efficient task adapters formatted for P2P chunked bitstream streaming. | SafeTensors / Merkle Chunked |

---

## 💻 Tech Stack in ML & Inference Systems

- **Runtimes & Compilation**: `candle` (minimalist Rust ML framework), ONNX Runtime, `llama.cpp` (GGUF tooling), WebAssembly
- **Formats & Primitives**: SafeTensors, Arrow / Parquet, FlatBuffers, Quantization (INT4 / INT8 / AWQ)
- **Host Systems**: Linux (Arch / Alpine), RISC-V SBCs, Raspberry Pi CM4, Apple Silicon (Metal)

---

## 📬 Contact & Collaboration

Interested in local-first AI, edge inference without corporate cloud dependencies, or P2P data synchronization? Feel free to connect:

- **GitHub**: [github.com/nhfftj-cell](https://github.com/nhfftj-cell)
- **Matrix**: `@mateo:matrix.org`
- **Email**: `mateo [at] silva-systems [dot] dev`
```
