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
Cloudflare Pages プロジェクト **`deskflow-labs-site` には絶対に接続しないでください**。
接続すると既存サイトがこのリポジトリの内容で置き換わります。

## Cloudflare Pages の設定(設定済み)

| 項目 | 値 |
|---|---|
| プロジェクト名 | `sudoku-iq-site` |
| プロダクションブランチ | `main` |
| フレームワークプリセット | None |
| ビルドコマンド | 空欄 |
| ビルド出力ディレクトリ | `.` |
| カスタムドメイン | `sudoku-iq.jewelrysunflower.com`(Active / SSL 有効) |

`main` への push で自動デプロイされます。

## 問い合わせ先

`support@jewelrysunflower.com`(他アプリと共通。**件名でアプリを判別する運用**)

サポートページ・プライバシーポリシーの双方に
「お問い合わせの際は、件名に『ナンプレIQ』とご記載ください。」と案内を掲載しています。

## 今後の差し替え予定

| ファイル | 箇所 | 内容 |
|---|---|---|
| `index.html` | `class="cta soon"` / `href="#"` | アプリ公開後、`soon` を外し App Store のURLを設定 |
