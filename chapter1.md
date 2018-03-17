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
---

## 创建自定义 npm script

### 1.添加 eslint 依赖

-D等于--save-dev

```
npm i eslint -D
```

### 2.生成规则

配置好后，根目录自动生成一个`.eslintrc.js`文件。

```
eslint --init
```

### 3.添加 eslint 命令

```
"scripts": {
    "eslint": "eslint *.js",
    "test": "echo \"Error: no test specified\" && exit 1"
}
```

### 4.运行

```
npm run eslint
```

- lint vue：https://github.com/vuejs/eslint-plugin-vue
- lint style:https://stylelint.io/
 - 新建`.stylelintrc`无后缀目录，加入规则。
- lint json:https://github.com/zaach/jsonlint
- lint markdown:https://github.com/igorshubovych/markdownlint-cli

---

## 运行多个 npm script

### 1.npm-run-all

```
npm i npm-run-all -D
```

### 2.package.json

```
"scripts": {
    "lint:js": "eslint *.js",
    "lint:css": "stylelint *.css",
    "test": "npm-run-all lint:js lint:css"
}
```

### 3.运行

```
npm test
npm t
```

这2种都可以

### 并行实行

此外，以上npm-run-all模式是顺序运行，如果要并行实行的话。

```
"test": "npm-run-all --parallel lint:js lint:css"
```

npm-run-all文档：https://github.com/mysticatea/npm-run-all/blob/HEAD/docs/npm-run-all.md

---

### 给 npm script 传递参数

eslint自动修复非语法类错误，命令行后添加`-- --fix`

```
npm run lint:js -- --fix
```














