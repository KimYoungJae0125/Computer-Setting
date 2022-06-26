## Redis Setting

### __1. Homebrew 설치__
> [Homebrew-Setting.md 참고](/Homebrew-Setting/Homebrew-Setting.md)

### __2. Reids 설치__
```shell
$ brew install redis
```

<details marakdown="1">
<summary>console</summary>

```shell
Running `brew update --auto-update`...
==> Auto-updated Homebrew!
Updated 1 tap (homebrew/core).
==> New Formulae
aztfy                      lexicon                    trzsz-go
evernote-backup            qbe

==> Downloading https://ghcr.io/v2/homebrew/core/redis/manifests/7.0.0
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/redis/blobs/sha256:05a9eddf3ed9
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sh
######################################################################## 100.0%
==> Pouring redis--7.0.0.monterey.bottle.tar.gz
==> Caveats
To restart redis after an upgrade:
  brew services restart redis
Or, if you don't want/need a background service you can just run:
  /usr/local/opt/redis/bin/redis-server /usr/local/etc/redis.conf
==> Summary
🍺  /usr/local/Cellar/redis/7.0.0: 14 files, 2.6MB
==> Running `brew cleanup redis`...
Disable this behaviour by setting HOMEBREW_NO_INSTALL_CLEANUP.
Hide these hints with HOMEBREW_NO_ENV_HINTS (see `man brew`).

```

</details>

### __3. Redis 서비스 실행, 중지, 재실행__
#### - 레디스 실행
```shell
$ brew services start redis
```
#### - 레디스 중지
```shell
$ brew services stop redis
```
#### - 레디스 재실행
```shell
$ brew services restart redis
```

> ### __Redis Server 확인__
> ```shell
> $ redis-server
> ```
> <details marakdown="1">
> <summary>console</summary>
> 
> ```shell
> 2315:C 26 Jun 2022 13:22:38.668 # oO0OoO0OoO0Oo Redis is starting oO0OoO0OoO0Oo
> 2315:C 26 Jun 2022 13:22:38.668 # Redis version=7.0.0, bits=64, commit=00000000, modified=0, pid=2315, just started
> 2315:C 26 Jun 2022 13:22:38.668 # Warning: no config file specified, using the default config. In order to specify a config file use redis-server /path/to/redis.conf
> 2315:M 26 Jun 2022 13:22:38.669 * Increased maximum number of open files to 10032 (it was originally set to 256).
> 2315:M 26 Jun 2022 13:22:38.669 * monotonic clock: POSIX clock_gettime
>                 _._                                                  
>            _.-``__ ''-._                                             
>       _.-``    `.  `_.  ''-._           Redis 7.0.0 (00000000/0) 64 bit
>   .-`` .-```.  ```\/    _.,_ ''-._                                  
> (    '      ,       .-`  | `,    )     Running in standalone mode
> |`-._`-...-` __...-.``-._|'` _.-'|     Port: 6379
> |    `-._   `._    /     _.-'    |     PID: 0000
>   `-._    `-._  `-./  _.-'    _.-'                                   
> |`-._`-._    `-.__.-'    _.-'_.-'|                                  
> |    `-._`-._        _.-'_.-'    |           https://redis.io       
> `-._    `-._`-.__.-'_.-'    _.-'                                   
> |`-._`-._    `-.__.-'    _.-'_.-'|                                  
> |    `-._`-._        _.-'_.-'    |                                  
> `-._    `-._`-.__.-'_.-'    _.-'                                   
>       `-._    `-.__.-'    _.-'                                       
>           `-._        _.-'                                           
>               `-.__.-'                                               
>
> 2315:M 26 Jun 2022 13:22:38.670 # WARNING: The TCP backlog setting of 511 cannot be enforced because kern.ipc.somaxconn is set to the lower value of 128.
> 2315:M 26 Jun 2022 13:22:38.670 # Server initialized
> 2315:M 26 Jun 2022 13:22:38.671 * The AOF directory appendonlydir doesn't exist
> 2315:M 26 Jun 2022 13:22:38.671 * Ready to accept connections
> ```
>
> </details>

> ### __Redis Client 확인__
> ```shell
> $ redis-cli
> ```
> ```shell
> 127.0.0.1:6379> <Redis 명령어 입력>
> ```

> ### __Redis 비밀번호 설정__
> 1. ```redis.conf```가 있는 폴더 위치로 이동
> ```shell
> 위치를 모를 경우 최상위 프로세스에서 파일 찾기
> $ find . -name "redis.conf"
> ```
> ```shell
> ./usr/local/etc/redis.conf
> ```
> - 필자의 컴퓨터에는 위의 경로로 파일이 나온다.
> - 여기서 ```cd usr/local/etc```까지만 입력하여 해당 폴더 위치로 이동한다.
> 2. ```redis.conf``` 열기
> ```shell
> $ vi redis.conf
> ```
> ```shell
> ################################## SECURITY ###################################
>
> # Warning: since Redis is pretty fast, an outside user can try up to
> # 1 million passwords per second against a modern box. This means that you
> # should use very strong passwords, otherwise they will be very easy to break.
> # Note that because the password is really a shared secret between the client
> # and the server, and should not be memorized by any human, the password
> # can be easily a long string from /dev/urandom or whatever, so by using a
> # long and unguessable password no brute force attack will be possible.
> ... 생략
> # requirepass foobared //기본 세팅
> ```
> - 설정 파일을 수정하려고 들어가면 많은 텍스트가 있는데 쭉쭉 내려가다가 ```SECURITY``` 부분을 찾는다.
> - ```SECURITY```부분에서 조금 더 찾다보면 ```requirepass``` 부분이 있는데 이 부분은 주석처리 되어있고 기본적으로 ```foobard```라는 비밀번호가 입력되어있다.
> - 주석을 해제하고 원하는 비밀번호를 입력하자.
> - __입력 방법__
>   - ```i```를 누를 시 왼쪽 하단에 ```--- INSERT ---```가 뜬다. 그러면 입력 모드로 바뀐것이다.
> ```shell
> ################################## SECURITY ###################################
>
> # Warning: since Redis is pretty fast, an outside user can try up to
> # 1 million passwords per second against a modern box. This means that you
> # should use very strong passwords, otherwise they will be very easy to break.
> # Note that because the password is really a shared secret between the client
> # and the server, and should not be memorized by any human, the password
> # can be easily a long string from /dev/urandom or whatever, so by using a
> # long and unguessable password no brute force attack will be possible.
> ... 생략
> requirepass 1234
> ```
> - __입력 후 저장방법__
> - 다 입력을 하였으면 ```ESC```버튼을 누른다. 그러면 ```--- INSERT ---```가 사라지고 ```:```가 뜬다.
> - ```wq```입력 후 ```Enter```를 누르면 저장이 된다.
> 3. Redis 재실행
> - ```$ brew services restart redis```명령어를 이용해 Redis를 재 실행하고 비밀번호를 입력하지 않고 ```redis-cli```를 접속한 후 테스트로 ```ping```을 입력하면 ```(error) NOAUTH Authentication required.``` 라는 문구가 뜬다.
> - 바뀐 비밀번호를 이용하여 접속을 하려면 ```redis-cli -a <비밀번호>```로 접속하면 문제없이 사용 가능하다.