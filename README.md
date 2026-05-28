# hkraftlabs-site

HKraft Labs の公式ウェブサイト。GitHub Pages で `https://hkraftlabs.com` に公開。

## 構成

- `index.html` — トップページ (About / Services / Products / Contact)
- `privacy.html` — プライバシーポリシー (JP + EN)
- `terms.html` — 利用規約 (JP + EN)
- `styles.css` — 共通スタイル
- `CNAME` — GitHub Pages カスタムドメイン設定

## ローカルプレビュー

```sh
cd /Users/hiroki/vscode/hkraftlabs-site
python3 -m http.server 8000
# → http://localhost:8000 をブラウザで開く
```

## デプロイ

1. GitHub に新規 repo (`hkraftlabs-site` または `hkraftlabs.github.io`) を作成
2. このディレクトリを push
3. repo Settings → Pages → Source: `main` branch / root
4. Custom domain: `hkraftlabs.com` を設定 (CNAME ファイルが自動認識される)
5. お名前.com の DNS を設定:
   - A レコード (apex): `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - CNAME (`www`): `<username>.github.io.`
6. GitHub Pages 側で「Enforce HTTPS」を有効化

## 公開前に埋める必要があるもの

- support@hkraftlabs.com のエイリアスを Workspace で作成

## ライセンス

(C) 2026 HKraft Labs. All rights reserved.
