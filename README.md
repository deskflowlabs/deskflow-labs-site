# deskflow-labs-site

Cloudflare Pages プロジェクト **`deskflow-labs-site`**(https://deskflowlabs.jewelrysunflower.com )で配信する静的サイトです。

```
sudoku-iq/index.html          … ナンプレIQ 紹介ページ
sudoku-iq/support/index.html  … サポートページ(App Store のサポートURL)
sudoku-iq/privacy/index.html  … プライバシーポリシー(App Store の必須URL)
```

素のHTMLのみで、ビルド作業は不要です。

> ⚠️ **トップページ(`/`)は既存のものを使用します。**
> Cloudflare Pages を Git 連携にすると、デプロイ内容はこのリポジトリの中身で
> **サイト全体が置き換わります**。連携する場合は、既存のトップページ一式も
> このリポジトリに含めてください。含めないとトップページが 404 になります。

## Cloudflare Pages の設定

Cloudflare ダッシュボード → Workers & Pages → `deskflow-labs-site` → 設定 → Build →
**Git repository の「Connect」** からこのリポジトリを接続します。

| 項目 | 値 |
|---|---|
| ビルドコマンド | 空欄 |
| ビルド出力ディレクトリ | `/` |

接続後は、`main` ブランチに push するだけで自動デプロイされます。

## 公開前に差し替えが必要な箇所

| ファイル | 箇所 | 内容 |
|---|---|---|
| `sudoku-iq/support/index.html` | `REPLACE_ME@example.com`(2箇所) | 実際の連絡先メールアドレス |
| `sudoku-iq/privacy/index.html` | `REPLACE_ME@example.com`(2箇所) | 実際の連絡先メールアドレス |
| `sudoku-iq/index.html` | `class="cta soon"` / `href="#"` | アプリ公開後、`soon` を外して App Store のURLを設定 |

## 確認URL

- https://deskflowlabs.jewelrysunflower.com/
- https://deskflowlabs.jewelrysunflower.com/sudoku-iq/
- https://deskflowlabs.jewelrysunflower.com/sudoku-iq/support/
- https://deskflowlabs.jewelrysunflower.com/sudoku-iq/privacy/
