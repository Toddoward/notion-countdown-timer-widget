<div align="right">
  🌐 Read in: <a href="README.kr.md" style="font-weight: bold;">한국어</a> | <a href="README.md">English</a>
</div>


# 노션 카운트다운 타이머 위젯

<img width="1920" height="944" alt="image" src="https://github.com/user-attachments/assets/79e9a56d-4679-4634-99b4-58368710554d" />

노션 페이지에 깔끔하게 삽입할 수 있는 커스텀 카운트다운 타이머 위젯입니다. 노션 임베드 블록 크기에 맞춰 자동으로 크기가 조절되며, 이 위젯은 [Logwork](https://logwork.com/countdown-timer)의 소스코드를 활용하여 작동합니다.

## 📂 레포지토리 구조

```text
notion-countdown-timer-widget/
├ README.md
├ README.kr.md
└ widget.html
```

## 🚀 사용 방법
아래 단계를 따라 나만의 타이머를 만들고 노션에 적용해 보세요.

### 1. 레포지토리 포크
화면 우측 상단의 `Fork` 버튼을 눌러 이 레포지토리를 본인의 GitHub 계정으로 복사합니다.

### 2. 위젯 설정 변경
포크해 온 본인의 레포지토리에서 `widget.html` 파일을 엽니다. 코드 42번째 줄 부근의 `<script>` 태그 안에 있는 `countdownConfig` 변수를 찾아 원하는 설정값으로 수정합니다:

```js
const countdownConfig = {
  title: "최종 프로젝트 카운트다운",        // 위젯 상단에 표시될 제목
  date: "2026-06-18 12:00",              // 목표 날짜 및 시간
  timezone: "Asia/Seoul",                // 타임존 설정
  language: "ko",                        // 시간 단위 언어 (예: ko, en)
  colors: {
    text: "#6e6e6e",                     // 텍스트 색상
    digits: "#ededed",                   // 숫자 색상
    units: "#8f8f8f"                     // 단위(일, 시간, 분, 초) 색상
  }
};
```

수정이 완료되면 커밋하여 변경 사항을 저장합니다.

### 3. GitHub Pages로 배포
1. 레포지토리의 `Settings` 탭으로 이동합니다.

2. 좌측 메뉴에서 `Pages`를 클릭합니다.

3. `Build and deployment` 항목에서 브랜치를 `main`으로 설정하고 `Save`를 누릅니다.

4. 잠시 후 웹사이트 배포가 완료되면, `widget.html`의 주소를 복사합니다.
(예: `https://본인아이디.github.io/notion-countdown-timer-widget/widget.html`)

### 4. 노션에 임베드
1. 노션 페이지의 빈 줄에서 `/embed` 또는 `/임베드`를 입력하여 임베드 블록을 생성합니다.

2. 복사해 둔 GitHub Pages URL을 붙여넣고 `링크 임베드` 버튼을 클릭합니다.

3. 생성된 블록의 모서리를 드래그하여 원하는 크기로 맞춥니다. 박스 크기에 맞춰 위젯이 자동으로 꽉 차게 렌더링됩니다!

## 💡 출처
이 레포지토리의 위젯은 [Logwork](https://logwork.com/countdown-timer)에서 제공하는 카운트다운 타이머 소스코드를 기반으로 제작되었습니다.
