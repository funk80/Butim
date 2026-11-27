# Documentation layout · 문서 구성

[English overview](../README.md) · [한국어 소개](../README.ko.md)

## Find information about Butim / 주제별 문서 찾기

Butim (붙임쪽지) is a Windows desktop sticky notes app with inline calculations. These documents describe v1.9.2. Use the product overview for supported platforms and usage terms, the user guide for behavior, and the data reference for compatibility. Check [Releases](https://github.com/funk80/Butim/releases) for downloadable versions.

붙임쪽지(Butim)는 메모 안에서 수식을 계산하는 Windows 바탕화면 메모 앱입니다. 문서 기준은 v1.9.2입니다. 제품 소개는 지원 환경과 사용 조건, 사용 설명서는 기능과 조작, 데이터 참고는 호환성을 설명합니다. 다운로드 버전은 Releases에서 확인합니다.

| Topic / 주제 | English | 한국어 |
| --- | --- | --- |
| Product, platform, free business use / 제품·환경·기업 무료 사용 | [Product facts](../README.md#product-facts) | [제품 정보](../README.ko.md#제품-정보) |
| Common questions / 자주 묻는 질문 | [FAQ](../README.md#frequently-asked-questions) | [자주 묻는 질문](../README.ko.md#자주-묻는-질문) |
| Installation / 설치 | [Download and install](../README.md#download-and-install) | [다운로드 및 설치](../README.ko.md#다운로드-및-설치) |
| Arithmetic and variables / 수식·변수 | [Calculations](en/user-guide.md#calculations) | [계산](ko/user-guide.md#계산) |
| Exclusion patterns / 계산 제외 패턴 | [Formats not to calculate](en/user-guide.md#formats-not-to-calculate) | [계산하지 않을 형식](ko/user-guide.md#계산하지-않을-형식) |
| Note search and organization / 메모 검색·정리 | [Manage notes](en/user-guide.md#manage-notes) | [붙임쪽지 관리](ko/user-guide.md#붙임쪽지-관리) |
| Export/import / 파일 내보내기·가져오기 | [Peel off and export](en/user-guide.md#peel-off-and-export) | [떼기와 내보내기](ko/user-guide.md#떼기와-내보내기) |
| Language and shortcuts / 언어·단축키 | [Settings](en/user-guide.md#settings) | [설정](ko/user-guide.md#설정) |
| Local storage / 로컬 저장 | [Data and installation](en/user-guide.md#data-and-installation) | [데이터와 설치](ko/user-guide.md#데이터와-설치) |
| Troubleshooting / 문제 해결 | [Troubleshooting](en/user-guide.md#troubleshooting) | [문제 해결](ko/user-guide.md#문제-해결) |
| Data and compatibility / 데이터·호환성 | [Data reference](en/technical-reference.md) | [데이터 참고](ko/technical-reference.md) |
| Bugs and suggestions / 오류·기능 제안 | [Issue templates](https://github.com/funk80/Butim/issues/new/choose) | [신고·제안 양식](https://github.com/funk80/Butim/issues/new/choose) |
| Security reporting / 보안 신고 | [Security policy](../SECURITY.md) | [보안 정책](../SECURITY.md) |
| Full usage terms / 전체 사용 조건 | [License (Korean)](../LICENSE.txt) | [사용권 약관](../LICENSE.txt) |

## Current layout / 현재 구성

```text
README.md                       English product overview
README.ko.md                    한국어 제품 소개
LICENSE.txt                     Software usage terms / 사용권 약관
SECURITY.md                     Security reporting policy / 보안 신고 정책
.github/ISSUE_TEMPLATE/         Bug and feature forms / 오류·제안 양식
docs/
  README.md                     Documentation maintenance / 문서 관리 안내
  en/
    user-guide.md               English user guide
    technical-reference.md      Public data and compatibility reference
  ko/
    user-guide.md               한국어 사용 설명서
    technical-reference.md      공개 데이터·호환성 참고
  assets/
    en/                         Real English UI screenshots
    ko/                         실제 한국어 UI 캡처
```

The root READMEs introduce the product and download. Detailed usage and data guidance live in separate documents. Screenshots belong to documentation under `docs/assets/`.

루트 README는 제품 소개와 다운로드를 안내합니다. 상세 사용법과 데이터 참고는 별도 문서로 나누고 이미지는 `docs/assets/`에서 관리합니다.

## Language rules / 언어별 규칙

- English pages reference only `assets/en` screenshots; Korean pages reference only `assets/ko` screenshots.
- Keep equivalent document names under `en/` and `ko/`, and provide links to the other language.
- Update both language versions when behavior changes; preserve the version each description documents.
- Use repository-relative image links so a clone or another branch can display the same content. Product download links point to GitHub Releases.
- Keep the Korean legal text in `LICENSE.txt`; English summaries point to it rather than silently introducing another license.

영문 문서는 영문 캡처만, 한글 문서는 한글 캡처만 사용합니다. 언어별 문서 파일명과 대응 구성을 유지하고, 동작이 바뀌면 양쪽을 함께 갱신합니다. 문서의 기준 버전과 실제 배포 버전은 구분합니다.

## Sources / 출처

Documentation and screenshots are based on the project's v1.9.2 documentation and installed bilingual help. All public images are stored in this repository and do not require access to an internal documentation service.

| Assets | Source |
| --- | --- |
| `ko/screenshot_memo.png`, `ko/screenshot_manage.png`, `ko/screenshot_settings.png` | Original project documentation screenshots |
| Other `ko/*.png` | Installed Butim v1.9.2 `help/` images |
| `en/*.png` | Installed Butim v1.9.2 `help-en/` images |

The English images are actual English UI captures supplied with the app, not translated overlays on Korean screenshots. Copied images retain their source bytes.

한글 대표 캡처 3개는 프로젝트 문서의 원본이며, 추가 한글 캡처와 영문 캡처는 설치된 v1.9.2 도움말 원본입니다. 영문 이미지는 한글 그림에 번역 문구를 합성한 것이 아닙니다.

## Publication scope / 공개 범위

This repository publishes user documentation and release installers. Application source code, internal architecture, build instructions, and internal service identifiers are outside its publication scope. Preserve existing media when editing documents; installer binaries belong in GitHub Releases. The existing reference filenames are retained so links continue to work.

이 저장소는 사용자 문서와 릴리스 설치 파일을 제공합니다. 앱 소스, 내부 아키텍처, 빌드 지침, 내부 서비스 식별자는 공개 범위에 포함하지 않습니다. 문서 편집 시 기존 미디어를 유지하고 설치 파일은 GitHub Releases에서 배포합니다. 기존 링크를 유지하기 위해 참고 문서의 파일명은 그대로 둡니다.
