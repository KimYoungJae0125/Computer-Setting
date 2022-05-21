# Java Setting

## __1. Homebrew 설치__
> [Homebrew-Setting.md 참고](/Homebrew-Setting/Homebrew-Setting.md)

<br>

## __2. Gradle 설치__
```bash
$ brew install gradle
```
```bash
Running `brew update --preinstall`...
==> Auto-updated Homebrew!
Updated 2 taps (homebrew/core and homebrew/services).
==> New Formulae
bore-cli               dotdrop                flix                   git-workspace          goctl                  libabw                 lndir                  octosql                release-it             sftpgo                 ttmath
dbml-cli               erlang@24              gcc@12                 glibc@2.13             helmify                libxcvt                mbt                    pget                   sdl2_sound             tradcpp                xcode-kotlin
==> Updated Formulae
Updated 798 formulae.

==> Downloading https://ghcr.io/v2/homebrew/core/openjdk/manifests/18.0.1
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/openjdk/blobs/sha256:acb7d100bd61aa51fd0014339897dc8b6405f5c62adf8551cbffe28c1ce6aac7
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sha256:acb7d100bd61aa51fd0014339897dc8b6405f5c62adf8551cbffe28c1ce6aac7?se=2022-05-21T13%3A50%3A00Z&sig=eo4Le21wSYS%2F%2BBdYJpBmtReuxyfW1S97PrG%2F5tf%2FhTQ%3D&sp=r&spr=https&
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/gradle/manifests/7.4.2
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/gradle/blobs/sha256:36f1f1e0d0f96a0e55c67b6938cf1ae170b59a280e2e9839533538e5b575d287
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sha256:36f1f1e0d0f96a0e55c67b6938cf1ae170b59a280e2e9839533538e5b575d287?se=2022-05-21T13%3A50%3A00Z&sig=OGO%2FNkKfNF3jrZA5iDgkSu4JHkwYFWQzFxRK4dvUXNM%3D&sp=r&spr=https&sr=b&s
######################################################################## 100.0%
==> Installing dependencies for gradle: openjdk
==> Installing gradle dependency: openjdk
==> Pouring openjdk--18.0.1.monterey.bottle.tar.gz
🍺  /usr/local/Cellar/openjdk/18.0.1: 641 files, 307.7MB
==> Installing gradle
==> Pouring gradle--7.4.2.all.bottle.tar.gz
🍺  /usr/local/Cellar/gradle/7.4.2: 11,257 files, 267.8MB
==> Running `brew cleanup gradle`...
Disable this behaviour by setting HOMEBREW_NO_INSTALL_CLEANUP.
Hide these hints with HOMEBREW_NO_ENV_HINTS (see `man brew`).
```
<br>

## __3. 설치된 버전 확인__
```bash
$ gradle -v
```
```bash
Welcome to Gradle 7.4.2!

Here are the highlights of this release:
 - Aggregated test and JaCoCo reports
 - Marking additional test source directories as tests in IntelliJ
 - Support for Adoptium JDKs in Java toolchains

For more details see https://docs.gradle.org/7.4.2/release-notes.html


------------------------------------------------------------
Gradle 7.4.2
------------------------------------------------------------

Build time:   2022-03-31 15:25:29 UTC
Revision:     540473b8118064efcc264694cbcaa4b677f61041

Kotlin:       1.5.31
Groovy:       3.0.9
Ant:          Apache Ant(TM) version 1.10.11 compiled on July 10 2021
JVM:          18.0.1 (Homebrew 18.0.1+0)
OS:           
```