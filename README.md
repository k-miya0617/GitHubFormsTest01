## GitHub Forms 入門

### 概要

- Issue作成のためのフォームを作成することができる。
- フォームの定義をyamlファイルで記述する。
  - 入力要素、説明文など （詳細は別記）
- フォームのSubmit new issueを押下すると、フォームの内容がそのままIssueに反映される。
- まだbeta版。現在のWoomsにはまだ不適格。今後のアップデートに期待。

### サンプルリポジトリ

これ

### 参考資料

-  [GitHub のフォームスキーマの構文 - GitHub Docs](https://docs.github.com/ja/communities/using-templates-to-encourage-useful-issues-and-pull-requests/syntax-for-githubs-form-schema#input) 

### 使える要素 （概要 詳しくは画面共有しながら）

- `markdown`
  - フォーム上に記載するマークダウン
  - ユーザに説明文などを提供する際に利用
  - ここで書かれた内容は**Issueに記述されない**
- `checkboxes`
- `dropdown`
  - 単一選択、複数選択 両方可能
- `input`
  - 一行の文字列を入力する際に利用。
- `textarea`
  - 複数行の文字列を入力する際に利用。
  - ユーザはマークダウンを記述できる他、画像のアップロードも可能

### 課題

- フォームの内容を動的に変更することができなさそう
  - 例: チェックボックスをつけると入力要素が増える、減る、など
  - 例: dropboxに既存のブランチの一覧を出す、など
