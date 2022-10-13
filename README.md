# 概要

lwc（Lightning Web コンポーネント）を trailhead でキャッチアップしたときのコードを残しておくリポジトリです

## trailhead

これやります
https://trailhead.salesforce.com/ja/content/learn/trails/build-lightning-web-components

## 気づいたメモ

### trailheadに従ってプロジェクト初期化にフォーマッタ

https://trailhead.salesforce.com/ja/content/learn/projects/quick-start-lightning-web-components/create-a-hello-world-lightning-web-component?trail_id=build-lightning-web-components

これをやっているときにyarn installしてフォーマッタ適用すると逆にエラーが出る・・・
.prettierrcの設定を入れればOK
参考: https://salesforce.stackexchange.com/questions/254786/vs-code-adds-quotes-in-lwc

### 作ったlwcがLightningアプリケーションビルダーに表示されない

xmlのisExposedをtrueにする
参考: https://salesforce.stackexchange.com/questions/255160/lightning-web-components-not-available-in-app-builder
