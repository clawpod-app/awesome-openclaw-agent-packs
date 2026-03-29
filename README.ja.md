[English](./README.md) | [中文](./README.zh-CN.md) | [日本語](./README.ja.md) | [Español](./README.es.md) | [Deutsch](./README.de.md)

# Awesome OpenClaw Agent Packs

**OpenClaw 用の設定済み AI エージェントパック。役割を選んで、Telegram にデプロイして、すぐに使い始めましょう。**

[![ClawPod にデプロイ](https://img.shields.io/badge/デプロイ-ClawPod-FF6B35?style=for-the-badge)](https://clawpod.app/templates)
![パック数](https://img.shields.io/badge/パック-11-blue?style=for-the-badge)
![スキル数](https://img.shields.io/badge/スキル-92-purple?style=for-the-badge)
![ライセンス](https://img.shields.io/badge/ライセンス-MIT-green?style=for-the-badge)

---

## これは何？

各パックは、汎用の OpenClaw エージェントを専門的なチームメンバーに変えます。通話準備、見込み客調査、アウトリーチ作成を行う**セールス・コパイロット**。スタンドアップ、コードレビュー、インシデント対応を行う**エンジニアリング・コパイロット**。契約審査とコンプライアンスチェックを行う**リーガルアナリスト**。

各パックには 6 つの定義ファイル + 完全な `skills/` ディレクトリが含まれます：

```
packs/sales/
├── SOUL.md          # エージェントの人格（性格、価値観、コミュニケーションスタイル）
├── AGENTS.md        # 起動時の動作、利用可能なスキル、ワークフロー
├── HEARTBEAT.md     # 定期タスク（デイリーブリーフィング、週次パイプラインレビュー）
├── TOOLS.md         # 接続ツールと MCP 設定
├── MEMORY.md        # セッション間のコンテキスト記憶方法
├── README.md        # セットアップガイド
└── skills/          # 9 つのスキルワークフロー
    ├── account-research/    → 企業・見込み客の調査
    ├── call-prep/           → コンテキスト付きの通話準備
    ├── draft-outreach/      → パーソナライズされたメール・LinkedIn メッセージ
    ├── pipeline-review/     → 案件の健全性分析とリスク検出
    ├── forecast/            → 加重売上予測
    └── ...                  → + さらに 4 つ
```

---

## 利用可能なパック

| パック | スキル数 | 分野 | デプロイ |
|--------|----------|------|----------|
| [セールス・コパイロット](./packs/sales/) | 9 | 営業・収益 | [![デプロイ](https://img.shields.io/badge/デプロイ-ClawPod-FF6B35)](https://clawpod.app/templates/sales) |
| [エンジニアリング・コパイロット](./packs/engineering/) | 10 | ソフトウェア開発 | [![デプロイ](https://img.shields.io/badge/デプロイ-ClawPod-FF6B35)](https://clawpod.app/templates/engineering) |
| [データアナリスト](./packs/data/) | 10 | データ分析 | [![デプロイ](https://img.shields.io/badge/デプロイ-ClawPod-FF6B35)](https://clawpod.app/templates/data) |
| [マーケティング戦略家](./packs/marketing/) | 8 | マーケティング・コンテンツ | [![デプロイ](https://img.shields.io/badge/デプロイ-ClawPod-FF6B35)](https://clawpod.app/templates/marketing) |
| [リーガルアナリスト](./packs/legal/) | 9 | 法務・コンプライアンス | [![デプロイ](https://img.shields.io/badge/デプロイ-ClawPod-FF6B35)](https://clawpod.app/templates/legal) |
| [ファイナンスアナリスト](./packs/finance/) | 8 | 財務・会計 | [![デプロイ](https://img.shields.io/badge/デプロイ-ClawPod-FF6B35)](https://clawpod.app/templates/finance) |
| [プロダクトマネージャー](./packs/product-management/) | 8 | プロダクト管理 | [![デプロイ](https://img.shields.io/badge/デプロイ-ClawPod-FF6B35)](https://clawpod.app/templates/product-management) |
| [HR パートナー](./packs/human-resources/) | 9 | 人事・採用 | [![デプロイ](https://img.shields.io/badge/デプロイ-ClawPod-FF6B35)](https://clawpod.app/templates/human-resources) |
| [カスタマーサポート](./packs/customer-support/) | 5 | カスタマーサービス | [![デプロイ](https://img.shields.io/badge/デプロイ-ClawPod-FF6B35)](https://clawpod.app/templates/customer-support) |
| [デザインパートナー](./packs/design/) | 7 | UX・デザイン | [![デプロイ](https://img.shields.io/badge/デプロイ-ClawPod-FF6B35)](https://clawpod.app/templates/design) |
| [オペレーションマネージャー](./packs/operations/) | 9 | 事業運営 | [![デプロイ](https://img.shields.io/badge/デプロイ-ClawPod-FF6B35)](https://clawpod.app/templates/operations) |

---

## クイックスタート

### 方法 A：ワンクリックデプロイ（推奨）

1. 上の表からパックを選び、**ClawPod にデプロイ** をクリック
2. Telegram Bot Token を入力
3. 30 秒でエージェントが稼働開始：[clawpod.app](https://clawpod.app)

Docker 不要、VPS 不要、設定ファイル不要。

### 方法 B：セルフホスト（OpenClaw）

```bash
git clone https://github.com/clawpod-app/awesome-openclaw-agent-packs.git
cp -r awesome-openclaw-agent-packs/packs/sales/* ~/.openclaw/workspace/
openclaw gateway restart
```

エージェントは起動時に `SOUL.md` を読み込み、`skills/` からスキルをロードして、すぐに動き始めます。

### 方法 C：手動セットアップ

1. 任意のパックを OpenClaw workspace ディレクトリにコピー
2. `TOOLS.md` に従って API キーと MCP ツールを設定
3. エージェントを再起動

---

## スキルの仕組み

スキルはテキストベースのワークフローガイドであり、実行可能なスクリプトではありません。ユーザーが「Acme 社を調べて」と言うと、エージェントは：

1. `skills/account-research/SKILL.md` を読み込む
2. 中に定義されたステップバイステップのワークフローに従う
3. 利用可能なツール（ウェブ検索、MCP コネクタ）を使って実行
4. 構造化された結果を返す

スキルはウェブ検索だけで動作します。MCP ツール（CRM、メール、カレンダー）を接続するとさらに高機能になりますが、接続なしでも完全に機能します。

---

## コントリビューション

新しいパックの提出を歓迎します！要件：

1. 6 つのコアファイルすべて：`SOUL.md`、`AGENTS.md`、`HEARTBEAT.md`、`TOOLS.md`、`MEMORY.md`、`README.md`
2. 完全な `SKILL.md` ワークフローを持つスキルが最低 1 つ
3. 実際の OpenClaw または ClawPod インスタンスでテスト済み
4. README にセットアップ手順と会話例を含む

フォーマットは既存のパックを参考にしてください。

---

## 帰属表示

[Anthropic の Knowledge Work Plugins](https://github.com/anthropics/knowledge-work-plugins)（Apache-2.0）から改変。詳細は [NOTICE](./NOTICE) を参照。

## ライセンス

MIT。Knowledge Work スキルは Anthropic の Apache-2.0 ライセンス作品から派生。詳細は [LICENSE](./LICENSE) を参照。

---

*[ClawPod](https://clawpod.app) がメンテナンス — 30 秒で AI Telegram Bot をデプロイ。*
