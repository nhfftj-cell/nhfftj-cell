| [KR 한국어](./ko.md) | [US English](../../README.md) | [JP 日本語](./ja.md) | [CN 简体中文](./zh-CN.md) | [ES Español](./es.md) |
| :---: | :---: | :---: | :---: | :---: |
| [FR Français](./fr.md) | [DE Deutsch](./de.md) | [RU Русский](./ru.md) | [BR Português](./pt-BR.md) | [SA العربية](./ar.md) |

---

# Mateo Silva

```text
Localização: Lisboa, Portugal (UTC+0 / WET)
Foco:        Sistemas Distribuídos, Arquitetura Local-First, Protocolos P2P
Filosofia:   Sistemas resilientes que sobrevivem aos seus servidores centrais
Atuação:     Staff Infrastructure Engineer na Distributed Storage Labs
Status:      Mantendo protocolos abertos e desenvolvendo malhas de rádio de baixo consumo
```

Olá, eu sou o Mateo. Desenvolvo software projetado para funcionar sob condições de rede adversas, enlaces instáveis e ambientes totalmente desconectados. A maior parte do meu trabalho concentra-se em Tipos de Dados Replicados Sem Conflito (CRDTs), sincronização de estado sobre larguras de banda extremamente limitadas e daemons de rede embarcados em Rust e Go.

Quando não estou analisando alocações de memória no terminal ou ajustando algoritmos de controle de congestão TCP, você geralmente me encontrará surfando na Costa da Caparica, torrando grãos de café especial de origem única ou revelando filmes fotográficos 35mm em preto e branco no meu laboratório escuro.

---

## 🔭 Foco Atual e Pesquisa Ativa

- **Sincronização Local-First**: Aperfeiçoamento de algoritmos de reconciliação de logs somente-anexação (append-only) com resolução determinística de conflitos, sem depender de uma única fonte da verdade.
- **P2P em Largura de Banda Restrita**: Exploração de formatos ultracompactos de serialização e replicação de estado delta sobre enlaces de rádio LoRa e Bluetooth LE.
- **Observabilidade de Rede no Kernel**: Desenvolvimento de sondas eBPF para rastrear picos de latência de cauda (tail latency) em pipelines de roteamento de pacotes de alto rendimento.
- **Armazenamento Colaborativo Offline**: Criação de extensões de tabelas virtuais em C para SQLite capazes de rastrear relógios vetoriais (Vector Clocks) de forma nativa nas árvores B-tree.

---

## 🛠️ Projetos Open Source em Destaque

| Projeto | Linguagem | Função / Status | Descrição |
| :--- | :--- | :--- | :--- |
| **`merkle-stream`** | Rust | Criador & Mantenedor | Biblioteca assíncrona de reconciliação de estado baseada em árvores de Merkle de alto desempenho para redes sem fio intermitentes. |
| **`driftwood-kv`** | Go / WASM | Autor Principal | Armazenamento chave-valor embarcado local-first com primitivas CRDT de estado integradas e zero telemetria em nuvem. |
| **`beacon-mesh`** | C99 / Rust | Mantenedor | Daemon leve de roteamento para retransmissão descentralizada de pacotes fora da rede em transceptores LoRa de baixo consumo. |
| **`polaroid-cli`** | Zig | Projeto Pessoal | Utilitário rápido de terminal para cálculo de curvas de exposição fotográfica e conversão de negativos digitalizados em RAW. |
| **`sqlite-vclock`** | C / SQLite | Autor | Extensão de tabela virtual para SQLite que permite o rastreamento concorrente de ramificações multi-mestre. |

---

## 💻 Arsenal Técnico

### Linguagens de Programação & Runtimes
- **Produção Principal**: Rust (tokio, serde, async-std), Go (concorrência, netpoll, componentes internos do runtime)
- **Baixo Nível & Embarcados**: C99, Zig, Assembly ARM Cortex-M
- **Camada Web & Interface**: TypeScript moderno, Svelte, WebAssembly (Wasm-bindgen)
- **Scripting & Automação**: POSIX Shell, Python (modelagem de dados e simulações numéricas), Lua

### Sistemas Distribuídos & Armazenamento
- **Engenharia de Protocolos**: libp2p, gRPC, Protobuf, QUIC, ajustes de pilha TCP/IP, WireGuard
- **Modelos de Replicação**: CRDTs baseados em estado e operações, Merkle DAGs, Relógios Vetoriais, consenso Raft
- **Mecanismos de Dados**: RocksDB, LMDB, SQLite (tabelas virtuais, modo WAL), PostgreSQL

### Engenharia de Sistemas & Infraestrutura
- **Sistemas Operacionais**: Linux (Debian, Arch Linux, Alpine), FreeBSD
- **Diagnóstico & Observabilidade**: eBPF (`bpftrace`, `bcc`), `perf`, `strace`, Wireshark, Valgrind
- **Contêineres & Implantação**: Docker (construções multi-stage e scratch), Nix / NixOS, QEMU / KVM

---

## ⚙️ Ambiente de Trabalho Diário

```text
Configuração de Hardware:
├── Estação Principal: AMD Ryzen 9 7950X, 64GB DDR5 ECC, Fedora Silverblue
├── Portátil:           ThinkPad T14s Gen 4 (AMD), Arch Linux (kernel reforçado)
├── Terminal:           Alacritty + tmux
├── Editor:             Neovim (configuração limpa em Lua, zero supérfluo)
├── Shell:              zsh + prompt pure
└── Teclado:            Corne mecânico dividido de 36 teclas (leiaute Colemak-DH)
```

---

## ☕ Além do Terminal

- **Fotografia Analógica**: Trabalho principalmente com uma Leica M3 mecânica de 1957 e uma Hasselblad 500 C/M de médio formato. Revelação manual de filmes Kodak Tri-X 400 e Ilford HP5+ com química D-76.
- **Café Especial**: Extração por alavanca manual em uma La Pavoni Europiccola. Origens favoritas: Etiópia Yirgacheffe lavado e Colômbia Huila.
- **Surf no Atlântico**: Sessões matinais em Carcavelos, Guincho e Supertubos sempre que as ondulações do Atlântico chegam à costa.
- **Restauração de Áudio Vintage**: Recuperação de amplificadores estéreo Marantz dos anos 70 e garimpo de discos de vinil de Bossa Nova, Post-Rock e música ambiente minimalista.

---

## 📬 Contato e Verificação Criptográfica

Valorizo trocas substanciais, debates técnicos assíncronos e colaborações em protocolos abertos e resilientes.

- **E-mail**: `mateo [at] silva-systems [dot] dev`
- **Matrix**: `@mateo:matrix.org`
- **Mastodon**: `@mateo@hachyderm.io`
- **Impressão Digital PGP**: `8A4E 71F2 39D0 C56B E114  0953 2F87 63AC 9D41 B822`

```text
-----BEGIN PGP PUBLIC KEY BLOCK-----
Comment: Mateo Silva (Personal Key - Valid through 2029)

mQGNBGXR7yYBDADK1F5N8K72YvA3k9sP2hGj...[Verified OpenPGP Key]...
=4kL9
-----END PGP PUBLIC KEY BLOCK-----
```
