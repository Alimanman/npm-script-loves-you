# 高阶篇
---

## npm script 跨平台兼容

~~~

## cross-var 引用变量

```
npm i cross-var -D
```

## cross-env 设置环境变量

```
npm i cross-env -D
```

---

## npm script 拆到单独文件中

```
npm i scripty -D

mkdir -p scripts/cover
touch scripts/cover.sh
touch scripts/cover/serve.sh
touch scripts/cover/open.sh
```

修改package.json

```
"scripts": {
     "cover": "scripty",
     "cover:serve": "scripty",
     "cover:open": "scripty"
}
```

## 用 node.js 脚本替代复杂的 npm script

~~~


