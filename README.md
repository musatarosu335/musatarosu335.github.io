# musatarosu335.github.io

iOSアプリの公式サイト（GitHub Pages）。

公開URL: https://musatarosu335.github.io/

## 目的

| ファイル | 役割 |
|---|---|
| `app-ads.txt` | AdMobの広告収益最適化のための認証ファイル。ドメインのルートに置く必要がある |
| `hibino-bunko/privacy.html` | 日々ノ文庫のプライバシーポリシー。App Store Connect の「プライバシーポリシーURL」に登録する |
| `index.html` | アプリ紹介ページ兼サポートページ。App Store Connect の「マーケティングURL」「サポートURL」に登録する |

## app-ads.txt について

AdMobは **App Store掲載の「デベロッパWebサイト」（App Store Connect のマーケティングURL）のドメイン直下** をクロールして `app-ads.txt` を探す。そのため以下の2つが揃っている必要がある。

1. `https://musatarosu335.github.io/app-ads.txt` が公開されていること
2. App Store Connect の**マーケティングURL**が `https://musatarosu335.github.io/` になっていること

内容はAdMobの管理画面（アカウント > アカウント情報）に表示されるスニペットと完全に一致させる。パブリッシャーIDは `pub-9607668579731485`。

反映後、AdMob管理画面の「アップデートを確認」を押すと再クロールされる（数分〜数日）。

## 更新方法

ファイルを編集して `main` ブランチにpushすると自動的に反映される（GitHub Pages）。
