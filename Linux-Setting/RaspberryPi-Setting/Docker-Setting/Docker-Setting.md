## 도커 세팅

### 1. Update & Upgrade System

### 2. 도커 설치
```shell
$ curl -fsSL https://get.docker.com -o get-docker.sh
```
- 다운로드 받은 sh 파일 실행
```shell
$ sudo sh get-docker.sh
```

<details>

<summary>console</summary>

```shell
# Executing docker install script, commit: b2e29ef7a9a89840d2333637f7d1900a83e71
53f
+ sh -c apt-get update -qq >/dev/null
+ sh -c DEBIAN_FRONTEND=noninteractive apt-get install -y -qq apt-transport-http
  s ca-certificates curl >/dev/null
+ sh -c mkdir -p /etc/apt/keyrings && chmod -R 0755 /etc/apt/keyrings
+ sh -c curl -fsSL "https://download.docker.com/linux/debian/gpg" | gpg --dearmo
  r --yes -o /etc/apt/keyrings/docker.gpg
+ sh -c chmod a+r /etc/apt/keyrings/docker.gpg
+ sh -c echo "deb [arch=arm64 signed-by=/etc/apt/keyrings/docker.gpg] https://do
  wnload.docker.com/linux/debian bullseye stable" > /etc/apt/sources.list.d/docker
  .list
+ sh -c apt-get update -qq >/dev/null
+ sh -c DEBIAN_FRONTEND=noninteractive apt-get install -y -qq --no-install-recom
  mends docker-ce docker-ce-cli containerd.io docker-compose-plugin >/dev/null
+ version_gte 20.10
+ [ -z  ]
+ return 0
+ sh -c DEBIAN_FRONTEND=noninteractive apt-get install -y -qq docker-ce-rootless
  -extras >/dev/null
+ sh -c docker version
  Client: Docker Engine - Community
  Version:           20.10.17
  API version:       1.41
  Go version:        go1.17.11
  Git commit:        100c701
  Built:             Mon Jun  6 23:02:34 2022
  OS/Arch:           linux/arm64
  Context:           default
  Experimental:      true

Server: Docker Engine - Community
Engine:
Version:          20.10.17
API version:      1.41 (minimum version 1.12)
Go version:       go1.17.11
Git commit:       a89b842
Built:            Mon Jun  6 23:01:01 2022
OS/Arch:          linux/arm64
Experimental:     false
containerd:
Version:          1.6.7
GitCommit:        0197261a30bf81f1ee8e6a4dd2dea0ef95d67ccb
runc:
Version:          1.1.3
GitCommit:        v1.1.3-0-g6724737
docker-init:
Version:          0.19.0
GitCommit:        de40ad0

================================================================================

To run Docker as a non-privileged user, consider setting up the
Docker daemon in rootless mode for your user:

    dockerd-rootless-setuptool.sh install

Visit https://docs.docker.com/go/rootless/ to learn about rootless mode.


To run the Docker daemon as a fully privileged service, but granting non-root
users access, refer to https://docs.docker.com/go/daemon-access/

WARNING: Access to the remote API on a privileged Docker daemon is equivalent
to root access on the host. Refer to the 'Docker daemon attack surface'
documentation for details: https://docs.docker.com/go/attack-surface/

================================================================================
```

</details>

### 3. 비루트 계정 권한 설정
```shell
$ sudo usermod -aG docker ${User}
```
- ${User} = 라즈베리 파이 로그인 시 계정명

#### 3-1. 확인
```shell
$ groups ${User}
```

<details>
<summary>console</summary>

```shell
${User} : ${User} adm dialout cdrom sudo audio plugdev games users input netdev spi i2c gpio lpadmin docker
```

### 3-2. 재부팅
```shell
$ reboot
```
- 권한 추가시 로그아웃 혹은 시스템을 재시작해야지 적용 된다.


</details>

### 4. 설치 확인
```shell
$ docker version
```
- 만약 permission denied 가 나올 경우 위에 권한 설정이 안 된것이므로 권한 설정을 해주거나 ```sudo```를 앞에 붙인다.

### 5. 부팅 시 도커 자동 실행
```shell
$ sudo systemctl enable docker
```