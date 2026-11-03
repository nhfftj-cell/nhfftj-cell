| [KR 한국어](./ko.md) | [US English](../../README.md) | [JP 日本語](./ja.md) | [CN 简体中文](./zh-CN.md) | [ES Español](./es.md) |
| :---: | :---: | :---: | :---: | :---: |
| [FR Français](./fr.md) | [DE Deutsch](./de.md) | [RU Русский](./ru.md) | [BR Português](./pt-BR.md) | [SA العربية](./ar.md) |

---

# Mateo Silva

```text
Localisation: Lisbonne, Portugal (UTC+0 / WET)
Domaines:     Systèmes Distribués, Architecture Local-First, Protocoles P2P
Philosophie:  Des logiciels résilients qui survivent à leurs serveurs centraux
Poste:        Staff Infrastructure Engineer chez Distributed Storage Labs
Statut:       Maintenance de protocoles ouverts et recherche sur radios maillées basse consommation
```

Bonjour, je m'appelle Mateo. Je conçois des logiciels bâtis pour fonctionner dans des conditions réseau hostiles, sur des liens instables et en environnement totalement déconnecté. La majeure partie de mes travaux est consacrée aux types de données répliquées sans conflit (CRDT), à la synchronisation d'état sur bande passante contrainte, et à l'implémentation de démons réseau embarqués en Rust et en Go.

Lorsque je ne suis pas en train de profiler des allocations mémoire ou d'ajuster des paramètres de congestion TCP, vous me trouverez généralement à surfer sur les vagues de Costa da Caparica, à torréfier du café de spécialité d'origine pure, ou à développer des pellicules argentiques noir et blanc 35 mm dans ma chambre noire.

---

## 🔭 Recherches et Projets Actuels

- **Synchronisation Local-First** : Perfectionnement d'algorithmes de réconciliation de journaux en ajout seul (append-only) avec résolution déterministe des conflits, sans nécessiter de source de vérité unique.
- **Réseaux P2P à Bande Passante Restreinte** : Exploration de formats de sérialisation ultra-compacts et de réplication d'état différentiel sur liaisons radio LoRa et Bluetooth LE.
- **Observabilité Réseau au Niveau Noyau** : Écriture de sondes de traçage eBPF pour isoler les pics de latence de queue (tail latency) sur des pipelines de routage de paquets à très haut débit.
- **Stockage Collaboratif Hors-Ligne** : Conception d'extensions de tables virtuelles en C pour SQLite permettant de suivre nativement les horloges vectorielles au sein même des arbres B-tree.

---

## 🛠️ Projets Open Source Phares

| Projet | Langage | Rôle / Statut | Description |
| :--- | :--- | :--- | :--- |
| **`merkle-stream`** | Rust | Créateur & Mainteneur | Bibliothèque asynchrone haute performance de réconciliation d'état par arbres de Merkle pour réseaux sans fil intermittents. |
| **`driftwood-kv`** | Go / WASM | Auteur Principal | Magasin clé-valeur embarqué local-first avec primitives CRDT d'état intégrées et zéro télémétrie cloud. |
| **`beacon-mesh`** | C99 / Rust | Mainteneur | Démon de routage léger pour le relais décentralisé de paquets hors-réseau sur émetteurs-récepteurs LoRa basse consommation. |
| **`polaroid-cli`** | Zig | Projet Personnel | Utilitaire en ligne de commande ultra-rapide calculant les courbes d'exposition argentique et convertissant les scans RAW de négatifs. |
| **`sqlite-vclock`** | C / SQLite | Auteur | Extension de table virtuelle pour SQLite offrant un suivi concurrentiel de branches multi-maîtres. |

---

## 💻 Boîte à Outils Technique

### Langages de Programmation & Runtimes
- **Production Principale** : Rust (tokio, serde, async-std), Go (concurrence, netpoll, mécanismes internes du runtime)
- **Bas Niveau & Embarqué** : C99, Zig, Assembleur ARM Cortex-M
- **Couche Web & Interface** : TypeScript moderne, Svelte, WebAssembly (Wasm-bindgen)
- **Scripting & Outils Système** : POSIX Shell, Python (modélisation de données & calcul numérique), Lua

### Systèmes Distribués & Stockage
- **Ingénierie de Protocoles** : libp2p, gRPC, Protobuf, QUIC, optimisation de pile TCP/IP, WireGuard
- **Modèles de Réplication** : CRDT basés sur l'état et sur les opérations, DAG de Merkle, Horloges Vectorielles, consensus Raft
- **Moteurs de Données** : RocksDB, LMDB, SQLite (tables virtuelles, mode WAL), PostgreSQL

### Ingénierie Système & Infrastructure
- **Systèmes d'Exploitation** : Linux (Debian, Arch Linux, Alpine), FreeBSD
- **Outils d'Analyse & Diagnostic** : eBPF (`bpftrace`, `bcc`), `perf`, `strace`, Wireshark, Valgrind
- **Conteneurs & Déploiement** : Docker (multi-étapes et scratch), Nix / NixOS, QEMU / KVM

---

## ⚙️ Environnement Quotidien

```text
Configuration Matérielle :
├── Station de Travail : AMD Ryzen 9 7950X, 64 Go DDR5 ECC, Fedora Silverblue
├── PC Portable :        ThinkPad T14s Gen 4 (AMD), Arch Linux (noyau durci)
├── Émulateur Terminal : Alacritty + tmux
├── Éditeur de Code :    Neovim (configuration Lua minimaliste, zéro surcharge)
├── Shell :              zsh + invite pure
└── Clavier :            Corne 36 touches mécanique ergonomique scindé (disposition Colemak-DH)
```

---

## ☕ Au-Delà du Terminal

- **Photographie Argentique** : Travaille principalement avec un boîtier mécanique Leica M3 de 1957 et un Hasselblad 500 C/M moyen format. Développement manuel des films Kodak Tri-X 400 et Ilford HP5+ avec le révélateur D-76.
- **Art de l'Espresso** : Extraction manuelle sur levier avec une La Pavoni Europiccola. Terroirs de prédilection : Éthiopie Yirgacheffe lavé et Colombie Huila.
- **Surf Océanique** : Sessions à l'aube sur les spots de Carcavelos, Guincho et Supertubos dès que les houles atlantiques se lèvent.
- **Restauration Audio Vintage** : Remise en état d'amplificateurs stéréo Marantz des années 1970 et collection de vinyles de Bossa Nova, Post-Rock et musique ambiante minimaliste.

---

## 📬 Contact & Vérification Cryptographique

J'apprécie les échanges constructifs, les débats techniques asynchrones et les collaborations autour de protocoles ouverts et résilients.

- **Courriel** : `mateo [at] silva-systems [dot] dev`
- **Matrix** : `@mateo:matrix.org`
- **Mastodon** : `@mateo@hachyderm.io`
- **Empreinte PGP** : `8A4E 71F2 39D0 C56B E114  0953 2F87 63AC 9D41 B822`

```text
-----BEGIN PGP PUBLIC KEY BLOCK-----
Comment: Mateo Silva (Personal Key - Valid through 2029)

mQGNBGXR7yYBDADK1F5N8K72YvA3k9sP2hGj...[Verified OpenPGP Key]...
=4kL9
-----END PGP PUBLIC KEY BLOCK-----
```
