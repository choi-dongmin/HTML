# Web_html (웹사이트 완성)

우리는 Link 까지 배움으로 각각의 페이지를 역어 하나의 책으로 만들수 있는 방법을 배웠다 대신 이 Web 에선 이 책을 Website 라고 일컫는다.

그럼 우리는 이제 우리가 Webpage 를 만들고 역어 역어서 하나의 Website 로 만들어 볼 것이다.

```
파일명 : main.html

<!doctype html>
<html>
	<head>
		<title> Web html </title>
		<mata charset="utf-8">
	</head>

	<body>
		<h1><a href="main.html"> Web</a></h1>
		
		<ol>
			<li> <a href="1.html">HTML</a> </li> 
			<li> <a href="2.html">CSS</a> </li> 
			<li> <a href="3.html">JavaScript</a> </li> 
		</ol>
	</body>
</html>

``` 

```
파일명 : 1.html

<!doctype html>
<html>


	<head>
    <h1><a href="main.html"> Web</a></h1>

    <ol>
      <li> <a href="1.html">HTML</a> </li>
      <li> <a href="2.html">CSS</a> </li>
      <li> <a href="3.html">JavaScript</a> </li>
    </ol>

	</head>
	<body>
    <h2>HTML </h2>
		<h3>HTML 이란 무엇인가?</h3> <a href="https://ko.wikipedia.org/wiki/HTML" target="_blank" title="https://ko.wikipedia.org/wiki/HTML"><h4><strong> H</strong>yperT</strong>ext <strong>M</strong>arkup <strong>L</strong>anguage</a>
    <p>
      HTML또는 하이퍼텍스트 마크업 언어(HyperText Markup Language) 는 웹 페이지를 위한 지배적인 마크업 언어다. HTML은 제목, 단락, 목록 등과 같은 본문을 위한 구조적 의미를 나타내는 것뿐만 아니라 링크, 인용과 그 밖의 항목으로 구조적 문서를 만들 수 있는 방법을 제공한다.</h4>
    </p>
    <br><br>
    <img src="1.jpg" width="70%">
	</body>
</html>

```

```
파일명 : 2.html

<!doctype html>
<html>
	<head>
    <h1><a href="main.html"> Web</a></h1>

    <ol>
      <li> <a href="1.html">HTML</a> </li>
      <li> <a href="2.html">CSS</a> </li>
      <li> <a href="3.html">JavaScript</a> </li>
    </ol>
	</head>
	<body>
    <h2>CSS </h2>

		<h3>CSS 란 무엇인가?</h3>
		<a href="https://ko.wikipedia.org/wiki/%EC%A2%85%EC%86%8D%ED%98%95_%EC%8B%9C%ED%8A%B8" target="_blank" title="https://ko.wikipedia.org/wiki/%EC%A2%85%EC%86%8D%ED%98%95_%EC%8B%9C%ED%8A%B8"><h4><strong>C</strong>ascading <strong>S</strong>tyle <strong>S</strong>heets</a>
    <p>
      종속형 시트 또는 캐스케이딩 스타일 시트(Cascading Style Sheets, CSS)는 마크업 언어가 실제 표시되는 방법을 기술하는 언어로, HTML과 XHTML에 주로 쓰이며, XML에서도 사용할 수 있다. W3C의 표준이며, 레이아웃과 스타일을 정의할 때의 자유도가 높다.

      마크업 언어(ex. HTML)가 웹사이트의 몸체를 담당한다면 CSS는 옷과 액세서리 같은 꾸미는 역할을 담당한다고 할 수 있다. 즉, HTML 구조는 그대로 두고 CSS 파일만 변경해도 전혀 다른 웹사이트처럼 꾸밀 수 있다.

      현재 개발 중인 CSS3의 경우 그림자 효과, 그라데이션, 변형 등 그래픽 편집 프로그램으로 제작한 이미지를 대체할 수 있는 기능이 추가되었다. 또한 다양한 애니메이션 기능이 추가되어 어도비 플래시를 어느 정도 대체하고 있다.
    </h4></p>
    <br><br>
    <img src="2.jpg" width="70%">

	</body>
</html>

```

```
파일명 : 3.html

<!doctype html>
<html>
	<head>
    <h1><a href="main.html"> Web</a></h1>

    <ol>
      <li> <a href="1.html">HTML</a> </li>
      <li> <a href="2.html">CSS</a> </li>
      <li> <a href="3.html">JavaScript</a> </li>
    </ol>
	</head>
	<body>

		<h2>JavaScript </h2>
		<h3>JavaScript 란 무엇인가?</h3>
		<a href="https://ko.wikipedia.org/wiki/%EC%9E%90%EB%B0%94%EC%8A%A4%ED%81%AC%EB%A6%BD%ED%8A%B8" title="https://ko.wikipedia.org/wiki/%EC%9E%90%EB%B0%94%EC%8A%A4%ED%81%AC%EB%A6%BD%ED%8A%B8" target="_blank"><h4><strong>J</strong>ava<strong>S</strong>cript</a>
    <p>
      자바스크립트(영어: JavaScript)는 객체 기반의 스크립트 프로그래밍 언어이다. 이 언어는 웹 브라우저 내에서 주로 사용하며, 다른 응용 프로그램의 내장 객체에도 접근할 수 있는 기능을 가지고 있다. 또한 Node.js와 같은 런타임 환경과 같이 서버 사이드 네트워크 프로그래밍에도 사용되고 있다. 자바스크립트는 본래 넷스케이프 커뮤니케이션즈 코퍼레이션의 브렌던 아이크(Brendan Eich)가 처음에는 모카(Mocha)라는 이름으로, 나중에는 라이브스크립트(LiveScript)라는 이름으로 개발하였으며, 최종적으로 자바스크립트가 되었다.</h4>
    </p>
    <img src="3.jpg" width="70%"
	</body>
</html>

```

우리는 위처럼 각각의 main, 1, 2, 3 이라는 html 로 작성된 WebPage 를 link 로 역어서 하나의 Website 처럼 만들수 있다. 

## 키워드

Website : Webpage 를 link 로 역어서 구성한 하나의 완성된 사이트로 마치 Page 로 역인 하나의 책과 같다.

Webpage : 하나의 Page 로 이것들을 link 들로 역고 역어서 하나의 Website 가 완성된다.

link : page 와 page , site 와 site 를 연결 시켜주는 방법 이 떄 Tag a 와 href 로 경로 지정을 해준다.

## 참고
[생활코딩](https://opentutorials.org/course/3084/18431)

