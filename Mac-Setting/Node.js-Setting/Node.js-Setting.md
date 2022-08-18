## Node.js Setting

### __1. Homebrew 설치__
> [Homebrew-Setting.md 참고](/Mac-Setting/Homebrew-Setting/Homebrew-Setting.md)

<br>

### __2. node/npm 설치__
> node 및 npm(node package manger) 설치
```shell
$ brew install node
```

<details>
<summary> console </summary>

```shell
==> Downloading https://ghcr.io/v2/homebrew/core/brotli/manifests/1.0.9
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/brotli/blobs/sha256:985ce69f1ae
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sh
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/c-ares/manifests/1.18.1_1
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/c-ares/blobs/sha256:62b9590a3b9
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sh
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/icu4c/manifests/70.1
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/icu4c/blobs/sha256:321592eb1aeb
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sh
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/libnghttp2/manifests/1.48.0
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/libnghttp2/blobs/sha256:f0e1cb4
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sh
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/libuv/manifests/1.44.2
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/libuv/blobs/sha256:395adc3a60c3
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sh
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/ca-certificates/manifests/2022-
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/ca-certificates/blobs/sha256:9e
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sh
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/openssl/1.1/manifests/1.1.1q
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/openssl/1.1/blobs/sha256:b4dabe
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sh
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/node/manifests/18.7.0
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/node/blobs/sha256:cbcfe985fe9bd
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sh
######################################################################## 100.0%
==> Installing dependencies for node: brotli, c-ares, icu4c, libnghttp2, libuv, ca-certificates and openssl@1.1
==> Installing node dependency: brotli
==> Pouring brotli--1.0.9.monterey.bottle.tar.gz
🍺  /usr/local/Cellar/brotli/1.0.9: 25 files, 2.3MB
==> Installing node dependency: c-ares
==> Pouring c-ares--1.18.1_1.monterey.bottle.tar.gz
🍺  /usr/local/Cellar/c-ares/1.18.1_1: 87 files, 645.3KB
==> Installing node dependency: icu4c
==> Pouring icu4c--70.1.monterey.bottle.tar.gz
🍺  /usr/local/Cellar/icu4c/70.1: 261 files, 74.4MB
==> Installing node dependency: libnghttp2
==> Pouring libnghttp2--1.48.0.monterey.bottle.tar.gz
🍺  /usr/local/Cellar/libnghttp2/1.48.0: 13 files, 739.8KB
==> Installing node dependency: libuv
==> Pouring libuv--1.44.2.monterey.bottle.tar.gz
🍺  /usr/local/Cellar/libuv/1.44.2: 50 files, 3.5MB
==> Installing node dependency: ca-certificates
==> Pouring ca-certificates--2022-07-19_1.all.bottle.tar.gz
==> Regenerating CA certificate bundle from keychain, this may take a while...
🍺  /usr/local/Cellar/ca-certificates/2022-07-19_1: 3 files, 222.7KB
==> Installing node dependency: openssl@1.1
==> Pouring openssl@1.1--1.1.1q.monterey.bottle.tar.gz
🍺  /usr/local/Cellar/openssl@1.1/1.1.1q: 8,097 files, 18.5MB
==> Installing node
==> Pouring node--18.7.0.monterey.bottle.tar.gz
🍺  /usr/local/Cellar/node/18.7.0: 1,934 files, 49.3MB
==> Running `brew cleanup node`...
Disable this behaviour by setting HOMEBREW_NO_INSTALL_CLEANUP.
Hide these hints with HOMEBREW_NO_ENV_HINTS (see `man brew`).
==> Upgrading 2 dependents of upgraded formulae:
Disable this behaviour by setting HOMEBREW_NO_INSTALLED_DEPENDENTS_CHECK.
Hide these hints with HOMEBREW_NO_ENV_HINTS (see `man brew`).
groonga 12.0.4 -> 12.0.5, redis 7.0.0 -> 7.0.4
==> Downloading https://ghcr.io/v2/homebrew/core/groonga/manifests/12.0.5
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/groonga/blobs/sha256:9495982a54
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sh
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/redis/manifests/7.0.4
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/redis/blobs/sha256:58f58d9fe070
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sh
######################################################################## 100.0%
==> Upgrading groonga
  12.0.4 -> 12.0.5 

==> Pouring groonga--12.0.5.monterey.bottle.tar.gz
🍺  /usr/local/Cellar/groonga/12.0.5: 986 files, 80.9MB
==> Running `brew cleanup groonga`...
Removing: /usr/local/Cellar/groonga/12.0.4... (985 files, 80.6MB)
==> Upgrading redis
  7.0.0 -> 7.0.4 

==> Pouring redis--7.0.4.monterey.bottle.tar.gz
==> Caveats
To restart redis after an upgrade:
  brew services restart redis
Or, if you don't want/need a background service you can just run:
  /usr/local/opt/redis/bin/redis-server /usr/local/etc/redis.conf
==> Summary
🍺  /usr/local/Cellar/redis/7.0.4: 14 files, 2.6MB
==> Running `brew cleanup redis`...
Removing: /usr/local/Cellar/redis/7.0.0... (14 files, 2.6MB)
==> Checking for dependents of upgraded formulae...
==> No broken dependents found!
==> Caveats
==> redis
To restart redis after an upgrade:
  brew services restart redis
Or, if you don't want/need a background service you can just run:
  /usr/local/opt/redis/bin/redis-server /usr/local/etc/redis.conf
```

</details>

<br>

### __3. node/npm 설치 확인__
```shell
$ node -v

v18.7.0
```
```shell
$ npm -v

8.15.0
```
