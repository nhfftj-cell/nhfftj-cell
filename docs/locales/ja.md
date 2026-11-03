| [KR 한국어](./ko.md) | [US English](../../README.md) | [JP 日本語](./ja.md) | [CN 简体中文](./zh-CN.md) | [ES Español](./es.md) |
| :---: | :---: | :---: | :---: | :---: |
| [FR Français](./fr.md) | [DE Deutsch](./de.md) | [RU Русский](./ru.md) | [BR Português](./pt-BR.md) | [SA العربية](./ar.md) |

---

# マテオ・シルバ (Mateo Silva)

```text
拠点:        ポルトガル・リスボン (UTC+0 / WET)
専門領域:    分散システム、ローカルファーストアーキテクチャ、P2P通信プロトコル
設計哲学:    中央サーバーの寿命を超えて存続する強靭なソフトウェア
現職:        Distributed Storage Labs スタッフインフラエンジニア
活動状況:    オープンプロトコルの保守および低電力メッシュ無線の研究開発
```

こんにちは、マテオです。私は過酷なネットワーク環境、不安定な通信回線、あるいは完全にオフラインの環境下でも確実に動作するソフトウェアを設計・開発しています。主にコンフリクトフリー複製データ型（CRDT）、帯域制限環境における状態同期アルゴリズム、そしてRustやGoを用いた軽量組み込みネットワークデーモンの実装に取り組んでいます。

端末でメモリ割り当てのプロファイリングやTCP輻輳制御アルゴリズムの調整をしていないときは、コスタ・ダ・カパリカ（Costa da Caparica）で波に乗るか、シングルオリジンのエスプレッソ豆を焙煎するか、暗室で35mmモノクロフィルムの現像を行っています。

---

## 🔭 現在の注力分野・研究テーマ

- **ローカルファースト同期**: 単一の信頼できる情報源（Single Source of Truth）を必要とせず、決定論的な競合解決を保証する追加専用（Append-only）ログ照合アルゴリズムの最適化。
- **狭帯域P2P通信**: LoRa無線やBluetooth LE上で動作する超高密度シリアライズ形式と差分状態（Delta-state）複製の研究。
- **カーネル層ネットワーク可観測性**: 高スループットなパケットルーティングパイプラインにおけるテールレイテンシのスパイクを追跡するeBPFトレーシングプローブの開発。
- **オフライン協調ストレージ**: SQLiteのB-Tree内部でベクタークロック（Vector Clocks）をネイティブに追跡するC言語拡張仮想テーブルモジュールの構築。

---

## 🛠️ 主なオープンソースプロジェクト

| プロジェクト | 言語 | 役割 / 状況 | 概要 |
| :--- | :--- | :--- | :--- |
| **`merkle-stream`** | Rust | 開発者 & メンテナ | 断続的な無線ネットワーク向けに設計された高性能非同期マークルツリー（Merkle-tree）状態照合ライブラリ。 |
| **`driftwood-kv`** | Go / WASM | 主著者 | 状態ベースCRDTプリミティブを内蔵し、クラウドテレメトリを一切持たないローカルファースト組み込みKVストア。 |
| **`beacon-mesh`** | C99 / Rust | メンテナ | 低電力LoRaトランシーバーを活用し、オフグリッド環境で分散パケットを中継する軽量ルーティングデーモン。 |
| **`polaroid-cli`** | Zig | ホビー開発 | アナログフィルムの露出曲線を計算し、カメラネガのRAWスキャンを変換・補正する高速ターミナルツール。 |
| **`sqlite-vclock`** | C / SQLite | 著者 | マルチマスターでの並行ブランチ履歴追跡を可能にするプラガブルなSQLite仮想テーブル拡張機能。 |

---

## 💻 技術スタックとツール

### プログラミング言語 & ランタイム
- **メイン実務**: Rust (tokio, serde, async-std), Go (並行処理ランタイム, netpoll, 内部機構)
- **低レイヤ & 組み込み**: C99, Zig, ARM Cortex-M アセンブリ
- **ウェブ & インターフェース**: モダン TypeScript, Svelte, WebAssembly (Wasm-bindgen)
- **スクリプト & ツール**: POSIX Shell, Python (データモデリングおよび数値シミュレーション), Lua

### 分散システム & ストレージ技術
- **プロトコル設計**: libp2p, gRPC, Protobuf, QUIC, TCP/IPカーネル調整, WireGuard
- **複製モデル**: 状態ベース / 操作ベースCRDT, Merkle DAG, Vector Clock, Raftコンセンサス
- **ストレージエンジン**: RocksDB, LMDB, SQLite (仮想テーブル, WALモード), PostgreSQL

### システム診断 & インフラストラクチャ
- **オペレーティングシステム**: Linux (Debian, Arch Linux, Alpine), FreeBSD
- **診断 & プロファイリング**: eBPF (`bpftrace`, `bcc`), `perf`, `strace`, Wireshark, Valgrind
- **コンテナ & デプロイ**: Docker (マルチステージおよびscratchビルド), Nix / NixOS, QEMU / KVM

---

## ⚙️ 開発環境・ハードウェア

```text
システム構成:
├── メインワークステーション: AMD Ryzen 9 7950X, 64GB DDR5 ECC, Fedora Silverblue
├── ノートPC:               ThinkPad T14s Gen 4 (AMD), Arch Linux (強化カーネル)
├── ターミナル:              Alacritty + tmux
├── エディタ:                Neovim (Luaによる無駄のない軽量カスタム構成)
├── シェル:                  zsh + pureプロンプト
└── キーボード:              Corne 36キー 分割型メカニカル (Colemak-DH配列)
```

---

## ☕ 端末の外での暮らし

- **銀塩モノクロ写真**: 主に1957年製ライカM3（Leica M3）とハッセルブラッド500 C/Mを使用。Kodak Tri-X 400およびIlford HP5+をD-76薬品を用いて自宅暗室で手作業現像しています。
- **手動エスプレッソ抽出**: La Pavoni Europiccolaレバーマシンを用いた圧力コントロール抽出。エチオピア・イルガチェフェやコロンビア・ウィラのウォッシュド銘柄を愛飲。
- **大西洋サーフィン**: うねりの入る朝は、カルカヴェロス（Carcavelos）、ギンショ（Guincho）、スペルツボス（Supertubos）の海へ向かいます。
- **ヴィンテージ音響のレストア**: 1970年代のマランツ製アンプを修理・調整し、ボサノヴァ、ポストロック、アンビエントのレコードをコレクションしています。

---

## 📬 連絡先 & 暗号署名検証

オープンで耐障害性に優れた通信プロトコルに関する非同期的な議論やコラボレーションを歓迎します。

- **メール**: `mateo [at] silva-systems [dot] dev`
- **Matrix**: `@mateo:matrix.org`
- **Mastodon**: `@mateo@hachyderm.io`
- **PGPフィンガープリント**: `8A4E 71F2 39D0 C56B E114  0953 2F87 63AC 9D41 B822`

```text
-----BEGIN PGP PUBLIC KEY BLOCK-----
Comment: Mateo Silva (Personal Key - Valid through 2029)

mQGNBGXR7yYBDADK1F5N8K72YvA3k9sP2hGj...[Verified OpenPGP Key]...
=4kL9
-----END PGP PUBLIC KEY BLOCK-----
```
