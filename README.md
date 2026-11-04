# 🏢 ConnectField (社内・現場向けスレッド掲示板)

[![GitHub Pages Deployment](https://img.shields.io/badge/status-active-success.svg)](https://your-username.github.io/repository-name/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

本社（マネジメント層）と現場（スタッフ）のコミュニケーションを円滑にするための、スレッド形式の掲示板Webアプリケーションです。現場の状況や業務連絡をリアルタイムで共有し、スムーズな情報連携をサポートします。

<br>

## 🖼️ スクリーンショット
| スレッド一覧画面 | 投稿作成画面 |
| :---: | :---: |
| ![Thread List](./assets/images/thread-list.png) | ![Post Create](./assets/images/post-create.png) |

---

## 🔗 デモ
実際にブラウザで操作していただけます：
👉 [デモサイトはこちら](https://your-username.github.io/repository-name/)

---

## 🛠️ 使用技術 (Tech Stack)
* **Frontend**: HTML5, CSS3, JavaScript (ES6+)
* **Styling**: Flexbox / Grid, CSS Variables
* **Data Persistence**: LocalStorage (ブラウザ内保存)
* **Deployment**: GitHub Pages
* **Tools**: Visual Studio Code, Git / GitHub

---

## 📋 設計ドキュメント (Design Documents)

本アプリケーションの設計図（ワイヤーフレームおよびER図）は、以下の `docs/` フォルダ内に格納しています。

* 📁 **`docs/wireframe.png`**: 画面遷移およびレイアウト構成を表すワイヤーフレーム
* 📁 **`docs/er-diagram.png`**: データベースのテーブル構造およびリレーションを表すER図

---

## ✨ 主な機能 (Features)
* **スレッド投稿・削除機能**
  * タイトル、本文、画像（任意）を入力して新しいスレッドを作成できます。
* **いいね・コメント（返信）機能**
  * 各スレッドに対してリアクションや意見のやり取りが行えます。
* **従業員プロフィール編集**
  * 部署名や名前を設定でき、匿名性を保ちつつ誰からの発信か分かりやすい設計にしています。
* **通知一覧**
  * 自分宛ての返信や新しいメンション情報を一覧で確認できます。
* **キーワード検索バー**
  * 目的のスレッドをキーワードで素早く絞り込んで探すことができます。

---

## 💡 こだわったポイント・工夫した点 (Highlights)
1. **現場目線に立った使いやすいUI/UX**
   * スマートフォンやタブレットなど、現場の移動中や作業の合間でも直感的にタップ・閲覧しやすいよう、レスポンシブデザインを徹底しました。
2. **スレッドと返信のデータ構造（リレーション）の意識**
   * フロントエンドのみの環境でも、親スレッドと子コメントの紐付けがスムーズに行えるよう、JavaScriptのデータ構造（配列とオブジェクトの組み合わせ）を工夫して設計しました。
3. **プライバシーと運用のバランス**
   * 現場での心理的安全性を考慮しつつ、一律のアイコンや部署情報を取り入れた「匿名性を守りながらも誰の意見か伝わる」プロフィール管理機能を実装しました。

---

## 📂 ディレクトリ構成 (Directory Structure)
```text
repository-name/
├── index.html          # トップ画面（全投稿一覧・検索）
├── create.html         # 投稿作成画面
├── profile.html        # プロフィール編集画面
├── notifications.html  # 通知一覧画面
├── style.css           # 共通スタイルシート
├── script.js           # アプリケーションのロジック・DOM操作
├── docs/               # 設計ドキュメント格納フォルダ
│   ├── wireframe.png   # ワイヤーフレーム画像
│   └── er-diagram.png  # ER図画像
├── assets/
│   └── images/         # アプリ画面のスクリーンショット画像
└── README.md
