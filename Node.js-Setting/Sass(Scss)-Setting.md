## Sass(Scss) Setting

### __1. Node.js 설치__
> [Node.js-Setting.md 참고](/Node.js-Setting/Node.js-Setting.md)

<br>

### __2. sass 설치__
```shell
$ npm install -g sass
```

<details>

<summary>console</summary>

```shell
added 18 packages, and audited 19 packages in 2s

2 packages are looking for funding
run `npm fund` for details

found 0 vulnerabilities
npm notice
npm notice New patch version of npm available! 8.15.0 -> 8.15.1
npm notice Changelog: https://github.com/npm/cli/releases/tag/v8.15.1
npm notice Run npm install -g npm@8.15.1 to update!
npm notice
```

</details>

<br>

### __3. sass 설치 확인__
```shell
$ sass --version
1.54.0 compiled with dart2js 2.17.6
```

<br>

### __4. 실시간으로 scss 파일 변경 확인하여 css 파일로 컴파일__
#### 단일 파일
```shell
$ sass --watch ${targetFile}:${sourcesFile}
```
#### ex)
```shell
$ sass --watch scss/input.scss/:css/output.css
```
#### 설명
- ```targetFile``` : scss 파일의 위치(ex : ```scss/input.scss``` : ```scss``` 하위 폴더 ```input.scss```가 타겟)
- ```sourcesFile``` : 컴파일 된 css 파일이 생성 될 위치(ex : ```css/output.css``` : ```css``` 하위 폴더에 ```output.css``` 이름으로 생성)

#### 폴더
```shell
$ sass --watch ${targetDirectory}:${sourcesDirectory}
```
#### ex)
```shell
$ sass --watch scss/input/:css/output
```
#### 설명
- ```targetDirectory``` : 해당 폴더 밑에 있는 scss 파일 감지(ex : ```scss/input/test.scss```, ```scss/input/dir/test2.scss``` : ```scss``` 하위 폴더 ```input``` 폴더 하위의 ```scss``` 파일 들 감지(```test.scss```, ```dir/test2.scss```))
- ```sourcesDirectory``` : 해당 폴더에 컴파일 된 css 파일 생성(ex : ```scss/input/test.scss``` -> ```css/output/test.css```, ```scss/input/dir/test2.scss``` -> ```css/input/dir/test2.css```)