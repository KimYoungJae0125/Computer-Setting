## 젠킨스 세팅

### 1. 도커에서 젠킨스 설치

```shell
$ docker pull jenkins/jenkins:lts
```

<details>
<summary>console</summary>

```shell
lts: Pulling from jenkins/jenkins
114ba63dd73a: Pull complete 
67df9da03ba5: Pull complete 
768bbc28af1b: Pull complete 
c9848ef3503d: Pull complete 
744ab7514e5e: Pull complete 
b94a49221990: Pull complete 
131a972b7f42: Pull complete 
b9746bcd8970: Pull complete 
a39bc14d8488: Pull complete 
aa2aea773eda: Pull complete 
869ecf8171e3: Pull complete 
3e121cb2ce0b: Pull complete 
b2edffe864c9: Pull complete 
4a111bd1d49e: Pull complete 
Digest: sha256:cc62444630fb4b7c4694ac6b11b68dc64864a67fd98121194f913027733c9dce
Status: Downloaded newer image for jenkins/jenkins:lts
docker.io/jenkins/jenkins:lts

```

</details>

#### 2. 도커에서 젠킨스 실행

```shell
$ docker run -itd -p 8085:8080 -v /jenkins:/var/jenkins_home --name jenkins -u root jenkins/jenkins:lts
```

#### 3. 젠킨스 접속

```shell
${Ip}:${port}
```
- 내부에서 접속 시 ```localhost:${port}```로 들어가면 됨
- 위의 컨테이너 정보로 예시를 들자면 ```localhost:8085```

### 4. Jenkins 비밀번호 확인

```shell
$ docker exec -it jenkins /bin/bash
```
```shell
$ cat /var/jenkins_home/secrets/initialAdminPassword
```

### 5. 젠킨스 권한 주기
```shell
$ cd .. //최상위 폴더로 이동
$ cd etc
$ sudo vi sudoers
```
```shell
# Allow members of group sudo to execute any command
%sudo   ALL=(ALL:ALL) ALL
jenkins ALL=(ALL) NOPASSWD: ALL //추가

```