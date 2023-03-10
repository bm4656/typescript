# TypeScript

> 🔥 TypeScript 를 공부하는 레포지토리입니다.

- [typescript 공식문서](https://www.typescriptlang.org/)
- [typescript 플레이그라운드](https://www.typescriptlang.org/play)
- [typescript 핸드북 필독](https://www.typescriptlang.org/docs/handbook/intro.html)
- [typescript 버전 수정 내역](https://www.typescriptlang.org/docs/handbook/release-notes/overview.html)
- [ts-all-in-one 강의 자료](https://github.com/ZeroCho/ts-all-in-one)

### 타입 구문이 존재하는 JavaScript

> 💡 타입 구문이 존재하는 JavaScript 즉 TypeScript이며
> TypeScript가 컴파일되면 JavaScript로 변환된다.

## 기본 지식

- **typescript는 최종적으로 javascript로 변환된다.** 순전한 typescript 코드를 돌릴 수 있는 것은 deno이나 대중화되지가 않았음. 브라우저, 노드는 모두 js 파일을 실행한다.
- typescript는 언어이자 **컴파일러(tsc)** 이다. 컴파일러는 ts 코드를 js로 바꿔준다.
- tsc는 **tsconfig.json**(tsc --init 시 생성)에 따라 ts 코드를 js(tsc 시 생성)로 바꿔준다. 인풋인 ts와 아웃풋인 js 모두에 영향을 끼치므로 tsconfig.json 설정을 반드시 봐야한다.
- **tsc 는 ts → js 로 변환하는 역할 + 타입 검사(는 강제가 아니긴 하다.)**
- 단순히 타입 검사만 하고싶다면 `tsc --noEmit` 하면 된다.
- ts 파일을 실행하는 게 아니라 결과물인 js를 실행해야 한다.
- tsconfig.json에서 그냥 esModuleInterop: true, strict: true 두 개만 주로 켜놓는 것 추천. strict: true가 핵심임.
- 에디터가 필수. VS Code나 웹스톰 반드시 필요.

```js
npm init -y         //package.json

npm i typescript    //typescript 설치

npx tsc --init      //tsconfig.json

npx tsc --noemit    //타입 검사

npx tsc             //ts -> js 파일로 바꾸는
```
