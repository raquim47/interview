# HTML

## HTML란?

<details>
<summary>자세히 보기</summary>
웹을 이루는 가장 기초적인 구성 요소로, 웹 콘텐츠의 의미와 구조를 정의할 때 사용하는 마크업 언어입니다.
</details>

## Semantic tag가 무엇인가요?

<details>
<summary>자세히 보기</summary>
 HTML5에서 추가된 의미론적 태그로 웹 페이지의 구조와 의미를 더 잘 나타내기 위한 태그입니다.
</details>

## article vs section

<details>
<summary>자세히 보기</summary>
article : 독립적인 콘텐츠를 나타내는 데 사용한다. 예를 들어, 블로그 게시물, 뉴스 기사, 포럼 글 등과 같이 웹 페이지의 다른 부분과 관련없이 독립적으로 읽을 수 있는 콘텐츠를 그룹화하는 데 쓰인다.
section : 문서의 구획을 나타내는 데 사용한다. section 태그는 문서에서 주제와 관련된 내용을 그룹화하며, 보통 제목 요소 h1~h6태그를 포함한다. 웹 페이지에서는 일반적으로 section 태그는 요소로 본문의 일부를 그룹화하는 데 사용한다.
</details>

## alt와 title의 차이

<details>
<summary>자세히 보기</summary>
alt 속성은 이미지에 대한 대체 텍스트 설명으로, 스크린 리더가 alt의 값을 읽어 사용자에게 이미지를 설명함으로써 웹 접근성을 향상시킵니다. 이미지를 표시할 수 없는 경우, alt 특성의 텍스트를 대신해서 브라우저가 보여주기도 합니다. 

title 속성은 주로 a태그에 사용하고 요소에 대한 추가 정보를 제공하는 역할. 마우스 오버하면 툴팁을 제공.

title 특성은 alt 특성을 대체하지 못하며, 이미지를 설명하는 대체 텍스트는 alt 특성을 사용해야 합니다. 두 값이 동일한 경우 스크린 리더에서 같은 내용을 두 번 읽게 되므로, 혼란을 줄이기 위해 서로 다른 값을 사용하는 것이 좋습니다."
</details>

## img vs background-image

<details>
<summary>자세히 보기</summary>
img: 웹 페이지 안에서 하나의 중요한 요소를 담고 있을 때 쓰임.
css bacground-image : 이미지가 문서의 일부분이 아니고, 스타일링 목적으로만 사용될 때 쓰임.
</details>

## ol, ul, dl

<details>
<summary>자세히 보기</summary>
ol 태그: 정렬된 목록 (순서 중요)
ul 태그: 정렬되지 않은 목록
dl 태그: 정의 목록, dt태그는 용어, dd태그는 해당 용어의 정의를 표시,
</details>

## srcset

<details>
<summary>자세히 보기</summary>
srcset 속성은 웹 페이지에서 이미지를 표시할 때, 다양한 크기의 이미지를 제공하여 화면의 크기에 따라 적절한 이미지를 선택해서 보여줄 수 있도록 도와주는 속성 -> 성능 향상

```<img src="image-1x.jpg" srcset="image-small.jpg 480w, image-medium.jpg 960w, image-large.jpg 1920w" sizes="(max-width: 480px) 480px, (max-width: 960px) 960px, 1920px" alt="Responsive image">```
```<img src="image-1x.jpg" srcset="image-1x.jpg 1x, image-2x.jpg 2x, image-3x.jpg 3x" alt="Responsive image">```
</details>




