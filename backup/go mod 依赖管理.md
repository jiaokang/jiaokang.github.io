## 进入到目录中 go mod init {项目名} 来初始化go项目,并生成go.mod文件
### go.mod用来管理依赖
```
// 模块名
module gomod
// sdk版本
go 1.22.1

// 当前module项目依赖的包
require(
 // dependency latest
)

// 排除第三方包
exclude(
// dependency latest
)

// 修改依赖包的路径或者版本
// 当依赖包发生迁移
// 原始包无法访问
// 二次开发第三方包
replace(
 // source latest => target latest
)

// 撤回
// 当前项目作为其他项目的依赖,如果说某个版本出现了问题
// 可以通过retract撤回
retract(
 // v1.0.0
)
```