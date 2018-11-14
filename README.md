# SSScript
一些图片批量处理脚本，用于React Native项目

## 使用方法

### 重命名

```
rpn a b
rpn a.png b
rpn a@2x.png b
rpn a@3x.png b
```
以上代码均可将当前目录下`a.png`的所有1x,2x,3x文件重命名为`b.png`的对应文件。

### 输出相关文件夹的对应JS代码

```
cpn a
```

若当前目录下有`a`文件夹，`a`文件夹中有`b.png`,`b@2x.png`,`b@3x.png`，`c.png`,`c@2x.png`,`c@3x.png`文件。
将输出以下内容
```
a: {
    b: require('./a/b.png'),
    c: require('./a/c.png')
}
```
