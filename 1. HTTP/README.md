# HTTP

## HTTP란?

<details>
<summary>자세히 보기</summary>
HTTP는 HyperText Transfer Protocol의 약자로, 클라이언트와 서버 간 웹 상에서 데이터를 주고받기 위한 프로토콜입니다. 주로 웹 페이지, 이미지, 동영상 등의 리소스를 교환하는데 사용됩니다.
</details>

## HTTP는 stateless하다는 것의 의미와 대안을 설명하세요

<details>
<summary>자세히 보기</summary>
 서버가 이전 요청에 대한 정보를 저장하지 않기 때문에 각각의 요청이 독립적이라는 의미입니다. 이러한 특성 덕분에 서버의 메모리 사용량이 줄어들고 확장성이 증가합니다. 그러나 상태 정보가 필요한 경우 추가 구현이 필요하며, 이때 쿠키와 세션을 이용하여 클라이언트의 상태 정보를 저장하고 추적할

 - 무상태(stateless)
 서버가 클라이언트의 상태를 보존하지 않음
 클라이언트 요청은 독립적으로 처리되며, 서버는 요청에 대한 응답만 전송
 서버의 확장성을 높임
 - 비연결성(connectionless)
 클라이언트의 요청과 서버의 응답 사이에 연결을 유지하지 않음
 서버는 불필요한 연결을 줄이고 많은 클라이언트의 요청을 동시에 처리할 수 있음
</details>

## HTTP 매서드에 대해 설명하세요

<details>
<summary>자세히 보기</summary>
 HTTP 매서드는 클라이언트가 서버에 요청을 보낼 때 사용하는 동작 방식입니다.
 GET: 리소스를 요청하는 메소드입니다. 
  POST: 리소스를 전송하는 메소드입니다. 
  PUT: 리소스를 업데이트하는 메소드입니다.
  PATCH: 리소스의 일부분만 수정하는 메소드입니다.
  DELETE: 특정 리소스를 삭제하는 메소드입니다.
</details>

## HTTP/1.0, 1.1, 2.0에 대해 설명하세요

<details>
<summary>자세히 보기</summary>
 HTTP/1.0은 기본 요청-응답 메커니즘을 제공하는 첫 버전입니다. HTTP/1.1은 지속적인 연결과 파이프라이닝 기능이 추가되어 성능이 향상되었고, HTTP/2.0은 다중화와 서버 푸시를 도입하여 웹 성능을 더욱 개선했습니다.
</details>

## DNS

<details>
<summary>자세히 보기</summary>
<pre>
 Domain Name System
 도메인 이름과 IP 주소간의 변환을 처리하는 시스템.
 인터넷 서비스 제공자(ISP)가 제공하는 DNS서버를 통해 실행.

 1. 웹브라우저에 도메인 이름을 입력하여 접속
 2. DNS서버에서 도메인 이름을 IP주소로 변환
 3. IP주소를 통해 웹서버에 페이지 요청
 4. 웹 브라우저에 웹페이지가 출력
</pre>
</details>

## TCP/UDP

<details>
<summary>자세히 보기</summary>
<pre>
 
 - TCP 
  신뢰성 있는 데이터 전송을 지원하는 연결 지향형 프로토콜
  패킷의 손실을 검사, 순서가 바뀌지 않도록 보장
  3-Way Handshake : TCP 통신을 시작할 준비가 되었는지 확인
  4-Way Handshake : TCP 통신을 종료할 준비가 되었는지 확인

  - UDP
  신호 절차 없이 일방적으로 데이터 전달
  데이터의 신뢰성은 낮지만 속도가 빠름
</pre>
</details>

## 쿠키와 세션

<details>
<summary>자세히 보기</summary>
<pre>
 
 - 쿠키
  클라이언트에 저장되는 데이터 파일
  서버의 부하가 줄어들지만 보안의 위험이 있음
 - 세션
  클라이언트의 상태 정보를 서버 측에서 유지
  보안성은 높지만 서버에 많은 자원이 필요하기 때문에 부하가 될 수 있음. 
</pre>
</details>

## JWT

<details>
<summary>자세히 보기</summary>
<pre>
 - JWT
  웹의 사용자 인증 정보를 안전하게 관리하기 위한 토큰
  서명을 통해 위조나 변조를 감지, 유효기간 설정으로 보안성을 높임
  서버에서 유지하지 않아도 됌.
</pre>
</details>

## HTTP와 HTTPS에 대해 설명하세요

<details>
<summary>자세히 보기</summary>
  HTTP는 도청이 가능하며(TCP/IP) 통신 상대를 확인하지 않아 신뢰성이 떨어집니다. 그래서 등장한 HTTPS는 보안 프로토콜인 SSL을 이용해 데이터를 암호화하고 보안성을 보장합니다. 추가로 검색엔진 최적화에도 도움을 줍니다.
</details>

## CORS와 CORS문제의 해결 방법을 설명하세요

<details>
<summary>자세히 보기</summary>
  CORS(Cross-Origin Resource Sharing)
   CORS는 보안을 위한 정책으로 CORS 문제는 일반적으로 브라우저가 다른 도메인의 리소스에 접근하려 할 때 서버가 적절한 CORS 헤더를 제공하지 않거나 클라이언트가 정책을 따르지 않는 경우에 발생합니다.
   해결방법으로는 서버 측에서 적절한 CORS 헤더를 설정하고, 클라이언트 측에서는 서버의 CORS 정책을 따르도록 구현합니다.
</details>

## OSI 7 계층이란 뭔가요?

<details>
<summary>자세히 보기</summary>
  물데네전세표응<br>
OSI 7 계층은 네트워크 통신을 7개의 계층으로 나누어 설명하는 모델입니다.
물리계층, 데이터 링크 계층, 네트워크 계층, 전송 계층, 세션 계층, 표현 계층, 응용 계층으로 나누어져 있고
각 계층을 서로 다른 기능을 담당하여 데이터를 전달합니다.
현대의 인터넷은 OSI모델이 아니라 TCP/IP모델을 따르고 있고 TCP/IP 모델에선 OSI모델의 세션 계층, 표현 계층, 응용 계층이 응용 계층으로 통합되어 있습니다.
</details>
