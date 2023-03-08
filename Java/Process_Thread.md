## 프로세스
* 실행되고 있는 프로그램의 개체

```
CPU 시간이나 메모리 등 시스템 자원이 할당되는 독립적인 개체.
다른 프로세스와 상관 없이 독립적으로 자원을 할당 받음.
프로세스 간의 통신을 위해선 파이프, 파일, 소켓 등을 사용하여 통신하여야 함. 
```

## 쓰레드
* 프로세스 안에 존재하여, 프로세스의 자원을 공유하는 개체

```
흔히 경량 프로세스라고 부르는데, 각 쓰레드는 별도의 레지스터와 스택을 가지고, 힙 영역은 공유함.
```