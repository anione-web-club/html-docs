# HTML DOCS

HTML을 설명하기 위한 문서입니다.

## 개발시 주의사항

`sveltestrap` 패키지에서 `popperjs` 라는 패키지를 쓰는데,
이게 vite로 빌드할때 좀 불안정해서 직접 바꿔줘야함.

레포 들고와서 `npm install` 하고 나서,
`node_modules/@popperjs/core/package.json`에 드가서,
맨 끝에 `"type": "module"` 이거 추가해 주면됨.