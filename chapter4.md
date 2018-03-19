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

---

## npm script 实现构建流水线

### 项目目录结构

```
src
├── images
│   └── schedule.png
├── index.html
├── scripts
│   └── main.js
└── styles
    └── main.css
```

功能要求
1. 压缩图片；
2. 编译 less、压缩 css；
3. 编译、压缩 js；
4. 给图片加版本号并替换 js、css 中的引用；
5. 给 js、css 加版本号并替换 html 中的引用；









