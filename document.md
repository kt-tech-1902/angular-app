# 2023/12/28 課題対応

## 課題の対応目的

Angular を過去に触ったことが無かったのだが、直近で Angular を触ることになったので、公式チュートリアルを触り Angular の仕組みの部分から把握する

## 環境

| 技術環境   | 使用バージョン等 |
| ---------- | ---------------- |
| OS         | Windows          |
| Node.js    | 20.10.0          |
| TypeScript | 5.3.3            |
| エディタ   | VSCode           |

## 参考サイト

-   Angular 公式チュートリアル
    -   https://angular.jp/tutorial/first-app

## 問題

-   スクリプトの実行が失敗
    -   発生タイミング：VScode 上で'tsc -v'を実行
    -   解決策：PowerShell のスクリプトの実行ポリシーを変更
    -   参考：https://qiita.com/Targityen/items/3d2e0b5b0b7b04963750
