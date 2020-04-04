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

## sequelize memo

- config
  - DB へ接続するための DB の URL 、アカウント、パスワード、データベース名を記述する config.json ファイルが格納されるディレクトリ
- migrations
  - DB マイグレーション用処理用のスクリプトを格納するディレクトリ
- models
  - DB の OR マッピングされたモデルの定義を記述するファイルを格納するディレクトリ。models ディレクトリ配下のモデルを読み込む index.js が作成される。（後述）
- seeders
  - テスト目的で利用する DB データ(seed)を作成するためのスクリプトファイルが格納されるディレクトリ。
