# Butim · 붙임쪽지

A Windows sticky notes app with inline calculations, customizable notes, and file export.

메모 속 수식 계산과 파일 내보내기를 지원하는 Windows 바탕화면 메모 앱입니다.

**Windows 10/11 (x64) · 한국어 / English · Free for personal and business use**

[English](#english) · [한국어](#한국어)

## English

Keep tasks, meeting notes, and quick calculations on your desktop. Butim gives each note its own window and remembers its appearance and position so you can pick up where you left off.

This repository provides installers and documentation. The source code is not published.

### Download and install

1. Open **Releases** on this repository and select the latest release.
2. Under **Assets**, download **Butim_Setup.exe**.
3. Run the installer and follow the instructions.
4. Launch Butim and press **Ctrl+Alt+N** to create a note.

**Requirements:** Windows 10 or 11, x64. If .NET 10.0 Desktop Runtime is missing, the installer installs it using the bundled runtime installer. Butim installs for the current user; installing the runtime may require administrator approval.

Butim stays in the system tray. On first launch, a welcome note introduces the basics.

### Features

- **Calculate as you write.** Use arithmetic, parentheses, powers, percentages, and named variables directly in a note. Results appear at the end of each expression line.
- **Customize each note.** Choose from eight colors, set fonts, and adjust the size and position of individual notes.
- **Keep your desktop organized.** Pin notes above other windows, lock editing, collapse notes to their title bars, and snap them to neighboring notes or screen edges.
- **Find and manage notes.** Search, mark favorites, sort, switch between grid and list views, and manage multiple notes together.
- **Save notes as files.** Export a note to a `.butim` file on your desktop. Double-click the file to bring it back into Butim.
- **Recover deleted notes.** Restore notes from the app's trash before permanently deleting them.
- **Choose your language and theme.** Korean and English interfaces and help are available, along with light, dark, and system-following themes.
- **Continue where you left off.** Notes save automatically, and their appearance and position are restored when you restart the app.

### Inline calculation example

Type the following into a note:

```text
price = 12000
quantity = 5
total = price * quantity
discounted = total * (1 - 10%)
```

Butim displays **60,000** beside the `total` expression and **54,000** beside `discounted`. You only type the expressions; results are displayed automatically.

Supported operators: `+`, `-`, `*`, `/`, `^`, parentheses, and postfix `%`. Variable names are case-sensitive and can be reused after they are defined. Date and phone-number exclusion patterns help keep ordinary text from being treated as calculations; custom patterns can be added in settings.

### Default shortcuts

| Shortcut | Action |
| --- | --- |
| `Ctrl+Alt+N` | Create a new note |
| `Ctrl+Alt+M` | Bring all notes to the front |
| `Ctrl` + mouse wheel | Adjust the font size while editing a note |
| `Ctrl+0` | Restore the default font and size while editing a note |
| `Alt` + drag | Move a note without snapping |

The two global shortcuts can be changed in settings.

### Tips and data

- The detach button exports the note to your desktop by default. Its action can be changed to hide the note or move it to the trash.
- Locking a note prevents text editing; it does not prevent moving or deleting the note.
- Notes and settings are stored locally in `%APPDATA%\Butim\`.
- Uninstalling the app leaves this data in place so it can be used after reinstallation.
- Open the built-in help from the note menu or the system tray menu for more details.

### License

Butim is free to use for individuals, businesses, and organizations, including for commercial work. Internal deployment within an organization and backup copies are permitted.

Butim is proprietary software; its source code is not published. Except where applicable law or a component's separate license permits otherwise, modification, external redistribution, sale, rental, or bundling with other products requires prior permission from the copyright holder. Sharing a link to the official download page is welcome.

See [LICENSE.txt](LICENSE.txt) for the full terms in Korean. Third-party components remain subject to their own licenses.

## 한국어

붙임쪽지(Butim)는 할 일, 회의 메모, 간단한 계산을 바탕화면에 붙여 두고 사용하는 메모 앱입니다. 메모마다 별도의 창으로 열리며, 모양과 위치를 기억해 다시 실행해도 이어서 사용할 수 있습니다.

이 저장소는 설치 파일과 사용 안내를 제공합니다. 소스 코드는 공개하지 않습니다.

### 다운로드 및 설치

1. 이 저장소의 **Releases**에서 최신 릴리스를 엽니다.
2. **Assets**에서 **Butim_Setup.exe**를 내려받습니다.
3. 설치 파일을 실행하고 안내에 따라 설치합니다.
4. Butim을 실행한 후 **Ctrl+Alt+N**을 눌러 새 붙임쪽지를 만듭니다.

**지원 환경:** Windows 10/11 (x64). .NET 10.0 Desktop Runtime이 없으면 함께 포함된 런타임 설치기로 설치합니다. 앱은 사용자 단위로 설치되며, 런타임 설치 시에는 관리자 권한 확인이 필요할 수 있습니다.

실행 후에는 작업 표시줄 알림 영역에 상주하며, 처음 실행하면 사용법을 소개하는 붙임쪽지가 열립니다.

### 주요 기능

- **메모 안에서 바로 계산:** 사칙연산, 괄호, 거듭제곱, 백분율과 이름을 붙인 변수를 사용하면 계산 결과가 줄 끝에 표시됩니다.
- **메모별 꾸미기:** 8가지 색상과 글꼴을 선택하고 메모마다 크기와 위치를 조절할 수 있습니다.
- **편리한 창 정리:** 항상 위에 두기, 편집 잠금, 제목줄만 남기는 접기, 다른 메모나 화면 가장자리에 맞추는 자석 정렬을 지원합니다.
- **한곳에서 관리:** 검색, 즐겨찾기, 정렬, 격자·목록 보기로 메모를 찾고 여러 메모를 함께 정리합니다.
- **파일로 보관:** 메모를 바탕화면의 `.butim` 파일로 내보내고, 파일을 더블클릭해 다시 가져옵니다.
- **휴지통에서 복원:** 휴지통으로 옮긴 메모는 영구 삭제하기 전에 복원할 수 있습니다.
- **언어와 테마 선택:** 한국어·영어 화면과 도움말, 밝은 테마·어두운 테마·시스템 설정 따르기를 지원합니다.
- **자동 저장:** 작성한 메모를 자동 저장하고, 다시 실행하면 메모의 모양과 위치를 복원합니다.

### 계산 예시

붙임쪽지에 다음과 같이 입력하세요.

```text
단가 = 12000
수량 = 5
합계 = 단가 * 수량
할인가 = 합계 * (1 - 10%)
```

`합계` 줄에는 **60,000**, `할인가` 줄에는 **54,000**이 표시됩니다. 결과를 직접 입력할 필요 없이 식을 작성하면 자동으로 계산합니다.

지원 연산자는 `+`, `-`, `*`, `/`, `^`, 괄호, 후위 `%`입니다. 변수는 정의한 뒤 아래 줄에서 사용할 수 있으며 대소문자를 구분합니다. 날짜나 전화번호를 계산하지 않도록 제외 패턴을 제공하며, 설정에서 사용자 패턴을 추가할 수 있습니다.

### 기본 단축키

| 단축키 | 기능 |
| --- | --- |
| `Ctrl+Alt+N` | 새 붙임쪽지 만들기 |
| `Ctrl+Alt+M` | 모든 붙임쪽지를 앞으로 가져오기 |
| `Ctrl` + 마우스 휠 | 본문 편집 중 글꼴 크기 조절 |
| `Ctrl+0` | 본문 편집 중 기본 글꼴과 크기로 되돌리기 |
| `Alt` + 끌기 | 자석 정렬 없이 메모 이동 |

새 붙임쪽지와 모두 앞으로 단축키는 설정에서 변경할 수 있습니다.

### 사용 팁과 데이터

- 떼기 단추의 기본 동작은 바탕화면으로 내보내기입니다. 설정에서 숨기기 또는 휴지통으로 이동으로 바꿀 수 있습니다.
- 잠금은 본문 편집을 막는 기능이며, 메모의 이동이나 삭제를 막지는 않습니다.
- 메모와 설정은 PC의 `%APPDATA%\Butim\`에 저장됩니다.
- 앱을 제거해도 해당 데이터는 남아 있어 다시 설치하면 이어서 사용할 수 있습니다.
- 자세한 사용법은 붙임쪽지 메뉴 또는 알림 영역 메뉴에서 도움말을 여세요.

### 라이선스

개인 및 기업·기관 모두 업무 목적을 포함해 무료로 사용할 수 있습니다. 조직 내부 배포와 백업 목적의 복사를 허용합니다.

Butim은 소스 코드를 공개하지 않는 소프트웨어입니다. 관련 법령 또는 구성요소의 별도 라이선스에서 허용하는 경우를 제외하고, 수정·외부 재배포·판매·대여·다른 제품에 포함한 배포에는 저작권자의 사전 허락이 필요합니다. 공식 다운로드 페이지의 링크 공유는 허용합니다.

자세한 조건은 [LICENSE.txt](LICENSE.txt)를 참고하세요. 제3자 구성요소에는 각 구성요소의 라이선스가 적용됩니다.
