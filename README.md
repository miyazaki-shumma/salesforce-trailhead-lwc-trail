# 概要

lwc（Lightning Web コンポーネント）を trailhead でキャッチアップしたときのコードを残しておくリポジトリです

## trailhead

これやります
https://trailhead.salesforce.com/ja/content/learn/trails/build-lightning-web-components

## コマンドメモ

```bash
# スクラッチ組織へコード反映
sfdx force:source:push
# スクラッチ以外の組織へコードは反映
sfdx force:source:deploy -u 組織名 -p force-app/main/default
# スクラッチ組織を開く
sfdx force:org:open
# 認証した組織一覧
sfdx force:org:list

```

## 気づいたメモ

### trailhead に従ってプロジェクト初期化にフォーマッタ

https://trailhead.salesforce.com/ja/content/learn/projects/quick-start-lightning-web-components/create-a-hello-world-lightning-web-component?trail_id=build-lightning-web-components

これをやっているときに yarn install してフォーマッタ適用すると逆にエラーが出る・・・
.prettierrc の設定を入れれば OK
参考: https://salesforce.stackexchange.com/questions/254786/vs-code-adds-quotes-in-lwc

### 作った lwc が Lightning アプリケーションビルダーに表示されない

xml の isExposed を true にする
参考: https://salesforce.stackexchange.com/questions/255160/lightning-web-components-not-available-in-app-builder
