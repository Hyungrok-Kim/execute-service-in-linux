# execute-jar service-in-Linux

> 백그라운드에서 실행(프로그램을 데몬처럼 실행하고 싶은 경우) **명령어 "&"**
```java
java -jar ~.jar &
```

> nohup파일에 서비스 로그 남기기 
```java
nohup java -jar ~.jar &
```

> 프로세스 안전하게 종료시키기 
```java
ps -ef | grep .jar -> .jar 파일 PID 확인
kill term -term PID || kill term -INT PID || kill -2 PID
```

> 프로세스 강제 종료시키기 (비권장)
```java
kill -kill PID || kill -9 PID
```
