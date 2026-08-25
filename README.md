# ナンプレIQ 公開サイト

iOSアプリ「ナンプレIQ」のサポート・プライバシーポリシー等を配信する静的サイトです。

**公開URL: https://sudoku-iq.jewelrysunflower.com/**

```
index.html              … アプリ紹介ページ            → /
support/index.html      … サポートページ              → /support/
privacy/index.html      … プライバシーポリシー         → /privacy/

favicon.ico             … タブアイコン(16/32/48px)
favicon.svg             … タブアイコン(ベクター・モダンブラウザ用)
apple-touch-icon.png    … iOSホーム画面用(180px)
og-image.png            … SNS/チャットのリンクプレビュー用(1200x630)
appstore-badge-ja.svg   … App Store バッジ(Apple公式アートワーク・日本語)
```

アイコン類は `scripts/gen_favicon.py`(親プロジェクト側)で `index.html` のヒーローアイコンと
同じ意匠から生成しています。デザインを変えたい時はスクリプトを直して再生成してください。

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

## App Store

| 項目 | 値 |
|---|---|
| アプリID | `6792964012` |
| Bundle ID | `com.deskflowlabs.sudoku-iq` |
| 販売者 | 株式会社ジュエリーサンフラワー (JEWELRY SUNFLOWER, K.K.) |
| ストアURL | https://apps.apple.com/jp/app/id6792964012 |
| 公開日 | 2026-08-17(価格: 無料 / iOS 15.0以上 / iPhone・iPad対応) |

`index.html` のヒーローに Apple 公式バッジ(`appstore-badge-ja.svg`)を設置済み。
併せて `<meta name="apple-itunes-app" content="app-id=6792964012">` により
iOS Safari でスマートアプリバナーが表示されます。

> バッジは Apple のマーケティングガイドライン上、**縦横比の変更・色や文字の改変が禁止**です。
> 差し替える場合は https://toolbox.marketingtools.apple.com/ の公式アートワークを使ってください。
