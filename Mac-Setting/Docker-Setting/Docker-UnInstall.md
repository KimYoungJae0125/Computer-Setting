# Docker-UnInstall

## 1. 도커 삭제 스크립트 설치
```shell
$ curl -O https://raw.githubusercontent.com/docker/toolbox/master/osx/uninstall.sh
```

<details>

<summary>console</summary>

```shell
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100   879  100   879    0     0   1948      0 --:--:-- --:--:-- --:--:--  1979
```

</details>

## 2. 삭제 스크립트 권한 주기
```shell
$ chmod +x uninstall.sh
```

## 3. 삭제 스크립트 실행
```shell
$ sudo ./uninstall.sh
```

```shell
Password: {컴퓨터 비밀번호}
Remove all Docker Machine VMs? (Y/N): Y
```

<details>

<summary>console</summary>

```shell
./uninstall.sh: line 13: docker-machine: command not found
./uninstall.sh: line 13: docker-machine: command not found
Removing Applications...
Removing docker binaries...
rm: /usr/local/bin/docker-machine-driver*: No such file or directory
Removing boot2docker.iso
Forget packages
No receipt for 'io.docker.pkg.docker' found at '/'.
No receipt for 'io.docker.pkg.dockercompose' found at '/'.
No receipt for 'io.docker.pkg.dockermachine' found at '/'.
No receipt for 'io.boot2dockeriso.pkg.boot2dockeriso' found at '/'.
All Done!
```

</details>
