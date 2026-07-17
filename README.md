# Pre-Animals サポートサイト

Pre-Animals が公開するアプリの、**サポートページとプライバシーポリシー**をまとめた静的サイトです。GitHub Pages で公開します。

このリポジトリには、**アプリ本体のソースコードは含まれません**。公開用のHTML/CSSのみです。

## 掲載しているアプリ

| アプリ | ページ |
| --- | --- |
| あれした？（かんたん行動記録） | `areshita/` |

今後、Days With You など他のアプリのページも、`areshita/` と同じ構成（`<アプリ>/`, `<アプリ>/privacy/`, `<アプリ>/support/`）で追加できます。

## 公開URL（GitHub Pages）

`[GitHubユーザー名]` は、公開後に実際の値へ置き換えてください。

- トップ： `https://[GitHubユーザー名].github.io/preanimals-support/`
- あれした？： `https://[GitHubユーザー名].github.io/preanimals-support/areshita/`
- プライバシーポリシー： `https://[GitHubユーザー名].github.io/preanimals-support/areshita/privacy/`
- サポート： `https://[GitHubユーザー名].github.io/preanimals-support/areshita/support/`

## ディレクトリ構成

```
preanimals-support/
├── index.html              Pre-Animals 入口
├── areshita/
│   ├── index.html          あれした？ 入口
│   ├── privacy/index.html  プライバシーポリシー
│   └── support/index.html  サポート
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
