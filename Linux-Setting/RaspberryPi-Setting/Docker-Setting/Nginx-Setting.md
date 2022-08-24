## NginX 설치

```shell
$ docker pull nginx:alpine
```

<details>

<summary>console</summary>

```shell
alpine: Pulling from library/nginx
9b18e9b68314: Pull complete 
51048c2d0108: Pull complete 
3897c47760f3: Pull complete 
f61a6b717778: Pull complete 
56ed090e0ec8: Pull complete 
e5a0a61a0146: Pull complete 
Digest: sha256:082f8c10bd47b6acc8ef15ae61ae45dd8fde0e9f389a8b5cb23c37408642bf5d
Status: Downloaded newer image for nginx:alpine
docker.io/library/nginx:alpine
```

</details>

```shell
$ docker run -it -p 80:80 nginx:alpine
```

<details>
<summary>console</summary>

```shell
/docker-entrypoint.sh: /docker-entrypoint.d/ is not empty, will attempt to perform configuration
/docker-entrypoint.sh: Looking for shell scripts in /docker-entrypoint.d/
/docker-entrypoint.sh: Launching /docker-entrypoint.d/10-listen-on-ipv6-by-default.sh
10-listen-on-ipv6-by-default.sh: info: Getting the checksum of /etc/nginx/conf.d/default.conf
10-listen-on-ipv6-by-default.sh: info: Enabled listen on IPv6 in /etc/nginx/conf.d/default.conf
/docker-entrypoint.sh: Launching /docker-entrypoint.d/20-envsubst-on-templates.sh
/docker-entrypoint.sh: Launching /docker-entrypoint.d/30-tune-worker-processes.sh
/docker-entrypoint.sh: Configuration complete; ready for start up
2022/08/18 14:22:36 [notice] 1#1: using the "epoll" event method
2022/08/18 14:22:36 [notice] 1#1: nginx/1.23.1
2022/08/18 14:22:36 [notice] 1#1: built by gcc 11.2.1 20220219 (Alpine 11.2.1_git20220219) 
2022/08/18 14:22:36 [notice] 1#1: OS: Linux 5.15.56-v8+
2022/08/18 14:22:36 [notice] 1#1: getrlimit(RLIMIT_NOFILE): 1048576:1048576
2022/08/18 14:22:36 [notice] 1#1: start worker processes
2022/08/18 14:22:36 [notice] 1#1: start worker process 32
2022/08/18 14:22:36 [notice] 1#1: start worker process 33
2022/08/18 14:22:36 [notice] 1#1: start worker process 34
2022/08/18 14:22:36 [notice] 1#1: start worker process 35


```

</details>