# java performance tuning


## 1 jvm arg
-Xms
-Xmx



## 2 cmd to check java proces status
jps -lmv
jstack \<pid>
jinfo \<pid>
jinfo -flags \<pid>
jinfo -sysprops \<pid>
jmap -heap \<pid>
jstat -gctuil \<pid> 1000




