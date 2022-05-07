# Java Setting

## __1. Homebrew 설치__
- [Homebrew-Setting.md 참고](/Homebrew-Setting/Homebrew-Setting.md)


## __2. AdoptOpenjdk 설치__
```
https://github.com/AdoptOpenJDK/homebrew-openjdk
```

## __3. openjdk 저장소 설치__
```bash
brew tap AdoptOpenJDK/openjdk
```

<details marakdown="1">
<summary>console</summary>

```bash
Running `brew update --preinstall`...
==> Auto-updated Homebrew!
Updated 1 tap (homebrew/core).
==> Updated Formulae
Updated 1 formula.

==> Tapping adoptopenjdk/openjdk
Cloning into '/usr/local/Homebrew/Library/Taps/adoptopenjdk/homebrew-openjdk'...
remote: Enumerating objects: 1996, done.
remote: Counting objects: 100% (60/60), done.
remote: Compressing objects: 100% (21/21), done.
remote: Total 1996 (delta 44), reused 54 (delta 39), pack-reused 1936
Receiving objects: 100% (1996/1996), 372.55 KiB | 8.28 MiB/s, done.
Resolving deltas: 100% (1424/1424), done.
Tapped 47 casks (69 files, 522.1KB).
```
</details>
<br>

## __4. 설치할 자바 버전 확인__
|Java Version|	JDK	|JRE|
|:---:|:---:|:---:|
|Latest OpenJDK with Hotspot JVM	|adoptopenjdk	        |adoptopenjdk-jre
|Latest OpenJDK with OpenJ9 JVM	    |adoptopenjdk-openj9	|adoptopenjdk-openj9-jre
|OpenJDK8 with Hotspot JVM	        |adoptopenjdk8	        |adoptopenjdk8-jre
|OpenJDK8 with OpenJ9 JVM	        |adoptopenjdk8-openj9	|adoptopenjdk8-openj9-jre
|OpenJDK9 with Hotspot JVM	        |adoptopenjdk9	        |n/a
|OpenJDK10 with Hotspot JVM	        |adoptopenjdk10	        |n/a
|OpenJDK11 with Hotspot JVM	        |adoptopenjdk11	        |adoptopenjdk11-jre
|OpenJDK11 with OpenJ9 JVM	        |adoptopenjdk11-openj9	|adoptopenjdk11-openj9-jre
|OpenJDK12 with Hotspot JVM	        |adoptopenjdk12	        |adoptopenjdk12-jre
|OpenJDK12 with OpenJ9 JVM	        |adoptopenjdk12-openj9	|adoptopenjdk12-openj9-jre
|OpenJDK13 with Hotspot JVM	        |adoptopenjdk13     	|adoptopenjdk13-jre
|OpenJDK13 with OpenJ9 JVM	        |adoptopenjdk13-openj9	|adoptopenjdk13-openj9-jre
|OpenJDK14 with Hotspot JVM	        |adoptopenjdk14	        |adoptopenjdk14-jre
|OpenJDK14 with OpenJ9 JVM	        |adoptopenjdk14-openj9	|adoptopenjdk14-openj9-jre
|OpenJDK15 with Hotspot JVM	        |adoptopenjdk15	        |adoptopenjdk15-jre
|OpenJDK15 with OpenJ9 JVM	        |adoptopenjdk15-openj9	|adoptopenjdk15-openj9-jre
|OpenJDK16 with Hotspot JVM	        |adoptopenjdk16	        |adoptopenjdk16-jre
|OpenJDK16 with OpenJ9 JVM	        |adoptopenjdk16-openj9	|adoptopenjdk16-openj9-jr

## __5. openjdk 설치__
```bash
brew install --cask <version>
```

<details markdown="1">
<summary>console</summary>

```bash
==> Downloading https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jdk_x64_mac_hotspot_11.0.11_9.pkg
==> Downloading from https://objects.githubusercontent.com/github-production-release-asset-2e65be/140419044/15623b80-a2e2-11eb-89cd-bed191d70c46?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIWNJYAX4CSVEH53A%2F20220507%2Fus-east-1%2Fs3%2Faws4_r
######################################################################## 100.0%
==> Installing Cask adoptopenjdk11
==> Running installer for adoptopenjdk11; your password may be necessary.
Package installers may write to any location; options such as `--appdir` are ignored.
Password: <계정의 Password 입력>
installer: Package name is AdoptOpenJDK
installer: Installing at base path /
installer: The install was successful.
package-id: net.adoptopenjdk.11.jdk
version: 11.0.11+9
volume: /
location: 
install-time: 1651898674
🍺  adoptopenjdk11 was successfully installed!
```

</details>
<br>

## __6. 설치 확인__
- 입력
```bash
java --version
```
- 출력
```bash
openjdk 11.0.11 2021-04-20
OpenJDK Runtime Environment AdoptOpenJDK-11.0.11+9 (build 11.0.11+9)
OpenJDK 64-Bit Server VM AdoptOpenJDK-11.0.11+9 (build 11.0.11+9, mixed mode)
```
