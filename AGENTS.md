# .github

Repo-specific delta only. The global baseline is inherited; do not repeat it here.

## Scope

CyberticalAI organization の default community health files(`SECURITY.md`、`.github/pull_request_template.md`)を置く public リポ。適用条件は README の GitHub 公式文書を参照する。

## Paths

- `SECURITY.md` / `.github/pull_request_template.md` は org 全体へ継承される。`AGENTS.md` / `CODEOWNERS` / `README.md` はこのリポだけのもの

## Commands

- install / build: N/A(Markdown だけのリポ)
- CI: `.github/workflows/docs.yml` が README と SECURITY の存在・リンク、変更行を検査する

## Constraints

- public リポ。`README.md` の「編集にあたって」にある項目(社内チャンネル名・社内 URL、稼働中の検査構成やセキュリティツールの具体的な設定、個別リポジトリ名、個人のメールアドレス)を書かない
- 継承されるファイルを足したり外したりしたら、`README.md` の適用範囲の表も同じ変更で直す

## Verification

- PR の `docs` チェックを通し、GitHub 上で Markdown の表示を確認する

## Delivery

- 正本ブランチは `main`。merge した時点で、同名ファイルを持たない org 内のリポに適用される。デプロイ手順は無い
- 受入確認: 自前のテンプレートを持たない org 内のリポで PR を新規作成し、本文にテンプレートが入ることを見る

Keep this file under 200 lines and 16 KiB. Put multi-step or occasional procedures in docs or a task-specific Skill.
