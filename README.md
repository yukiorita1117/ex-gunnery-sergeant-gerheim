# このリポジトリについて

react-express のボイラーテンプレートです。

## 実行

`npm run dev`

## 運用

原則このリポジトリでは server を管理する。<br/>
その為、client の変更は行わないようにする。
client のリポジトリ管理は `[project name]-client` で行う。

## アーキテクト

React<br/>
react-router-dom<br/>
axios<br/>
mysql<br/>
express(Sequelize)<br/>

## ターゲット

1. show / create / update / delete api を作成。
2. 作成画面 / 編集画面 / 一覧画面 の作成
3. 作成画面 → create 編集画面 → show,update,delete 一覧画面 → id と name だけを全件取得する。
4. 編集画面で既に作成した data を削除した際,router を用いて一覧画面に戻る。この時 DB から再 fetch する。
