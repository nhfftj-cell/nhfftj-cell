| [KR 한국어](./ko.md) | [US English](../../README.md) | [JP 日本語](./ja.md) | [CN 简体中文](./zh-CN.md) | [ES Español](./es.md) |
| :---: | :---: | :---: | :---: | :---: |
| [FR Français](./fr.md) | [DE Deutsch](./de.md) | [RU Русский](./ru.md) | [BR Português](./pt-BR.md) | [SA العربية](./ar.md) |

---

# Mateo Silva

```text
Ubicación:   Lisboa, Portugal (UTC+0 / WET)
Especialidad: Sistemas Distribuidos, Arquitectura Local-First, Protocolos P2P
Filosofía:   Software resiliente que perdura más allá de los servidores centrales
Cargo:       Staff Infrastructure Engineer en Distributed Storage Labs
Actividad:   Mantenimiento de protocolos abiertos e investigación de mallas de radio de baja potencia
```

Hola, soy Mateo. Construyo software diseñado para operar en condiciones de red hostiles, enlaces intermitentes y entornos completamente fuera de línea. La mayor parte de mi trabajo se centra en Tipos de Datos Replicados Libres de Conflicto (CRDT), sincronización de estado sobre anchos de banda extremadamente reducidos y demonios de red embebidos escritos en Rust y Go.

Cuando no estoy analizando asignaciones de memoria en terminal o ajustando algoritmos de congestión TCP, suelo estar cabalgando olas en la Costa da Caparica, tostando café de especialidad de origen único o revelando película analógica de 35 mm en blanco y negro en mi cuarto oscuro.

---

## 🔭 Foco Actual e Investigación Activa

- **Sincronización Local-First**: Perfeccionamiento de algoritmos de reconciliación de registros sólo-adición (append-only) con resolución determinista de conflictos sin requerir una única fuente de verdad.
- **P2P en Ancho de Banda Restringido**: Exploración de formatos de serialización ultracompactos y replicación de estado diferencial sobre radios LoRa y Bluetooth LE.
- **Observabilidad de Red a Nivel de Kernel**: Desarrollo de sondas eBPF para rastrear picos de latencia en cola (tail latency) en tuberías de enrutamiento de paquetes de alto rendimiento.
- **Almacenamiento Colaborativo Desconectado**: Creación de extensiones virtuales en C para SQLite que rastrean relojes vectoriales de forma nativa en las estructuras B-tree.

---

## 🛠️ Proyectos Open Source Destacados

| Proyecto | Lenguaje | Rol / Estado | Descripción |
| :--- | :--- | :--- | :--- |
| **`merkle-stream`** | Rust | Creador & Mantenedor | Biblioteca asíncrona de reconciliación de estado basada en árboles de Merkle de alto rendimiento para redes inalámbricas intermitentes. |
| **`driftwood-kv`** | Go / WASM | Autor Principal | Almacén clave-valor embebido local-first con primitivas CRDT de estado integradas y cero telemetría en la nube. |
| **`beacon-mesh`** | C99 / Rust | Mantenedor | Demonio de enrutamiento ligero para retransmisión de paquetes descentralizados en transceptores LoRa de bajo consumo. |
| **`polaroid-cli`** | Zig | Proyecto Personal | Utilidad rápida de terminal que calcula curvas de exposición tonal y convierte escaneos de negativos RAW. |
| **`sqlite-vclock`** | C / SQLite | Autor | Extensión de tabla virtual para SQLite que habilita el seguimiento concurrente de ramas multi-maestro. |

---

## 💻 Arsenal Técnico y Herramientas

### Lenguajes y Tiempos de Ejecución
- **Producción Principal**: Rust (tokio, serde, async-std), Go (concurrencia, netpoll, aspectos internos del runtime)
- **Bajo Nivel y Embebido**: C99, Zig, Ensamblador ARM Cortex-M
- **Capa Web e Interfaz**: TypeScript moderno, Svelte, WebAssembly (Wasm-bindgen)
- **Scripting y Utilidades**: POSIX Shell, Python (modelado y simulación numérica), Lua

### Sistemas Distribuidos y Almacenamiento
- **Ingeniería de Protocolos**: libp2p, gRPC, Protobuf, QUIC, optimización de pila TCP/IP, WireGuard
- **Replicación y Estado**: CRDT basados en estado y operaciones, DAGs de Merkle, Relojes Vectoriales, consenso Raft
- **Motores de Almacenamiento**: RocksDB, LMDB, SQLite (tablas virtuales, modo WAL), PostgreSQL

### Ingeniería de Sistemas e Infraestructura
- **Sistemas Operativos**: Linux (Debian, Arch Linux, Alpine), FreeBSD
- **Diagnóstico y Rendimiento**: eBPF (`bpftrace`, `bcc`), `perf`, `strace`, Wireshark, Valgrind
- **Contenedores y Despliegue**: Docker (multi-stage y scratch), Nix / NixOS, QEMU / KVM

---

## ⚙️ Entorno de Trabajo Diario

```text
Configuración de Hardware:
├── Estación de Trabajo: AMD Ryzen 9 7950X, 64GB DDR5 ECC, Fedora Silverblue
├── Portátil:            ThinkPad T14s Gen 4 (AMD), Arch Linux (kernel reforzado)
├── Terminal:            Alacritty + tmux
├── Editor:              Neovim (configuración limpia en Lua, sin bloatware)
├── Shell:               zsh + prompt pure
└── Teclado:             Corne mecánico dividido de 36 teclas (disposición Colemak-DH)
```

---

## ☕ Más Allá de la Terminal

- **Fotografía Analógica**: Trabajo principalmente con una Leica M3 mecánica de 1957 y una Hasselblad 500 C/M de formato medio. Revelado manual de películas Kodak Tri-X 400 e Ilford HP5+ con química D-76.
- **Café de Especialidad**: Extracción con palanca manual en una La Pavoni Europiccola. Variedades predilectas: Etiopía Yirgacheffe lavado y Colombia Huila.
- **Surf en el Atlántico**: Sesiones al amanecer en Carcavelos, Guincho y Supertubos cuando entran las marejadas del Atlántico.
- **Restauración de Audio Vintage**: Mantenimiento de amplificadores estéreo Marantz de los años 70 y colección selecta de vinilos de Bossa Nova, Post-Rock y Ambient minimalista.

---

## 📬 Contacto y Verificación Criptográfica

Aprecio la correspondencia constructiva, el debate técnico asíncrono y las colaboraciones en protocolos abiertos y resistentes.

- **Correo**: `mateo [at] silva-systems [dot] dev`
- **Matrix**: `@mateo:matrix.org`
- **Mastodon**: `@mateo@hachyderm.io`
- **Huella PGP**: `8A4E 71F2 39D0 C56B E114  0953 2F87 63AC 9D41 B822`

```text
-----BEGIN PGP PUBLIC KEY BLOCK-----
Comment: Mateo Silva (Personal Key - Valid through 2029)

mQGNBGXR7yYBDADK1F5N8K72YvA3k9sP2hGj...[Verified OpenPGP Key]...
=4kL9
-----END PGP PUBLIC KEY BLOCK-----
```
