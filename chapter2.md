# 进阶篇
---

## npm script 的钩子

`pre` 和 `post`,类似生命周期的机制。

举例来说，运行 npm run test 的时候，分 3 个阶段：

```
"pretest": "echo 3",
"test": "echo 2",
"posttest": "echo 1"
```

1. 检查 scripts 对象中是否存在 pretest 命令，如果有，先执行该命令；
2. 检查是否有 test 命令，有的话运行 test 命令，没有的话报错；
3. 检查是否存在 posttest 命令，如果有，执行 posttest 命令；

运行`npm t`,显示的结果是：

`
3
2
1
`

## npm script 中使用变量

```
npm run env
```

## 实现命令行自动补全