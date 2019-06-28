# gitlab-java-analysis
A gitlab plugin for static analysis of java code
基于gitlab的,通shell脚本调用java语言进行代码提交的规范检查



## 部署步骤
### 1. Gitlab 上安装JDK  
通过java -version 确定是否安装成功

例如出现以下类似信息代表安装成功：
```
java version "1.8.0_121"
Java(TM) SE Runtime Environment (build 1.8.0_121-b13)
Java HotSpot(TM) 64-Bit Server VM (build 25.121-b13, mixed mode) 
```

### 2. 部署shell脚本
2.1 找到gitlab服务需要校验的代码仓库地址

例如：test.git项目
```
/var/opt/gitlab/git-data/repositories/root/test.git
```
2.2 copy  check-lib/p3c-pmd-1.3.6.jar 到gitlab服务上
```
check-lib/p3c-pmd-1.3.6.jar
```
2.3 打开gitlab-plugin/pre-receive文件修改jar路径

例如：
```
JAVA_HOME=/var/opt/gitlab/git-data/repositories/root/test.git/custom_hooks
```

