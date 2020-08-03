# Web_CSS (기본문법과 변화)

## 기본문법

Html 과 CSS 는 완전히 다른 언어이기 때문에 Web Browser 로 하여금 어디에서 부터 어디까지가 가장 CSS 언어인지 확인시켜주어야 한다.

그때 사용하는 Tag 가 바로 Style 이라는 것이다, 그런데 이 Tag 를 이용하는것이 아닌 속성을 이용해서 하는 방법도 있다.

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
* 위의 방법이 Tag 를 이용한 방법이다.

```

<!doctype html>
<html>
	<head>
		<title> Web html </title>
		<mata charset="utf-8">
	</head>

	<body>
		<h1><a href="main.html"> Main</a></h1>

		<ol>
			<li> <a href="1.html" style="color:red">HTML</a> </li>
			<li> <a href="2.html" style="color:red">CSS</a> </li>
			<li> <a href="3.html" style="color:red">JavaScript</a> </li>
		</ol>

    <a href="https://ko.wikipedia.org/wiki/%EC%9B%94%EB%93%9C_%EC%99%80%EC%9D%B4%EB%93%9C_%EC%9B%B9" target="_blank" title="https://ko.wikipedia.org/wiki/%EC%9B%94%EB%93%9C_%EC%99%80%EC%9D%B4%EB%93%9C_%EC%9B%B9"> <h2> Web</h2> </a>

    <p><h4>월드 와이드 웹(World Wide Web, WWW, W3)은 인터넷에 연결된 컴퓨터를 통해 사람들이 정보를 공유할 수 있는 전 세계적인 정보 공간을 말한다. 간단히 웹(Web)이라 부르는 경우가 많다. 이 용어는 인터넷과 동의어로 쓰이는 경우가 많으나 엄격히 말해 서로 다른 개념이다. 웹은 전자 메일과 같이 인터넷 상에서 동작하는 하나의 서비스일 뿐이다. 그러나 1993년 이래로 웹은 인터넷 구조의 절대적 위치를 차지하고 있다.</h4></p>
    <br><br>
    <img src="main.jpg" width="70%">
	</body>
</html>

```
* 위의 방법이 속성을 사용한것이다.

이렇게 Web Page 에 CSS 를 적용하는 방법은 2가지이다 Tag 를 이용해서 적용하는것 , 속성을 이용하는 방법

Html 의 개발자들은 style 이라는 속성이 시작되면 그 안에 위치한 문법을 CSS 방식으로 처리를 하도록 했다.

style="xx" 이곳이 html 적인 속성이고 그 안쪽의 color : red 는 CSS 적인 문법이다.

그러나 우리는 같인 style 임에도 같고 다른점을 볼수 있다.

```
<li> <a href="1.html" style="color:red">HTML</a> </li>
<li> <a href="2.html" style="color:red">CSS</a> </li>
<li> <a href="3.html" style="color:red">JavaScript</a> </li>
--------------------------------------------------------------
<head>
	<title> Web html </title>
	<mata charset="utf-8">
	<style>
		a {
			color : red;
		}
	</style>
</head>
```

위는 속성 아래는 Tag 이다, Tag 와 속성 style 모두 color : red 라는 CSS 적 문법을 가지고 있다 그러나 속성은 자신이 원하는 위치에 style 을 적용시키고

Tag 같은 경우 따로 어떤 위치에 CSS 효과를 적용 할 것인지 선택 해주어야 한다, 그러한 것들을 선택자 (selecter) 라고 한다 (위 경우 a{}).

정리하면 Tag 를 통해 CSS 효과를 주고 싶다면 선택자를 통해 어디에 적용 할 것인가 지정해주어야 하고 속성을 이용할 때는 속성이 위치한 Tag 에 적용이 된다.

## 키워드

Tag 를 이용한 CSS : style Tag 이용해 CSS 문법을 읽는 방식으로 선택자를 통해 지정한 위치에 적용한다.

속성을 이용한 CSS : Style 속성을 이용해 CSS 문법을 읽는 방식으로 속성이 위치한 Tag에 적용시킨다.

## 참고
[생활코딩](https://opentutorials.org/course/3086/18318)  

