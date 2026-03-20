# portfolio-site

[![Netlify Status](https://api.netlify.com/api/v1/badges/6cfe1eb5-d9af-48ce-af3e-79b1ef33bfcf/deploy-status)](https://app.netlify.com/sites/portfolio-robo358/deploys)

[ROBO358](https://ROBO358.com/) のポートフォリオ・ブログサイト。[Hugo](https://gohugo.io/) + [Blowfish](https://blowfish.page/) テーマで構築し、[Netlify](https://www.netlify.com/) でホスティングしている。

---

## Local run

Hugoが必要。インストール方法は [公式ドキュメント](https://gohugo.io/installation/) を参照

```bash
git clone --recurse-submodules https://github.com/ROBO358/portfolio-site.git
cd portfolio-site
hugo server -D
```

---

## Deploy

`main` ブランチへ push すると Netlify が自動でビルド・デプロイする。設定は [netlify.toml](netlify.toml) を参照

手動でビルドする場合:

```bash
hugo --gc --minify
```

---

## Config

設定ファイルは`config/_default/`以下にある。各パラメータの意味は [Blowfish のドキュメント](https://blowfish.page/docs/configuration/) を参照

Custom headersをNetlifyに適用する設定が`static/_headers`にある。これは[Netlifyのドキュメント](https://docs.netlify.com/routing/headers/) を参照
