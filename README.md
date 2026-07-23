# Pre-Animals サポートサイト

Pre-Animals が公開するアプリの、**サポートページとプライバシーポリシー**をまとめた静的サイトです。GitHub Pages で公開します。

このリポジトリには、**アプリ本体のソースコードは含まれません**。公開用のHTML/CSSのみです。

## 掲載しているアプリ

| アプリ | ページ |
| --- | --- |
| あれした？（かんたん行動記録） | `areshita/` |
| イツマデ（暮らしの期限管理） | `itsumade/` |

今後のアプリのページも、`areshita/` と同じ構成（`<アプリ>/`, `<アプリ>/privacy/`, `<アプリ>/support/`）で追加できます。

**`itsumade/` だけは扱いが違います。** アプリ本体のリポジトリで生成しているため、
共通の `assets/styles.css` を読まず、配色を自前で持っています。文面もアプリ内の
画面と同じ元データ（`src/lib/data/legal.ts`）から作られます。更新するときは
itsumade 側で `npm run build:web` を実行し、生成された `web/` の中身を
このリポジトリの `itsumade/` へ上書きコピーしてください。ここで直接編集すると、
次の生成で戻ります。

## 公開URL（GitHub Pages）

- トップ： <https://preanimals.github.io/preanimals-support/>

あれした？

- 入口： <https://preanimals.github.io/preanimals-support/areshita/>
- プライバシーポリシー： <https://preanimals.github.io/preanimals-support/areshita/privacy/>
- サポート： <https://preanimals.github.io/preanimals-support/areshita/support/>

イツマデ

- 入口： <https://preanimals.github.io/preanimals-support/itsumade/>
- プライバシーポリシー： <https://preanimals.github.io/preanimals-support/itsumade/privacy/>
- サポート： <https://preanimals.github.io/preanimals-support/itsumade/support/>
- 利用規約： <https://preanimals.github.io/preanimals-support/itsumade/terms/>

リポジトリ： <https://github.com/preanimals/preanimals-support>

### App Store Connect に入力するURL

あれした？

| 項目 | URL |
| --- | --- |
| Privacy Policy URL | `https://preanimals.github.io/preanimals-support/areshita/privacy/` |
| Support URL | `https://preanimals.github.io/preanimals-support/areshita/support/` |
| Marketing URL（任意） | `https://preanimals.github.io/preanimals-support/areshita/` |

イツマデ

| 項目 | URL |
| --- | --- |
| Privacy Policy URL | `https://preanimals.github.io/preanimals-support/itsumade/privacy/` |
| Support URL | `https://preanimals.github.io/preanimals-support/itsumade/support/` |
| Marketing URL（任意） | `https://preanimals.github.io/preanimals-support/itsumade/` |

## ディレクトリ構成

```
preanimals-support/
├── index.html              Pre-Animals 入口
├── areshita/
│   ├── index.html          あれした？ 入口
│   ├── privacy/index.html  プライバシーポリシー
│   └── support/index.html  サポート
├── itsumade/               イツマデ（itsumade 側の build:web が生成）
│   ├── index.html
│   ├── privacy/index.html
│   ├── support/index.html
│   └── terms/index.html
├── assets/
│   └── styles.css          共通スタイル
├── .nojekyll               GitHub Pages に Jekyll 処理をさせない
└── README.md
```

## 更新方法

1. 対象のHTMLを編集します（文面や日付など）。
2. プライバシーポリシーを変更したときは、`最終更新日` を書き換えます。
3. コミットして `main` に push すると、GitHub Pages に自動で反映されます。

## ローカルでの確認方法

```bash
cd preanimals-support
python3 -m http.server 8000
```

ブラウザで `http://127.0.0.1:8000/` を開きます。リンクはすべて相対パスのため、GitHub Pages のプロジェクトサイト配下（`/preanimals-support/…`）でもそのまま動作します。

## お問い合わせ

dayswithyousupport@gmail.com

## 方針

- アプリ本体のソースコードは置きません（公開ページのみ）。
- Apple ID、Team ID、署名情報、個人用の連絡先などの秘密情報・個人情報は置きません。
- 掲載するのは、上記の公開用サポート窓口のメールアドレスのみです。
