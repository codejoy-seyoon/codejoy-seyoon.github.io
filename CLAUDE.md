# 블로그 작업 규칙 (Code.Joy)

- Minimal Mistakes **remote theme starter** 기반 (fork 아님)
- 그래서 `_layouts` · `_includes` · `_sass` 폴더가 **없다**. 강의·블로그 글에서 그 파일을 고치라고 하면
  해당 폴더를 직접 만들어 override 해야 한다
- `remote_theme` 은 버전 고정: `mmistakes/minimal-mistakes@4.28.1` (풀면 테마 업데이트에 사이트가 흔들림)
- 로컬에 Ruby/bundler 없음 → `bundle exec jekyll serve` 안 됨.
  **push 후 실제 사이트에서 확인**한다 (반영까지 1~2분)
- 배포 확인: <https://codejoy-seyoon.github.io> / 실패 여부는 저장소 Actions 탭

## 파일 규칙

- 글 파일명: `_posts/YYYY-MM-DD-슬러그.md` — 날짜 뒤 슬러그 필수, 확장자는 `.md` 하나만
- 이미지: `assets/images/` 에 두고, 본문에서는 `/assets/images/파일명.png`
  (앞에 `/`, `../` 없음. Typora가 넣는 상대경로는 Jekyll에서 깨진다)
- 파일명은 영문 소문자 + 하이픈만. 한글·공백 금지 (URL 인코딩으로 깨짐)
- front matter 는 `---` 사이에 빈 줄 없이 붙여 쓴다

## 도구

- 글쓰기는 Typora, 설정 파일·커밋은 VS Code
- Typora 사이드바는 마크다운만 보여줘서 `_config.yml` 이 안 보인다 (파일이 없는 게 아님)
- git 계정이 두 개라 remote URL 에 계정이 박혀 있어야 한다 → 이 저장소는 `codejoy-seyoon`
