# fuzihara App

## 仕様

### ざっくり

- hot peper api を使用してグルナビ的なappをつくる
- login機能あり
- user my pageあり
- mainの機能は店を探して表示
- とりあえずお気に入りon/offだけ最初は実装する

### ページ

- ログイン
- マイページ
- メインの検索フォーム & 検索結果
- お気に入り店舗一覧

### 機能

- ユーザー登録とログイン
- ユーザーデータを一部修正できる。削除も可能

### あとで追加するかも

- パスワード再設定
- パスワード忘れた時の再設定
- 管理者権限
- もし店舗データを持つならtop pageに「昨日追加した店舗一覧」とかはあり


### どっち？

#### リアルタイム制を重視するか、レスポンスを早くするか(APIを都度叩く負荷)

店舗データをこっちで持つかAPI叩くか?  
→功いわくバッチがいいと思うとのこと

#### Rails APIで作る時一緒のリポジトリ？

分けた方がいいけど、どちらでもいい。

##### 一緒になるメリット

- 対応するAPI versionが一緒になる
- Gitの管理上でリリースをすり合わせられる

##### 分ける場合

- Gitツリーが見やすい
- 権限を管理できる
