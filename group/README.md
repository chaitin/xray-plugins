# 运行策略组

该文件夹中的主要存放一些希望一起运行的插件的文件，便于使用者可以快捷的使用一些预设好的策略组合

## 文件格式

- 策略组文件实际上是一个txt文件，一行表示一个加载策略，一般约定使用`.list`作为文件后缀
- 每行中可以写相对路径，绝对路径，以及glob风格的路径 

### 具体示例

**绝对路径**
```text
/root/xray-plugins/finger/manual/web/Azure.yml
/root/xray-plugins/finger/manual/service/*.yml
```

**相对路径**

相对运行目录的路径：
```text
finger/manual/web/Azure.yml
finger/manual/service/*.yml
```
如果希望是相对这个策略组文件的路径，则可以写：
```text
{{path}}/../finger/manual/web/Azure.yml
{{path}}/../finger/manual/service/*.yml
```
系统会自动取当前策略组文件的路径，替换到`{{path}}`中。

## 策略组文件说明

每个策略组文件都应该有一个说明，表示建立该策略组的目的，如果提交一个新的策略组，请务必在该文件中添加说明。

- test.list：测试用例，用于示范如何使用策略组
- hvv.list：一些在hvv中重点关注的产品的指纹
