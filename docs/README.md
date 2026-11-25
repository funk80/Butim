# Documentation layout · 문서 구성

[English overview](../README.md) · [한국어 소개](../README.ko.md)

## Current layout / 현재 구성

```text
README.md                       English product overview
README.ko.md                    한국어 제품 소개
LICENSE.txt                     Software usage terms / 사용권 약관
docs/
  README.md                     Documentation maintenance / 문서 관리 안내
  en/
    user-guide.md               English user guide
    technical-reference.md      Architecture, data, and build reference
  ko/
    user-guide.md               한국어 사용 설명서
    technical-reference.md      아키텍처·데이터·빌드 참고
  assets/
    en/                         Real English UI screenshots
    ko/                         실제 한국어 UI 캡처
```

The root READMEs introduce the product and download. Detailed user instructions and development reference material live in separate documents. Images belong to documentation, not a top-level generic `images` folder or future application runtime assets.

루트 README는 제품 소개와 다운로드를 안내합니다. 상세 사용법과 개발 참고는 별도 문서로 나누고, 이미지는 `docs/assets`에서 관리하여 향후 앱 자산과 혼동하지 않게 합니다.

## Language rules / 언어별 규칙

- English pages reference only `assets/en` screenshots; Korean pages reference only `assets/ko` screenshots.
- Keep equivalent document names under `en/` and `ko/`, and provide links to the other language.
- Update both language versions when behavior changes; preserve the version each description documents.
- Use repository-relative image links so a clone or another branch can display the same content. Product download links point to GitHub Releases.
- Keep the Korean legal text in `LICENSE.txt`; English summaries point to it rather than silently introducing another license.

영문 문서는 영문 캡처만, 한글 문서는 한글 캡처만 사용합니다. 언어별 문서 파일명과 대응 구성을 유지하고, 동작이 바뀌면 양쪽을 함께 갱신합니다. 기술 문서의 버전과 실제 배포 버전은 구분합니다.

## Sources / 출처

Documentation was adapted from the project's Confluence page (page ID `2417328259`, page revision **14**) describing Butim **v1.9.2**, and the installed v1.9.2 bilingual help. Readers do not need Confluence access to use these documents; no authenticated image links are embedded.

| Assets | Source |
| --- | --- |
| `ko/screenshot_memo.png`, `ko/screenshot_manage.png`, `ko/screenshot_settings.png` | Original attachments downloaded from the Confluence project page |
| Other `ko/*.png` | Installed Butim v1.9.2 `help/` images |
| `en/*.png` | Installed Butim v1.9.2 `help-en/` images |

The English images are actual English UI captures supplied with the app, not translated overlays on Korean screenshots. All copied images retain their source bytes. Diagram content in the technical references is recreated as language-specific Mermaid, based on the documented responsibilities. Memory figures are attributed development measurements, not newly verified benchmarks.

한글 대표 캡처 3개는 Confluence 첨부 원본, 추가 한글 캡처와 영문 캡처는 설치된 v1.9.2 도움말 원본입니다. 영문 이미지는 한글 그림에 번역 문구를 합성한 것이 아닙니다. 기술 구성도는 문서 설명을 바탕으로 언어별 Mermaid로 재작성했습니다.

## Future source code / 향후 소스 코드

These are placement conventions, not directories that exist in the current checkout:

| Path | Purpose |
| --- | --- |
| `src/Butim.Core/` | Calculation, models, storage, layout, localization |
| `src/Butim/` | WPF app; its `Assets/` contains runtime resources |
| `tests/Butim.Tests/` | Tests |
| `tools/` | Development and migration tools |
| `Installer/` | Installer scripts |
| `Butim.sln` | Solution file at repository root |

Do not create placeholder source trees merely to match the documentation. When source is added, keep `docs/` independent, update the source-availability statements, and verify the build paths against the real tree. Build outputs (`bin/`, `obj/`, `Output/`) and installers should not be mixed with the published documentation. Installer downloads belong in GitHub Releases.

위 경로는 향후 배치 기준이며 현재 소스가 있다는 의미가 아닙니다. 빈 소스 디렉터리를 문서 때문에 미리 만들지 않습니다. 소스를 추가할 때 실제 경로와 빌드 명령을 검증하고, 문서의 소스 제공 여부를 함께 바꿉니다. `bin/`, `obj/`, `Output/` 및 설치 파일은 문서와 섞지 않으며 설치 파일은 Releases에 둡니다.

Directory organization alone does not publish source or grant new rights. Retain the intended license when adding files; a public repository makes any committed source publicly visible.

폴더를 준비하는 것만으로 소스 공개나 이용 권한이 바뀌지는 않습니다. 파일 추가 시 기존 사용권 의도를 유지해야 하며, 공개 저장소에 커밋한 소스는 누구나 볼 수 있습니다.
