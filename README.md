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
    
    build : 改变了build工具 如 grade 换成了 npm
    
    revert : 撤销上一次的 commit
    
    chore : 构建过程或辅助工具的变动
```


### pipeline搭建说明规范

### 文件命名规范
```
包的命名：全部小写，eg：server

类的命名：单词首字母大写，eg：Controller、loginServer

方法的命名：首字母小写，后面的字母开头大写，eg：loginMethod

常量的命名：全部大写 ，常加下划线 eg：MAX_NUMBER

变量的命名：首字母小写，后面的字母开头大写，eg：loginMethod
```

### 目录说明
```
controller: 与第三方、前端打交道 调用service方法

dao: 数据访问对象、负责数据库打交道

service：处理数据信息 与dao和controller打交道，一般调用dao的方法

model：数据类型定义 eg：User、Student
```
