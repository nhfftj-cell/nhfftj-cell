| [KR 한국어](./ko.md) | [US English](../../README.md) | [JP 日本語](./ja.md) | [CN 简体中文](./zh-CN.md) | [ES Español](./es.md) |
| :---: | :---: | :---: | :---: | :---: |
| [FR Français](./fr.md) | [DE Deutsch](./de.md) | [RU Русский](./ru.md) | [BR Português](./pt-BR.md) | [SA العربية](./ar.md) |

---

# Mateo Silva

```text
Standort:      Lissabon, Portugal (UTC+0 / WET)
Schwerpunkte:  Verteilte Systeme, Local-First-Architektur, P2P-Protokolle
Philosophie:   Resiliente Systeme, die ihre zentralen Server überdauern
Position:      Staff Infrastructure Engineer bei Distributed Storage Labs
Status:        Wartung offener Protokolle & Experimente mit stromsparendem Mesh-Funk
```

Hallo, ich bin Mateo. Ich entwickle Software, die unter widrigen Netzwerkbedingungen, bei instabilen Verbindungen und in komplett netzfernen Umgebungen zuverlässig funktioniert. Der Großteil meiner Arbeit konzentriert sich auf konfliktfreie replizierte Datentypen (CRDTs), Zustandssynchronisation über stark bandbreitenbeschränkte Kanäle und eingebettete Netzwerk-Dämonen in Rust und Go.

Wenn ich nicht gerade Speicherallokationen im Terminal analysiere oder TCP-Staukontrollparameter optimiere, findet man mich meistens beim Wellenreiten an der Costa da Caparica, beim Rösten von sortenreinem Espresso oder beim Entwickeln von 35-mm-Schwarzweißfilmen in meiner Dunkelkammer.

---

## 🔭 Aktuelle Schwerpunkte & Forschung

- **Local-First-Synchronisation**: Verfeinerung von Abgleichsalgorithmen für reine Anfügeprotokolle (Append-only Logs) mit deterministischer Konfliktlösung ohne zentrale Datenquelle.
- **Bandbreitenbeschränkte P2P-Netze**: Erforschung hochkompakter Serialisierungsformate und Delta-Zustandsreplikation über LoRa-Funk und Bluetooth LE.
- **Netzwerk-Observability auf Kernel-Ebene**: Entwicklung von eBPF-Tracesonden zur Lokalisierung von Latenzspitzen (Tail Latency) in hochdurchsatzfähigen Paketweiterleitungspipelines.
- **Offline-fähige kooperative Speicherung**: Implementierung von C-basierten virtuellen Tabellenerweiterungen für SQLite zur nativen Erfassung von Vektoruhren (Vector Clocks) direkt in den B-Tree-Strukturen.

---

## 🛠️ Ausgewählte Open-Source-Projekte

| Projekt | Sprache | Rolle / Status | Beschreibung |
| :--- | :--- | :--- | :--- |
| **`merkle-stream`** | Rust | Urheber & Maintainer | Hochperformante asynchrone Merkle-Tree-Zustandsabgleichsbibliothek für instabile drahtlose Funknetzwerke. |
| **`driftwood-kv`** | Go / WASM | Hauptautor | Eingebetteter, lokaler Key-Value-Speicher mit integrierten zustandsbasierten CRDT-Primitiven und ohne jegliche Cloud-Telemetrie. |
| **`beacon-mesh`** | C99 / Rust | Maintainer | Leichtgewichtiger Routing-Dämon zur dezentralen Paketweiterleitung im autarken Einsatz auf stromsparenden LoRa-Transceivern. |
| **`polaroid-cli`** | Zig | Hobby-Projekt | Extrem schnelles Terminal-Werkzeug zur Berechnung analoger Filmbelichtungskurven und Konvertierung von RAW-Negativscans. |
| **`sqlite-vclock`** | C / SQLite | Autor | Modulare SQLite-Erweiterung für virtuelle Tabellen zur simultanen Multi-Master-Zweigverfolgung. |

---

## 💻 Technisches Arsenal & Werkzeuge

### Programmiersprachen & Laufzeitsysteme
- **Primär in Produktion**: Rust (tokio, serde, async-std), Go (Parallelität, netpoll, Laufzeitinterna)
- **Systemnah & Eingebettet**: C99, Zig, ARM Cortex-M Assembler
- **Web- & Schnittstellenschicht**: Modernes TypeScript, Svelte, WebAssembly (Wasm-bindgen)
- **Skripte & Automatisierung**: POSIX Shell, Python (Datenmodellierung & numerische Simulationen), Lua

### Verteilte Systeme & Datenspeicherung
- **Protokollentwicklung**: libp2p, gRPC, Protobuf, QUIC, Kernel-TCP/IP-Tuning, WireGuard
- **Replikationsmodelle**: Zustands- und operationsbasierte CRDTs, Merkle DAGs, Vektoruhren, Raft-Konsens
- **Speicher-Engines**: RocksDB, LMDB, SQLite (virtuelle Tabellen, WAL-Modus), PostgreSQL

### Systemtechnik & Infrastruktur
- **Betriebssysteme**: Linux (Debian, Arch Linux, Alpine), FreeBSD
- **Diagnose & Analyse**: eBPF (`bpftrace`, `bcc`), `perf`, `strace`, Wireshark, Valgrind
- **Container & Bereitstellung**: Docker (Multi-Stage & scratch), Nix / NixOS, QEMU / KVM

---

## ⚙️ Tägliches Arbeitsumfeld

```text
Hardware-Konfiguration:
├── Haupt-Workstation: AMD Ryzen 9 7950X, 64 GB DDR5 ECC, Fedora Silverblue
├── Notebook:          ThinkPad T14s Gen 4 (AMD), Arch Linux (gehärteter Kernel)
├── Terminal:          Alacritty + tmux
├── Editor:            Neovim (schlanke, kompromisslose Lua-Konfiguration)
├── Shell:             zsh + pure Prompt
└── Tastatur:          Corne 36-Tasten Split-Mechanik (Colemak-DH Layout)
```

---

## ☕ Abseits des Terminals

- **Analoge Fotografie**: Fotografiert primär mit einer mechanischen Leica M3 von 1957 und einer Hasselblad 500 C/M im Mittelformat. Eigene Filmentwicklung von Kodak Tri-X 400 und Ilford HP5+ mit D-76-Chemie.
- **Espresso-Kultur**: Manuelle Hebelextraktion auf einer La Pavoni Europiccola. Bevorzugte Röstungen: gewaschener Äthiopien Yirgacheffe und Kolumbien Huila.
- **Atlantik-Surfen**: Frühmorgendliche Sessions in Carcavelos, Guincho und Supertubos, sobald atlantische Dünungen eintreffen.
- **Vintage-Audio-Restauration**: Instandsetzung von Marantz-Stereoreceivern aus den 1970er Jahren und Pflege einer handverlesenen Vinylsammlung aus Bossa Nova, Post-Rock und minimalistischer Ambient-Musik.

---

## 📬 Kontakt & Kryptografische Verifizierung

Ich schätze substanziellen Austausch, asynchrone Fachdiskussionen und die Zusammenarbeit an offenen, widerstandsfähigen Softwareprotokollen.

- **E-Mail**: `mateo [at] silva-systems [dot] dev`
- **Matrix**: `@mateo:matrix.org`
- **Mastodon**: `@mateo@hachyderm.io`
- **PGP-Fingerabdruck**: `8A4E 71F2 39D0 C56B E114  0953 2F87 63AC 9D41 B822`

```text
-----BEGIN PGP PUBLIC KEY BLOCK-----
Comment: Mateo Silva (Personal Key - Valid through 2029)

mQGNBGXR7yYBDADK1F5N8K72YvA3k9sP2hGj...[Verified OpenPGP Key]...
=4kL9
-----END PGP PUBLIC KEY BLOCK-----
```
