# 概要
typescript,reactの検証用dockerファイル

# 実行方法
## typescript,reactのソース取得
[typescript,reactのレポジトリ](https://github.com/shintaro123/typescript_react)を本レポジトリと同階層にclone
```zsh
$ # こんな感じ
$ tree -L 2
.
├── practice_docker
│   ├── README.md
│   ├── docker-compose.yml
│   └── nginx01
└── typescript
    ├── README.md
    ├── src
    └── webpack.config.js
```

## コンテナを立ち上げる
```zsh
# 初回
docker-compose up -d --build
# 2回目以降
docker-compose up -d 
```

## ブラウザで確認
### hostsに追記
ローカルのhostsファイルに以下追記
```
127.0.0.1 practice.local
```

### ブラウザにアクセス
`http://practice.local`