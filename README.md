# .github

株式会社サイバーティカル（CyberticalAI organization）の **default community health files** を置くリポジトリです。

ここに置いたファイルは、同じ organization が所有するリポジトリのうち、**自前の同名ファイルを持たないもの** に自動で適用されます。GitHub の仕様上、この機能を有効にするには本リポジトリが public である必要があります。

適用条件と配置場所は GitHub の[既定コミュニティファイルの説明](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file)に従います。ここでは `.github/pull_request_template.md` と `.github/ISSUE_TEMPLATE/` を使います。

| ファイル | 適用範囲 |
| --- | --- |
| [`SECURITY.md`](./SECURITY.md) | 脆弱性の報告経路と対応の目安 |
| [`.github/pull_request_template.md`](./.github/pull_request_template.md) | PR 本文の既定(何を・なぜ・どう確かめたか)と、Issue を閉じる `Closes #番号`。自前の PR テンプレートを持たないリポで、PR 作成時に本文へ入る |
| [`.github/ISSUE_TEMPLATE/task.yml`](./.github/ISSUE_TEMPLATE/task.yml) | Issue フォーム「作業」(As-Is・To-Be・実行・証拠)。自前の `.github/ISSUE_TEMPLATE/` を持たないリポで、Issue 作成時に選べる |

## 編集にあたって

このリポジトリは **public** です。以下は書かないでください。

- 社内チャンネル名、社内システムの URL、社内向け runbook へのリンク
- 稼働中の検査構成やセキュリティツールの具体的な設定
- 個別リポジトリ名や、まだ公開していないサービスの名称
- 連絡先として個人のメールアドレス

社内向けの詳細版は private 側の正典に置いています。

## 個別リポジトリで上書きしたいとき

そのリポジトリのルートに `SECURITY.md` を置けば、そちらが優先されます(PR テンプレートも同じで、リポ側に `.github/pull_request_template.md` などがあればそちらが使われます。Issue テンプレートは、リポ側に `.github/ISSUE_TEMPLATE/` があると、ここのものは一つも使われません)。社内情報を含む完全版を使いたい場合はこの方法を取ってください。
