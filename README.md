# 릴스 대본 스튜디오

뷰티 릴스 나레이션 대본(+선택 시 인스타 캡션)을 만드는 단일 HTML 웹앱입니다.

## 사용
https://skyy03180-wq.github.io/reels-script-studio/ 를 열고, 상단에 Google AI Studio에서 발급한
Gemini API 키를 한 번만 입력하면 이 브라우저에 저장됩니다. 키는 브라우저(localStorage)에만
저장되고 서버로 보내지 않습니다.

## 구성
- 제품 소구점 이미지·PDF 여러 개 업로드(합쳐 8개까지, 섞어서 가능)
- 제품 소구점 텍스트
- 레퍼런스 영상 업로드(18MB 이하는 인라인, 초과 시 Files API 업로드)
- 레퍼런스 영상 링크 입력(공개 YouTube는 fileData로 직접 분석, 인스타 등 나머지 링크는 프롬프트 참고용 + 인스타 안내 문구)
- 소구점 PDF(19MB 인라인 예산 안이면 inlineData, 초과 시 Files API 업로드 후 ACTIVE 확인)
- 캡션 작성 ON/OFF, 길이(20초/30초), 밈 강도, 후킹 스타일
- 나레이션 대본 / 캡션 원클릭 복사

`index.html` 단일 파일로 동작하며 빌드 과정이 없습니다.
