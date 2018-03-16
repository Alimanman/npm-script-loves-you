# 入门篇
---

## npm init 快速创建项目

```
npm init
```

### 预设值

```
npm config set init.author.email "longjun.huang@rakuten.com"
npm config set init.author.name "Huang, Longjun"
npm config set init.author.url "http://git.rakuten-it.com"
npm config set init.license "MIT"
npm config set init.version "0.1.0"
```

### 快速建立

```
npm init -f
```

## 创建自定义 npm script

### 1.添加 eslint 依赖

-D等于--save-dev

```
npm install eslint -D
```

### 2.生成配置

配置好后，根目录自动生成已个`.eslintrc.js`文件。

```
eslint --init
```

### 3.添加 eslint 命令

```
"scripts": {
    "eslint": "eslint index.js",
    "test": "echo \"Error: no test specified\" && exit 1"
}
```

### 4.运行

```
npm run eslint
```
---

///















