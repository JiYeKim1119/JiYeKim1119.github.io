# Ji Ye Kim Academic Website 배포 방법

이 버전은 기존 Jekyll/SCSS 빌드에 의존하지 않는 완전한 정적 웹사이트입니다. CSS와 JavaScript가 `index.html` 안에 들어 있어서 GitHub Pages의 경로 문제나 SCSS 컴파일 문제로 디자인이 사라지지 않습니다.

## 가장 안전한 적용 방법

1. 이 압축파일을 컴퓨터에서 풉니다.
2. GitHub repository `JiYeKim1119/jiyekim.github.io`를 엽니다.
3. repository 루트에 다음 파일을 업로드합니다.
   - `index.html`
   - `.nojekyll`
   - `images/README.txt`
   - `files/README.txt`
4. 기존 파일은 당장 삭제하지 않아도 됩니다. `.nojekyll`과 새 `index.html`이 기존 Jekyll 페이지 대신 사용됩니다.
5. 프로필 사진은 `images/avatar.jpg`라는 정확한 경로와 파일명으로 업로드합니다.
6. `Settings → Pages`에서 Source가 `Deploy from a branch`, Branch가 `main / (root)`인지 확인합니다.
7. Actions의 배포가 완료된 후 강력 새로고침합니다.
   - Mac: `Command + Shift + R`
   - Windows: `Ctrl + Shift + R`

## 현재 주소

Repository 이름을 그대로 두면:

`https://jiyekim1119.github.io/jiyekim.github.io/`

Repository 이름을 `JiYeKim1119.github.io`로 바꾸면:

`https://jiyekim1119.github.io/`

이 완성본은 상대경로를 사용하므로 두 주소 모두에서 작동합니다.

## 사진 추가

사진을 다음 위치에 추가합니다.

`images/avatar.jpg`

세로형 4:5 사진이 가장 자연스럽습니다. 사진이 없을 때는 `JK` 이니셜이 자동으로 표시됩니다.

## 수정하기 쉬운 부분

`index.html`에서 아래 텍스트를 검색하면 빠르게 수정할 수 있습니다.

- `Ji Ye Kim`
- `jiyek@usc.edu`
- `Selected Publications`
- `Education`
- `Teaching & Service`

색상은 파일 위쪽 `:root`의 `--wine-...` 값에서 바꿀 수 있습니다.
