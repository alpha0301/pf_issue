# Heap Dump

```
jmap -dump:format=b,file={file path} {java PID}
```

윈도우 서비스로 실행중인 java의 heap dump는 PsExec 를 통해 실행해야 함
- [PsExec](https://docs.microsoft.com/en-us/sysinternals/downloads/psexec)

```
PsExec.exe -s "{JAVA_HOME}/bin/jmap.exe" -dump:format=b,file={file path} {java PID}
```

# Thread Dump

```
jstack {java PID} > {file path}
```
