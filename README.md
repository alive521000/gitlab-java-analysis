# gitlab-java-analysis
A gitlab plugin for static analysis of java code
����gitlab��,ͨshell�ű�����java���Խ��д����ύ�Ĺ淶���



## ������
### 1. Gitlab �ϰ�װJDK  
ͨ��java -version ȷ���Ƿ�װ�ɹ�

�����������������Ϣ����װ�ɹ���
```
java version "1.8.0_121"
Java(TM) SE Runtime Environment (build 1.8.0_121-b13)
Java HotSpot(TM) 64-Bit Server VM (build 25.121-b13, mixed mode) 
```

### 2. ����shell�ű�
2.1 �ҵ�gitlab������ҪУ��Ĵ���ֿ��ַ

���磺test.git��Ŀ
```
/var/opt/gitlab/git-data/repositories/root/test.git
```
2.2 copy  check-lib/p3c-pmd-1.3.6.jar ��gitlab������
```
check-lib/p3c-pmd-1.3.6.jar
```
2.3 ��gitlab-plugin/pre-receive�ļ��޸�jar·��

���磺
```
JAVA_HOME=/var/opt/gitlab/git-data/repositories/root/test.git/custom_hooks
```

