# devdoit.github.io

Hugo + [Blowfish](https://blowfish.page/) 테마 기반 개인 사이트.
`main` 브랜치에 push하면 GitHub Actions가 자동으로 빌드·배포합니다.

## 글 쓰는 방법 (CMS — 권장)

1. https://app.pagescms.org 접속 → **GitHub 계정으로 로그인**
2. `devdoit.github.io` 저장소 선택
3. 왼쪽 메뉴에서 **일기 / 포트폴리오 / 이력서** 선택 → 폼에서 작성
4. 이미지는 에디터에서 바로 업로드 (자동으로 `static/images/`에 저장됨)
5. **저장**을 누르면 자동 커밋 → 1~2분 후 사이트에 반영

## 로컬에서 직접 쓰기

```powershell
hugo new diary/2026-07-04-제목.md   # 새 글
hugo server -D                       # 미리보기 (http://localhost:1313)
git add . ; git commit -m "글 추가" ; git push
```

## 구조

- `content/diary/` — 일기
- `content/portfolio/` — 포트폴리오
- `content/resume/index.md` — 이력서
- `static/images/` — 업로드 이미지
- `config/_default/` — 사이트 설정 (hugo.toml, params.toml, menus.ko.toml 등)
- `.pages.yml` — Pages CMS 편집 폼 설정
