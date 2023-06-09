# 웹접근성

## 웹접근성이란?

<details>
<summary>자세히 보기</summary>
모든 사용자가 인터넷을 차별과 제한 없이 동등하게 이용하도록 보장하는 것
</details>

## 웹접근성을 중점적으로 고려해야 하는 대상이 있다면?

<details>
<summary>자세히 보기</summary>
<pre>
- 느린 네트워크를 가진 사용자
  - lazy loading, 페이지네이션으로 순차적 데이터 가져오기.
  - 이미지나 동영상 등의 큰 파일 크기를 최소화  
- 모바일 환경을 이용하는 사용자
  - 반응형 웹디자인을 적용.
- 장애인 (시각장애인, 청각장애인, 거동이 불편한 사람, 인지장애인 등등)
  - 키보드 탭 키를 이용한 네비게이션 지원
  - 대체텍스트 제공
</pre>
</details>

## 웹접근성을 개선하기 위한 구체적인 방법?

<details>
<summary>자세히 보기</summary>
<pre>
1. 대체 텍스트 사용 : 이미지나 비디오, 오디오 등의 대체 텍스트를 제공하여 시각적으로 이해하기 어려운 콘텐츠에 대한 정보와 의미를 전달.
2. 시맨틱 마크업 : 시맨틱한 HTML 태그를 사용하여 웹사이트의 구조를 명확하게 표현, 보조기기가 웹사이트를 읽는 데 도움을 줌.
3. 키보드 접근성 : 키보드만으로 모든 콘텐츠에 접근할 수 있도록 설계.
4. 색상, 폰트 : 적절한 색상 대비와 폰트 크기로 시각적으로 이해하기 쉬운 웹페이지 구현.
</pre>
</details>

## hover, focus, active?

<details>
<summary>자세히 보기</summary>
<pre>
사용자가 웹사이트 상호작용할 때 매우 중요한 개념.<br>
  1. hover : hover는 마우스 포인터가 요소 위에 올라갈 때 발생, 요소가 선택 가능하다는 것을 사용자에게 알림.
  2. focus : 키보드 입력을 기다릴 때 활성화, 사용자에게 현재 선택된 요소를 알림.
  3. active : 요소를 클릭했을 때 발생하는 이벤트, 해당 요소가 사용자의 입력에 대응하고 있음을 알림.
  </pre>
</details>

## html의 lang 속성

<details>
<summary>자세히 보기</summary>
<pre>
웹페이지가 사용하는 언어를 지정<br>
검색엔진이나 스크린리더 등이 해당 언어에 대한 처리를 수행할 수 있도록 도움.
</pre>
</details>

## role, name, value 속성

<details>
<summary>자세히 보기</summary>
<pre>
웹접근성을 높이기 위해 사용되는 속성<br>
  - role : HTML 요소의 기본 역할과 다른 역할을 지정, 보조기기가 해당 요소의 역할을 인식하고할 수 있도록 도움.
  - name : JS에서 요소를 참조하거나 form 전송시 참조.
  - value : 요소의 값, input의 초기값을 설정
  </pre>
</details>

## 대체텍스트가 필요한 이유는

<details>
<summary>자세히 보기</summary>
<pre>
대체 텍스트는 이미지, 동영상 등과 같은 미디어 콘텐츠를 대신하여 제공되는 텍스트 정보<br>
  1. 시각 장애인 등 모든 사용자가 제한없이 웹 콘텐츠를 이용할 수 있도록 도움.
  2. 검색엔진 최적화에 도움. 이미지, 동영상 콘텐츠를 검색엔진이 인식하여 노출 가능성을 높임.
</pre>
</details>
