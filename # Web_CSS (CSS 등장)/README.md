# Web_CSS

Html 은 Web 이 등장하면서 생긴 첫 기능이다, 그러나 사람들은 이 Html 로 정보를 표현하면서 조금 더 정보를 구체적으로 표현하고 싶어했다

예를 들어 글씨의 모양과 크기, Divison 등등 이 CSS 라는것은 직접적인 정보를 담고있지 않다.

Html 같은경우에는 직접적으로 정보를 전달하는 기능이지만 이 CSS 는 정보를 전달하는 주체보단 그 정보 전달을 조금더 가독성을 좋게 만들어 주는 역할을 한다.

## CSS의 등장

Web 에서 Html 은 정말 중요한 역할을 하고 있다 그것은 바로 정보를 전달하는 가장 본질적이고 중요한 역할이다

하지만 사람들은 시간이 지남에 따라 가독성과 디자인에 신경을 쓰게 되었고 CSS와 Html 을 구분지어 서로가 서로의 역할에 침범하지 않고 상호작용을 할 수 있도록 고안하였다.

## style 활용

Web browser 가 처음 나왔을때 어떤 컴퓨터 언어만을 해석 할 수 있었을까? 바로 Html 이다.

그리고 CSS는 Html 과는 완전히 다른 컴퓨터 언어이다 그렇다면 어떻게 Web browser 에게 CSS 를 입력 시킬수 있을까?

바로 style 이다 , 이 Tag 는 Html 문법이지만 이 Style 안쪽으로 위치하는 코드들은 CSS 문법으로 인시하여라 라는 의미를 가진 Tag 이다.

우리가 a 라는 Tag 를 가진 모든 글자를 빨간색으로 바꾸고 싶다면 어떻게 해야할까? 우리는 그떄 Style Tag 를 사용 할 수있다.


```
<style>
	a {
		color : red;
	}

</style>

```

위와 같이 작성을 해주면 Tag Style = CSS 문법으로 해석하여라 , a {} = a 코드의 글씨를 , color : red ; = 빨간색으로 바꾸어라

그럼 한번 우리가 Html 에서 작성했던 코드에 적용시켜보자.

```
<!doctype html>
<html>
	<head>
		<title> Web html </title>
		<mata charset="utf-8">
	<style>
		a {
			color : red;
		}
	</style>

	</head>

	<body>
		<h1><a href="main.html"> Main</a></h1>

		<ol>
			<li> <a href="1.html">HTML</a> </li>
			<li> <a href="2.html">CSS</a> </li>
			<li> <a href="3.html">JavaScript</a> </li>
		</ol>

    <a href="https://ko.wikipedia.org/wiki/%EC%9B%94%EB%93%9C_%EC%99%80%EC%9D%B4%EB%93%9C_%EC%9B%B9" target="_blank" title="https://ko.wikipedia.org/wiki/%EC%9B%94%EB%93%9C_%EC%99%80%EC%9D%B4%EB%93%9C_%EC%9B%B9"> <h2> Web</h2> </a>

    <p><h4>월드 와이드 웹(World Wide Web, WWW, W3)은 인터넷에 연결된 컴퓨터를 통해 사람들이 정보를 공유할 수 있는 전 세계적인 정보 공간을 말한다. 간단히 웹(Web)이라 부르는 경우가 많다. 이 용어는 인터넷과 동의어로 쓰이는 경우가 많으나 엄격히 말해 서로 다른 개념이다. 웹은 전자 메일과 같이 인터넷 상에서 동작하는 하나의 서비스일 뿐이다. 그러나 1993년 이래로 웹은 인터넷 구조의 절대적 위치를 차지하고 있다.</h4></p>
    <br><br>
    <img src="main.jpg" width="70%">
	</body>
</html>
```

위와 같이 적용을 시켜주면 Tag a 의 글씨는 모두 빨간색으로 변경 되었다.

## 키워드

CSS : Cascading Style Sheets 의 약자로 Html 처럼 정보를 전달하는 역할보단 조금 더 보기 편하도록 디자인 혹은 가독성이 좋도록 보조해주는 언어

Tag a : 마치 하이퍼링크같이 다른 Web Page 로 연결해주는 Tag 이다.

Tag style : Html Tag 이지만 그 안쪽의 코드는 CSS 문법으로 처리하라는 Tag

## 참고

[생활코딩](https://opentutorials.org/course/3086/18312)