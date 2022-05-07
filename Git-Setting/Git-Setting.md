# Mac에서 Git 세팅

## __1. Homebrew 설치__
- [Homebrew-Setting.md 참고](/Homebrew-Setting/Homebrew-Setting.md)

## __2. Homebrew를 이용하여 Git 설치__
### __2-1. Git Install__
- 입력
```bash
brew install git
```
<details markdown="1">
<summary>출력</summary>

```
Running `brew update --preinstall`...
==> Homebrew is run entirely by unpaid volunteers. Please consider donating:
  https://github.com/Homebrew/brew#donations
==> Auto-updated Homebrew!
Updated 1 tap (homebrew/core).
==> Updated Formulae
Updated 13 formulae.

==> Downloading https://ghcr.io/v2/homebrew/core/gettext/manifests/0.21
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/gettext/blobs/sha256:0e93b5264879cd5ece6efb644fd6320b0b96cce36de3901c1926e53f851d14c7
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sha256:0e93b5264879cd5ece6efb644fd6320b0b96cce36de3901c1926e53f851d14c7?se=2022-05-07T03%3A40%3A00Z&sig=UZTJUFoGaFsFVSfgeWOPJUzZfcAZ%2BDn2rCRQAlv0neQ%3D&sp=r&spr=https&sr=b&s
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/pcre2/manifests/10.40
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/pcre2/blobs/sha256:3d2707e8d5a80e1a28875e3b9c7b47cebaf5fd420049d6f1a72fa933b0e68339
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sha256:3d2707e8d5a80e1a28875e3b9c7b47cebaf5fd420049d6f1a72fa933b0e68339?se=2022-05-07T03%3A40%3A00Z&sig=T0DbKIh37vCI%2BOsxrSfZSWQ%2FH%2Fw2OIPzLTy1uR9HGWM%3D&sp=r&spr=https&sr
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/git/manifests/2.36.1
######################################################################## 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/git/blobs/sha256:ab1bc7b6fe710217007d10792425733c09e97d97f1aa3a3b1590038a9d9f4187
==> Downloading from https://pkg-containers.githubusercontent.com/ghcr1/blobs/sha256:ab1bc7b6fe710217007d10792425733c09e97d97f1aa3a3b1590038a9d9f4187?se=2022-05-07T03%3A40%3A00Z&sig=11VEeZ8dKbkoM3CuqdzAAYxbt8OHDQQGmfnSuaDkKps%3D&sp=r&spr=https&sr=b&sv=
######################################################################## 100.0%
==> Installing dependencies for git: gettext and pcre2
==> Installing git dependency: gettext
==> Pouring gettext--0.21.monterey.bottle.tar.gz
🍺  /usr/local/Cellar/gettext/0.21: 1,953 files, 20.2MB
==> Installing git dependency: pcre2
==> Pouring pcre2--10.40.monterey.bottle.tar.gz
🍺  /usr/local/Cellar/pcre2/10.40: 230 files, 6.4MB
==> Installing git
==> Pouring git--2.36.1.monterey.bottle.tar.gz
==> Caveats
The Tcl/Tk GUIs (e.g. gitk, git-gui) are now in the `git-gui` formula.
Subversion interoperability (git-svn) is now in the `git-svn` formula.

zsh completions and functions have been installed to:
  /usr/local/share/zsh/site-functions

Emacs Lisp files have been installed to:
  /usr/local/share/emacs/site-lisp/git
==> Summary
🍺  /usr/local/Cellar/git/2.36.1: 1,545 files, 43.6MB
==> Running `brew cleanup git`...
Disable this behaviour by setting HOMEBREW_NO_INSTALL_CLEANUP.
Hide these hints with HOMEBREW_NO_ENV_HINTS (see `man brew`).
==> Caveats
==> git
The Tcl/Tk GUIs (e.g. gitk, git-gui) are now in the `git-gui` formula.
Subversion interoperability (git-svn) is now in the `git-svn` formula.

zsh completions and functions have been installed to:
  /usr/local/share/zsh/site-functions

Emacs Lisp files have been installed to:
  /usr/local/share/emacs/site-lisp/git
  ```

</details>
<br>

### __2-2. 설치 확인__
- 입력
```bash
git --version
```
- 출력
```bash
git version 2.32.0 (Apple Git-132)
```
