# 拥抱现代化前端工作流
---

## onchange

onchange 可以和 gulp、grunt 的 watch 一样强大。

```
npm i onchange -D
```

```
"scripts": {
    "watch": "onchange \"**/*.html\" \"**/*.css\"  \"**/*.js\" -- npm test"
}

```

## browser-sync

```
npm i browser-sync-D
```

```
"scripts": {
    "test": "browser-sync start --server --files \"**/*.html, **/*.css, **/*.js\""
}
```