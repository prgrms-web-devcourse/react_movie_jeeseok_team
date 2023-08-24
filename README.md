# 프로젝트 초기 세팅 가이드

아래와 같은 순서로 프로젝트 초기 세팅을 했다.

### vite + react + typescript

```
npm create vite@latest
```

React, TypeScript를 선택한다.

```
npm i
```

### prettier

```
npm i -D prettier eslint-config-prettier eslint-plugin-prettier
```

```
// .eslintrc.cjs
extends: [
	...
	"plugin:prettier/recommended"
]
```

```
// .prettierrc
{
	"trailingComma": "es5",
	"tabWidth": 2,
	"semi": true,
	"singleQuote": true,
	"arrowParens": "always"
}
```

만약 prettier에서 A dynamic import callback was not specified 라는 에러가 뜨면 vs code를 재시작하면 된다.

### emotion/styled

```
npm i @emotion/styled
```

### reset css

```
// index.html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/reset-css@5.0.2/reset.min.css">
```

### storybook

```
npx storybook@latest init
```

중간에 `...Would you like to install it? › `라는 질문에 y를 입력한다.
