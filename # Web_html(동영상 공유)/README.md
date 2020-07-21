# Web_html (동영상 공유)

만약  우리가 동영상을 우리의 Web Page 에 넣고 공유하고 싶다면 어떻게 해야할까?

우리는 유튜브를 통해 동영상을 Web Page 에 넣고 Page 에서 공유 할 수 있도록 할 것이다.

Tag inframe 을 통해서 동영상을 공유 할 수 있게된다.

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

위에 그 전에 만들었던 예제가 있다 이곳에 img 대신에 동영상을 공유 싶다면 아래와 같이 변경해 주면 동영상이 나오게 된다.

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
			<li> <a href="1.html">HTML</a> </li>
			<li> <a href="2.html">CSS</a> </li>
			<li> <a href="3.html">JavaScript</a> </li>
		</ol>

    <a href="https://ko.wikipedia.org/wiki/%EC%9B%94%EB%93%9C_%EC%99%80%EC%9D%B4%EB%93%9C_%EC%9B%B9" target="_blank" title="https://ko.wikipedia.org/wiki/%EC%9B%94%EB%93%9C_%EC%99%80%EC%9D%B4%EB%93%9C_%EC%9B%B9"> <h2> Web</h2> </a>

    <p><h4>월드 와이드 웹(World Wide Web, WWW, W3)은 인터넷에 연결된 컴퓨터를 통해 사람들이 정보를 공유할 수 있는 전 세계적인 정보 공간을 말한다. 간단히 웹(Web)이라 부르는 경우가 많다. 이 용어는 인터넷과 동의어로 쓰이는 경우가 많으나 엄격히 말해 서로 다른 개념이다. 웹은 전자 메일과 같이 인터넷 상에서 동작하는 하나의 서비스일 뿐이다. 그러나 1993년 이래로 웹은 인터넷 구조의 절대적 위치를 차지하고 있다.</h4></p>

    <p>
    <iframe width="670" height="377" src="https://www.youtube.com/embed/7T7r_oSp0SE" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </p>
  </body>
</html>

```

그렇다면 저 코드 즉 소스는 어떻게 알수 있을까? 인터넷 상에 존재하는 모든 동영상에는 소스라는 것이 존재한다.
```
<iframe width="670" height="377" src="https://www.youtube.com/embed/7T7r_oSp0SE" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
```
이것이 동영상을 동영상의 소스인데 이것을 복사해 html 에 Tag 로 입력함으로 공유 할 수있다.

## 키워드

inframe : 동영상을 공유 할 수 있도록 하는 Tag , 인터넷 상의 모든 동영상에는 소스가 존재한다.

## 출처 
[생활코딩](https://opentutorials.org/course/3084/18453)


