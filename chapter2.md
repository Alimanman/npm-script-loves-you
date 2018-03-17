# 进阶篇
---

## npm script 的钩子

`pre` 和 `post`

举例来说，运行 npm run test 的时候，分 3 个阶段：

```
"pretest":"1"
"test":"2"
"posttest":"3"
```

1. 检查 scripts 对象中是否存在 pretest 命令，如果有，先执行该命令；
2. 检查是否有 test 命令，有的话运行 test 命令，没有的话报错；
3. 检查是否存在 posttest 命令，如果有，执行 posttest 命令；