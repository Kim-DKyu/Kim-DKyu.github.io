# 이력서 사이트

GitHub Pages + Jekyll(minimal 테마). 서버 없이 push 만 하면 GitHub 이 빌드해 올린다.

## 올리는 법 (처음 한 번)

1. GitHub 에서 `<계정>.github.io` 이름으로 public 저장소를 만든다 (README 없이 빈 저장소).
2. 이 폴더에서:

   ```bash
   git remote add origin https://github.com/<계정>/<계정>.github.io.git
   git push -u origin main
   ```

3. 1~2분 뒤 `https://<계정>.github.io` 가 열린다. 저장소 Actions 탭의
   "pages build and deployment" 가 초록색이면 완료.

## 고치는 법

- 내용: `index.md` 수정 → commit → push. 다시 빌드되어 반영된다.
- 모양: `_config.yml` 의 `remote_theme` 한 줄 교체.
- 검색 노출: `_includes/head-custom.html` 의 robots 메타 삭제.
- PDF 도 같이 두려면 `resume.pdf` 를 이 폴더에 넣고 push. `index.md` 의 [PDF](resume.pdf) 링크가 살아난다.

## 파일 구성

```
_config.yml                 테마·제목 설정
index.md                    이력서 본문 (마크다운)
_includes/head-custom.html  <head> 추가분 (noindex)
.gitignore
README.md                   이 문서 (사이트에는 안 나옴)
```
