# X (Twitter) コンテンツカレンダー

週次で7本ずつ選定し、`drafts/YYYY-MM-DD.md` に下書きを生成する。

## フォーマット

| 記号 | 意味 |
|------|------|
| `- [ ]` | 未使用 |
| `- [x]` | 使用済み（日付付き） |

---

## カテゴリ一覧

### Productivity / Workflow

- [x] git worktreeで3〜5セッション並列実行 — 最大の生産性向上策 (2026-03-30)
- [ ] voice dictationで話す速度はタイピングの3倍 — 詳細なプロンプトが書ける
- [ ] Scheduled Tasks: /loop でローカル定期実行、/schedule でクラウド実行（マシンがオフでも動く）
- [ ] Remote Control: /rc でスマホ・タブレットからローカルセッションを継続

### Prompting

- [x] plan modeで計画に全エネルギーを注ぎ、1-shotで実装 (2026-03-31)
- [ ] "Prove to me this works" — mainとfeatureブランチの差分を比較させる
- [ ] "Grill me on these changes" — Claudeにレビュアーをやらせる
- [ ] "Knowing everything you know now, implement the elegant solution" — やり直しの指示

### Memory / Context

- [x] CLAUDE.mdに投資する — ミスのたびにルールを書かせ、ミス率が下がるまで反復 (2026-04-01)
- [ ] @path importでCLAUDE.mdを分割管理 — トピックごとにルールファイルを切り出す
- [ ] /compact を50%コンテキスト時点で手動実行 — コンテキスト枯渇を防ぐ
- [ ] output style "Explanatory" で新しいコードベースを学ぶ

### Skills

- [x] Skillの9カテゴリ分類 — Gotchasセクションが最も信号が高い (2026-04-02)
- [ ] Skillはフォルダ全体がコンテキストエンジニアリング — progressive disclosureを活用
- [ ] on-demand hooks: /careful, /freeze — 必要なときだけ有効化するフック
- [ ] Skillのdescriptionフィールドはモデル向けのトリガー条件を書く

### Subagents

- [x] test time compute — 複数コンテキストウィンドウで相関しないバグ検出 (2026-04-03)
- [ ] Agent vs Command vs Skill の使い分け — 自動起動・コンテキスト分離の違い
- [ ] "use subagents"を付けるだけで並列コンテキストが立ち上がる
- [ ] permissionリクエストをOpus経由でフック — 安全なものを自動承認

### Settings / Configuration

- [x] 設定ファイル5層階層 — チーム設定はsettings.jsonにコミット、個人はlocal (2026-04-04)
- [ ] /permissions でBash(bun run *)などワイルドカードで事前承認
- [ ] サンドボックス有効化 — /sandbox でファイル・ネットワーク分離
- [ ] env フィールドでシェルラッパースクリプト不要 — 100+の環境変数をsettings.jsonで管理

### Git Workflow

- [x] squash merge + median 118行PR — 1PR=1コミットで歴史をクリーンに (2026-04-05)
- [ ] Code Review: PRが開くとエージェントチームがバグを自動検出
- [ ] GitHub Actionsでレビュー・イシュートリアージを自動化
- [ ] git bisect のためにPRを小さく保つ — p90で498行以下が目安

### Hooks

- [ ] Hookの4つの実行タイプ: bash, http, prompt, agent
- [ ] PreToolUse フックで git commit 前に独自バリデーション
- [ ] Stop フックでClaudeが止まったとき自動で続行させる
- [ ] hooks-config.jsonをチームで共有、local.jsonで個人上書き

### MCP

- [ ] Slack MCPでバグスレッドを貼り付けて "fix" と言うだけ — コンテキストスイッチゼロ
- [ ] BigQuery MCPで自然言語からSQLを6ヶ月書いていない
- [ ] .mcp.jsonとsettings.jsonの使い分け — プロジェクト共有 vs 個人設定
