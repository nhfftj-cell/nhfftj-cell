| [KR 한국어](./ko.md) | [US English](../../README.md) | [JP 日本語](./ja.md) | [CN 简体中文](./zh-CN.md) | [ES Español](./es.md) |
| :---: | :---: | :---: | :---: | :---: |
| [FR Français](./fr.md) | [DE Deutsch](./de.md) | [RU Русский](./ru.md) | [BR Português](./pt-BR.md) | [SA العربية](./ar.md) |

---

# 마테오 실바 (Mateo Silva)

```text
위치:        포르투갈 리스본 (UTC+0 / WET)
전문 분야:   분산 시스템, 로컬 우선 아키텍처, P2P 통신 프로토콜
엔지니어링 철학: 중앙 서버보다 오래 지속되는 회복탄력적 소프트웨어
현재 업무:   Distributed Storage Labs 수석 인프라 엔지니어
현재 활동:   오픈 프로토콜 메인터넌스 및 저전력 메시 무선 통신 연구
```

안녕하세요, 마테오입니다. 저는 불안정한 네트워크 환경, 빈번한 연결 끊김, 통신망이 전무한 오프라인 상황에서도 견고하게 동작하는 소프트웨어를 설계하고 개발합니다. 주로 CRDT(무충돌 복제 데이터 타입), 극도로 제한된 대역폭 환경에서의 상태 동기화 알고리즘, 그리고 Rust와 Go 기반의 경량 임베디드 네트워크 데몬 구현에 집중하고 있습니다.

터미널에서 메모리 할당을 프로파일링하거나 TCP 혼잡 제어 파라미터를 튜닝하지 않을 때는 카파리카 해변(Costa da Caparica)에서 대서양 파도를 타거나, 직접 에스프레소 원두를 로스팅하고, 암실에서 35mm 흑백 필름을 현상하곤 합니다.

---

## 🔭 현재 관심사 및 연구 주제

- **로컬 우선(Local-First) 동기화**: 단일 진실 공급원(Single Source of Truth) 없이도 결정론적 충돌 해결을 보장하는 단조 증가 추가 전용(Append-only) 로그 상태 조정 알고리즘 연구.
- **초저대역폭 P2P 프로토콜**: LoRa 무선 장비 및 BLE 환경에서 극도로 압축된 직렬화 포맷과 델타 상태 복제 파이프라인 구현.
- **커널 레벨 네트워크 관측성**: 고대역폭 패킷 라우팅 파이프라인 전반에서 발생하는 테일 레이턴시(Tail Latency) 스파이크를 추적하기 위한 eBPF 프로브 개발.
- **오프라인 협업 스토리지 엔진**: SQLite B-Tree 내부에서 벡터 시계(Vector Clock)를 네이티브 수준으로 추적하는 C 기반 확장 가상 테이블 모듈 설계.

---

## 🛠️ 주요 오픈소스 프로젝트

| 프로젝트 | 구현 언어 | 역할 / 상태 | 상세 설명 |
| :--- | :--- | :--- | :--- |
| **`merkle-stream`** | Rust | 제작자 & 메인테이너 | 간헐적 무선 통신망을 위해 설계된 고성능 비동기 머클 트리(Merkle-tree) 상태 조정 라이브러리. |
| **`driftwood-kv`** | Go / WASM | 핵심 개발자 | 상태 기반 CRDT 프리미티브를 내장하고 클라우드 원격 측정(Telemetry)이 전혀 없는 로컬 우선 임베디드 KV 스토리지. |
| **`beacon-mesh`** | C99 / Rust | 메인테이너 | 저전력 LoRa 트랜시버를 활용해 재난 및 통신 두절 지역에서 탈중앙 패킷을 중계하는 경량 라우팅 데몬. |
| **`polaroid-cli`** | Zig | 개인 프로젝트 | 아날로그 카메라 네거티브 필름 스캔 데이터를 보정하고 색조 노출 곡선을 정밀 계산하는 고속 터미널 도구. |
| **`sqlite-vclock`** | C / SQLite | 제작자 | 다중 마스터 동시 브랜치 상태 추적을 지원하는 플러그형 SQLite 가상 테이블 확장 모듈. |

---

## 💻 기술 스택 및 아키텍처

### 프로그래밍 언어 & 런타임 시스템
- **주력 프로덕션**: Rust (tokio, serde, async-std), Go (동시성 런타임, netpoll, 채널 아키텍처)
- **저수준 & 임베디드**: C99, Zig, ARM Cortex-M 어셈블리
- **웹 & 인터페이스 계층**: 모던 TypeScript, Svelte, WebAssembly (Wasm-bindgen)
- **스크립팅 & 도구**: POSIX Shell, Python (데이터 모델링 및 수치 시뮬레이션), Lua

### 분산 시스템 & 스토리지 엔진
- **프로토콜 엔지니어링**: libp2p, gRPC, Protobuf, QUIC, TCP/IP 커널 튜닝, WireGuard
- **상태 복제 모델**: 상태 기반(State-based) & 연산 기반(Operation-based) CRDT, Merkle DAG, Vector Clock, Raft 합의 알고리즘
- **임베디드 스토리지**: RocksDB, LMDB, SQLite (Virtual Tables, WAL 모드), PostgreSQL

### 시스템 진단 & 인프라
- **운영체제**: Linux (Debian, Arch Linux, Alpine), FreeBSD
- **진단 및 프로파일링**: eBPF (`bpftrace`, `bcc`), `perf`, `strace`, Wireshark, Valgrind
- **컨테이너 및 배포**: Docker (멀티스테이지 및 scratch 빌드), Nix / NixOS, QEMU / KVM

---

## ⚙️ 데일리 하드웨어 & 워크스테이션 환경

```text
시스템 하드웨어:
├── 메인 워크스테이션: AMD Ryzen 9 7950X, 64GB DDR5 ECC 메모리, Fedora Silverblue
├── 랩톱:            ThinkPad T14s Gen 4 (AMD), Arch Linux (커널 하드닝 적용)
├── 터미널 에뮬레이터: Alacritty + tmux
├── 에디터:          Neovim (순수 Lua 기반 미니멀 경량 설정)
├── 셸 환경:         zsh + pure 프롬프트
└── 키보드:          Corne 36키 분할형 기계식 키보드 (Colemak-DH 자판 배열)
```

---

## ☕ 터미널 밖의 삶

- **아날로그 필름 사진**: 1957년식 기계식 라이카 M3(Leica M3)와 핫셀블라드 500 C/M을 주로 사용합니다. 코닥 Tri-X 400과 일포드 HP5+ 필름을 D-76 약품으로 직접 암실 현상합니다.
- **수동 에스프레소**: 라 파보니(La Pavoni Europiccola) 레버 머신을 사용해 가변 압력으로 에스프레소를 추출합니다. 에티오피아 예가체프 워시드와 콜롬비아 우일라 싱글 오리진을 즐깁니다.
- **대서양 서핑**: 대서양 너울이 들어오는 날이면 이른 아침 카르카벨루스(Carcavelos), 긴슈(Guincho), 수퍼투보스(Supertubos) 해변에서 서핑을 합니다.
- **빈티지 오디오 복원**: 1970년대 마란츠(Marantz) 리시버 앰프를 복원하며, 보사노바, 포스트록, 앰비언트 바이닐 LP 컬렉션을 즐겨 듣습니다.

---

## 📬 연락처 및 암호학적 신원 검증

개방적이고 회복탄력성 있는 오픈 프로토콜 및 비동기 기술 토론을 환영합니다.

- **이메일**: `mateo [at] silva-systems [dot] dev`
- **Matrix**: `@mateo:matrix.org`
- **Mastodon**: `@mateo@hachyderm.io`
- **PGP 핑거프린트**: `8A4E 71F2 39D0 C56B E114  0953 2F87 63AC 9D41 B822`

```text
-----BEGIN PGP PUBLIC KEY BLOCK-----
Comment: Mateo Silva (Personal Key - Valid through 2029)

mQGNBGXR7yYBDADK1F5N8K72YvA3k9sP2hGj...[Verified OpenPGP Key]...
=4kL9
-----END PGP PUBLIC KEY BLOCK-----
```
