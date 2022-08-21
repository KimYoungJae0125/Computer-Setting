## Nest.js tpxld

### __1. Node.js 설치__
> [Node.js-Setting.md 참고](/Mac-Setting/Node.js-Settinge.js-Setting/Node.js-Setting.md)

<br>


### __2. Nest.js 설치__
```shell
$ npm i -g @nestjs/cli
```

```shell
added 250 packages, and audited 251 packages in 21s

39 packages are looking for funding
  run `npm fund` for details

found 0 vulnerabilities
npm notice 
npm notice New minor version of npm available! 8.15.0 -> 8.18.0
npm notice Changelog: https://github.com/npm/cli/releases/tag/v8.18.0
npm notice Run npm install -g npm@8.18.0 to update!
npm notice 

```

### __3. 설치 확인__
```shell
$ nest --version
```

### __4. Nest.js 프로젝트 만들기__
```shell
$ nest new ${project-name}
```

```shell
⚡  We will scaffold your app in a few seconds..

CREATE nest-start/.eslintrc.js (665 bytes)
CREATE nest-start/.prettierrc (51 bytes)
CREATE nest-start/README.md (3340 bytes)
CREATE nest-start/nest-cli.json (118 bytes)
CREATE nest-start/package.json (1995 bytes)
CREATE nest-start/tsconfig.build.json (97 bytes)
CREATE nest-start/tsconfig.json (546 bytes)
CREATE nest-start/src/app.controller.spec.ts (617 bytes)
CREATE nest-start/src/app.controller.ts (274 bytes)
CREATE nest-start/src/app.module.ts (249 bytes)
CREATE nest-start/src/app.service.ts (142 bytes)
CREATE nest-start/src/main.ts (208 bytes)
CREATE nest-start/test/app.e2e-spec.ts (630 bytes)
CREATE nest-start/test/jest-e2e.json (183 bytes)

## Nets.js Package Manger 어떤걸로 사용할지 선택(화살표 방향으로 이동) 
? Which package manager would you ❤️  to use? (Use arrow keys)
❯ npm
yarn
pnpm 

## 선택하였으면

✔ Installation in progress... ☕

🚀  Successfully created project ${Project-name}
👉  Get started with the following commands:

$ cd nest-start
$ npm run start

                                         
                          Thanks for installing Nest 🙏
                 Please consider donating to our open collective
                        to help us maintain this package.
                                         
                                         
               🍷  Donate: https://opencollective.com/nest

```
