# pipeline-tutorial

### 代码提交规范
```
[类别]：context
类别：
    feat : 新功能
    fix : 修复bug
    docs : 文档改变
    style : 代码格式改变
    refactor : 某个已有功能重构
    perf : 性能优化
    test : 增加测试
    build : 改变了build工具 如 grunt换成了 npm
    revert : 撤销上一次的 commit
    chore : 构建过程或辅助工具的变动
```


### pipeline搭建说明规范


### 目录说明
```
controller: 与第三方、前端打交道 调用service方法

dao: 数据访问对象、负责数据库打交道

service：处理数据信息 与dao和controller打交道，一般调用dao的方法

model：数据类型定义 eg：User、Student
```
