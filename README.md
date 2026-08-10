# ナンプレIQ 公開サイト

iOSアプリ「ナンプレIQ」のサポート・プライバシーポリシー等を配信する静的サイトです。

**公開予定URL: https://sudoku-iq.jewelrysunflower.com/**

```
index.html          … アプリ紹介ページ            → /
support/index.html  … サポートページ              → /support/
privacy/index.html  … プライバシーポリシー         → /privacy/
```

素のHTML(CSSはインライン、外部依存は Google Fonts のみ)。**ビルド不要**。

## App Store Connect に登録するURL

| 項目 | URL |
|---|---|
| サポートURL | `https://sudoku-iq.jewelrysunflower.com/support/` |
| プライバシーポリシーURL | `https://sudoku-iq.jewelrysunflower.com/privacy/` |

## ⚠️ 既存サイトとの関係

このリポジトリは **`sudoku-iq.jewelrysunflower.com` 専用**です。

`deskflowlabs.jewelrysunflower.com`(7か国語の既存サイト)を配信している
Cloudflare Pages プロジェクト **`deskflow-labs-site` には接続しないでください**。
接続すると既存サイトがこのリポジトリの内容で置き換わります。

**新規の Cloudflare Pages プロジェクトを作成して接続してください。**

## Cloudflare Pages の設定(新規プロジェクト)

| 項目 | 値 |
|---|---|
| プロダクションブランチ | `main` |
| フレームワークプリセット | None |
| ビルドコマンド | 空欄 |
| ビルド出力ディレクトリ | `/` |

接続後、カスタムドメインに `sudoku-iq.jewelrysunflower.com` を追加します。

## 公開前に差し替えが必要な箇所

| ファイル | 検索文字列 | 置換内容 |
|---|---|---|
| `support/index.html` | `REPLACE_ME@example.com`(2箇所) | 問い合わせ用メールアドレス |
| `privacy/index.html` | `REPLACE_ME@example.com`(2箇所) | 同上 |
| `index.html` | `class="cta soon"` / `href="#"` | アプリ公開後、`soon` を外し App Store のURLを設定 |
