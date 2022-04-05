
调试mvn程序
1. 使用mvnDebug命令
2. export JAVA_TOOL_OPTIONS：-agentlib:jdwp=transport=dt_socket,server=y,suspend=n,address=1044
```
1. 搞清楚你的代码跑在那个jdk里面
2. 找到跑的程序的代码对应的源代码
```

详细步骤
例如要调试Main.calss
拿到在命令行中使用
```bash
java -agentlib:jdwp=transport=dt_socket,server=y,suspend=y,address=1044 Main
```
然后打开IDEA->Configure -> remote 修改你的端口
then:
可以愉快的开始debug了