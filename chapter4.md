# 拥抱现代化前端工作流
---

## onchange

onchange 可以和 gulp、grunt 的 watch 一样强大。

```
npm i onchange -D
```

## browser-sync

```
npm i browser-sync-D
```

```
"scripts": {
    "lint:js": "eslint *.js",
    "test": "browser-sync start --server --files \"**/*.html, **/*.css, **/*.js\""
}
```