# MariaDB Setting

## __1. Homebrew 설치__
> [Homebrew-Setting.md 참고](/Homebrew-Setting/Homebrew-Setting.md)

<br>

## __2. 참고 사이트__
> https://mariadb.com/kb/ko/installing-mariadb-on-macos-using-homebrew/

<br>

## __3. MariaDB 설치__
```bash
$ brew install mariadb
```

<details marakdown="1">
<summary>console</summary>

```bash
Running `brew update --preinstall`...
==> Auto-updated Homebrew!
Updated 1 tap (homebrew/core).
==> Updated Formulae
Updated 6 formulae.

==> Downloading https://ghcr.io/v2/homebrew/core/mecab/manifests/0.996-3
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/mecab/blobs/sha256:839a67ae318170dea1c0ea8f3e55d8c5291da3e77ad0d62491fa656cf5539a18
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sha256:839a67ae318170dea1c0ea8f3e55d8c5291da3e77ad0d62491fa656cf5539a18?se=2022-05-07T07%3A10%3A00
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/mecab-ipadic/manifests/2.7.0-20070801
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/mecab-ipadic/blobs/sha256:fd42086389a7302de36628435004c2f8de2f55b01f6fd8b5a74529779fc2754a
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sha256:fd42086389a7302de36628435004c2f8de2f55b01f6fd8b5a74529779fc2754a?se=2022-05-07T07%3A10%3A00
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/msgpack/manifests/4.0.0
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/msgpack/blobs/sha256:c457413b910943f87cffc03951d9dbe5cc60c23abf862c572dab0b18011bb682
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sha256:c457413b910943f87cffc03951d9dbe5cc60c23abf862c572dab0b18011bb682?se=2022-05-07T07%3A10%3A00
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/ca-certificates/manifests/2022-04-26
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/ca-certificates/blobs/sha256:c05a44feba2a630de2e1cefba90d3aa3f74e4d57146c0117858f648c419abeae
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sha256:c05a44feba2a630de2e1cefba90d3aa3f74e4d57146c0117858f648c419abeae?se=2022-05-07T07%3A10%3A00
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/openssl/1.1/manifests/1.1.1n
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/openssl/1.1/blobs/sha256:b22f50654fe0262e81493dfd38e18d2f146317c78198bea1a0c3c7c2f0dc983c
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sha256:b22f50654fe0262e81493dfd38e18d2f146317c78198bea1a0c3c7c2f0dc983c?se=2022-05-07T07%3A10%3A00
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/pcre/manifests/8.45
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/pcre/blobs/sha256:5e5cc7a5bf8bb6488ec57d4263bf6b0bc89e93252a0a2460f846de29373162d8
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sha256:5e5cc7a5bf8bb6488ec57d4263bf6b0bc89e93252a0a2460f846de29373162d8?se=2022-05-07T07%3A10%3A00
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/groonga/manifests/12.0.3
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/groonga/blobs/sha256:4c3a4c62f4192a784129846e98568da27957fbb4858bc9b3c445a940342fb752
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sha256:4c3a4c62f4192a784129846e98568da27957fbb4858bc9b3c445a940342fb752?se=2022-05-07T07%3A10%3A00
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/zstd/manifests/1.5.2-2
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/zstd/blobs/sha256:3cd1dc42736c2873b0684f0da4ffe3e9fdac30ec9ed5b4c0f9f657bc0d5c3f50
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sha256:3cd1dc42736c2873b0684f0da4ffe3e9fdac30ec9ed5b4c0f9f657bc0d5c3f50?se=2022-05-07T07%3A10%3A00
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/mariadb/manifests/10.7.3
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/mariadb/blobs/sha256:439378c9adf87ed440d543882a0a6aafdbe089e2bcc1af7225069a08ffc34782
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sha256:439378c9adf87ed440d543882a0a6aafdbe089e2bcc1af7225069a08ffc34782?se=2022-05-07T07%3A10%3A00
######################################################################## 100.0%
==> Installing dependencies for mariadb: mecab, mecab-ipadic, msgpack, ca-certificates, openssl@1.1, pcre, groonga and zstd
==> Installing mariadb dependency: mecab
==> Pouring mecab--0.996.monterey.bottle.3.tar.gz
🍺  /usr/local/Cellar/mecab/0.996: 18 files, 4.4MB
==> Installing mariadb dependency: mecab-ipadic
==> Pouring mecab-ipadic--2.7.0-20070801.monterey.bottle.tar.gz
🍺  /usr/local/Cellar/mecab-ipadic/2.7.0-20070801: 14 files, 50.6MB
==> Installing mariadb dependency: msgpack
==> Pouring msgpack--4.0.0.monterey.bottle.tar.gz
🍺  /usr/local/Cellar/msgpack/4.0.0: 35 files, 200.5KB
==> Installing mariadb dependency: ca-certificates
==> Pouring ca-certificates--2022-04-26.all.bottle.tar.gz
==> Regenerating CA certificate bundle from keychain, this may take a while...
🍺  /usr/local/Cellar/ca-certificates/2022-04-26: 3 files, 215.6KB
==> Installing mariadb dependency: openssl@1.1
==> Pouring openssl@1.1--1.1.1n.monterey.bottle.tar.gz
🍺  /usr/local/Cellar/openssl@1.1/1.1.1n: 8,089 files, 18.5MB
==> Installing mariadb dependency: pcre
==> Pouring pcre--8.45.monterey.bottle.tar.gz
🍺  /usr/local/Cellar/pcre/8.45: 204 files, 5.7MB
==> Installing mariadb dependency: groonga
==> Pouring groonga--12.0.3.monterey.bottle.tar.gz
🍺  /usr/local/Cellar/groonga/12.0.3: 985 files, 80.6MB
==> Installing mariadb dependency: zstd
==> Pouring zstd--1.5.2.monterey.bottle.2.tar.gz
🍺  /usr/local/Cellar/zstd/1.5.2: 31 files, 2.4MB
==> Installing mariadb
==> Pouring mariadb--10.7.3.monterey.bottle.tar.gz
==> /usr/local/Cellar/mariadb/10.7.3/bin/mysql_install_db --verbose --user=kyj --basedir=/usr/local/Cellar/mariadb/10.7.3 --datadir=/usr/local/var/mysql --tmpdir=/tmp
==> Caveats
A "/etc/my.cnf" from another install may interfere with a Homebrew-built
server starting up correctly.

MySQL is configured to only allow connections from localhost by default

To restart mariadb after an upgrade:
  brew services restart mariadb
Or, if you don't want/need a background service you can just run:
  /usr/local/opt/mariadb/bin/mysqld_safe --datadir=/usr/local/var/mysql
==> Summary
🍺  /usr/local/Cellar/mariadb/10.7.3: 914 files, 186.8MB
==> Running `brew cleanup mariadb`...
Disable this behaviour by setting HOMEBREW_NO_INSTALL_CLEANUP.
Hide these hints with HOMEBREW_NO_ENV_HINTS (see `man brew`).
==> Caveats
==> mariadb
A "/etc/my.cnf" from another install may interfere with a Homebrew-built
server starting up correctly.

MySQL is configured to only allow connections from localhost by default

To restart mariadb after an upgrade:
  brew services restart mariadb
Or, if you don't want/need a background service you can just run:
  /usr/local/opt/mariadb/bin/mysqld_safe --datadir=/usr/local/var/mysql
  ```
</details>

<br>

## __4. mariaDB 시작__
```bash
$ brew services start mariadb
```

<details markdown="1">
<summary>console</summary>

```bash
==> Tapping homebrew/services
Cloning into '/usr/local/Homebrew/Library/Taps/homebrew/homebrew-services'...
remote: Enumerating objects: 1996, done.
remote: Counting objects: 100% (505/505), done.
remote: Compressing objects: 100% (169/169), done.
remote: Total 1996 (delta 342), reused 444 (delta 328), pack-reused 1491
Receiving objects: 100% (1996/1996), 547.76 KiB | 11.18 MiB/s, done.
Resolving deltas: 100% (897/897), done.
Tapped 1 command (45 files, 699.6KB).
==> Successfully started `mariadb` (label: homebrew.mxcl.mariadb)
```

</details>

<br>

## __5. database 세팅__
- Root 계정 로그인
```bash
$ sudo mysql -u root -p
$ Password: <'컴퓨터 비밀번호'>
```
- DataBase 만들기
```bash
$ create database <DB명>;
```
- DataBase 확인
```bash
$ show databases;
```
- 계정 생성
```bash
$ create user <'유저명'>@<'host주소'['localhost' 또는 '%(외부 접근 가능)']> identified by <'비밀번호'>;
```
- 권한 부여
```bash
$ grant <권한> on <DB명>.<테이블명> to <'유저명'>@<'host주소'>
```

> ### 참고) MariaDB 삭제
> 1. 설치 확인
> ```shell
> $ brew services list
> ```
> 2. MariaDB 가동 중단
> ```shell
> $ brew services stop mariadb
> ```
> 3. 삭제하기
> ```shell
> $ brew uninstall mariadb
> ```