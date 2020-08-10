# Web_html (코드의 재사용)

모든 정보가 그러하듯 CSS 도 나혼자만 사용하는것이 아닌 다른 사용자와 같이 나눌떄 그 효과가 최대한으로 커질수 있게 된다.

하지만 이렇게 생각 할 수도 있다 지금 우리는 모든 Web Page 에 각각 하나의 CSS style Tag 를 적용시키고 있다.

그렇다면 이것은 중복이다 그래서 우리는 CSS style Tag 의 안에 코드들을 따로 모아두어서 각각의 Page 에서 불러올수 있도록 만들고 싶다면 어떨까?

```
			#grid{
				display: grid;
				grid-template-columns: 300px 1fr
			}
			#now{
					color : red
			}
			#CSShref{
				font-size: 15px
			}
			a{
				color : black;
				text-decoration : none;
			}
			.saw{
				color : gray
			}
			h1{
				text-align: center;
				border-bottom:  3px gray solid;
				margin:0px;
				font-size: 70px;
				padding: 10px;

			}
			ol{
				font-size: 26px;
				border-right: 3px gray solid;
				width:160px;
				margin:0px;
				padding : 50px;
	    	padding-top: 30px;

				}
			h2{
				display: inline;
			}
			@media(max-width:800px) {
				#grid{
					display: block;
				}
				ol{
					border-right: none;
					padding : 20px;
				}
				h1{
					border-bottom: none;
					padding: 0px;
				}
			}
```

위와 같이 style Tag 안쪽의 코드를 따로 style.css 라는 파일에 저장을 해두었다.

그리고 우리는 이전 Page 들의 style Tag 가 있던 자리에 style.css 파일을 불러오라는 명령을 해주면 된다.

우리는 기능을 사용할때 link 라는 Tag 를 이용할것이다.
```

<!DOCTYPE html>
<html>
	<head>
		<meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
		<style>
			#grid{
				display: grid;
				grid-template-columns: 300px 1fr
			}
			#now{
					color : red
			}
			#CSShref{
				font-size: 15px
			}
			a{
				color : black;
				text-decoration : none;
			}
			.saw{
				color : gray
			}
			h1{
				text-align: center;
				border-bottom:  3px gray solid;
				margin:0px;
				font-size: 70px;
				padding: 10px;

			}
			ol{
				font-size: 26px;
				border-right: 3px gray solid;
				width:160px;
				margin:0px;
				padding : 50px;
	    	padding-top: 30px;

				}
			h2{
				display: inline;
			}
			@media(max-width:800px) {
				#grid{
					display: block;
				}
				ol{
					border-right: none;
					padding : 20px;
				}
				h1{
					border-bottom: none;
					padding: 0px;
				}
			}

			</style>
	</head>

	<body>
		<h1><a href="file:///Users/choi/Desktop/coding/web/CSS/%23%20Web_CSS(%E1%84%8F%E1%85%A9%E1%84%83%E1%85%B3%E1%84%8B%E1%85%B4%20%E1%84%8C%E1%85%A2%E1%84%89%E1%85%A1%E1%84%8B%E1%85%AD%E1%86%BC)/main.html"> Web</a></h1>

		<div id="grid">
			<ol>
				<li> <a href="file:///Users/choi/Desktop/coding/web/CSS/%23%20Web_CSS(%E1%84%8F%E1%85%A9%E1%84%83%E1%85%B3%E1%84%8B%E1%85%B4%20%E1%84%8C%E1%85%A2%E1%84%89%E1%85%A1%E1%84%8B%E1%85%AD%E1%86%BC)/1.html" class="saw">HTML</a> </li>
				<li> <a href="file:///Users/choi/Desktop/coding/web/CSS/%23%20Web_CSS(%E1%84%8F%E1%85%A9%E1%84%83%E1%85%B3%E1%84%8B%E1%85%B4%20%E1%84%8C%E1%85%A2%E1%84%89%E1%85%A1%E1%84%8B%E1%85%AD%E1%86%BC)/2.html" class="saw" id="now">CSS</a> </li>
				<li> <a href="file:///Users/choi/Desktop/coding/web/CSS/%23%20Web_CSS(%E1%84%8F%E1%85%A9%E1%84%83%E1%85%B3%E1%84%8B%E1%85%B4%20%E1%84%8C%E1%85%A2%E1%84%89%E1%85%A1%E1%84%8B%E1%85%AD%E1%86%BC)/3.html">  JavaScript </a> </li>
			 </ol>

			<div>
				<br>
				<a href="https://ko.wikipedia.org/wiki/%EC%9B%94%EB%93%9C_%EC%99%80%EC%9D%B4%EB%93%9C_%EC%9B%B9" target="_blank" title="https://ko.wikipedia.org/wiki/%EC%9B%94%EB%93%9C_%EC%99%80%EC%9D%B4%EB%93%9C_%EC%9B%B9"> <h2> Web</h2> </a>

		    <p><h4>월드 와이드 웹(World Wide Web, WWW, W3)은 인터넷에 연결된 컴퓨터를 통해 사람들이 정보를 공유할 수 있는 전 세계적인 정보 공간을 말한다. 간단히 웹(Web)이라 부르는 경우가 많다. 이 용어는 인터넷과 동의어로 쓰이는 경우가 많으나 엄격히 말해 서로 다른 개념이다. 웹은 전자 메일과 같이 인터넷 상에서 동작하는 하나의 서비스일 뿐이다. 그러나 1993년 이래로 웹은 인터넷 구조의 절대적 위치를 차지하고 있다.</h4></p>
		    <br><br>
		    <img src="main.jpg" width="70%">
			</div>
		</div>
	</body>
</html>

```
위와 같은 코드를 아래와 같이 바꾸어 줌으로 훨씬 더 효율적인 코드가 완성되었다.

```

<!DOCTYPE html>
<html>
	<head>
		<meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
		<link rel="stylesheet" href="style.css">
	</head>

	<body>
		<h1><a href="file:///Users/choi/Desktop/coding/web/CSS/%23%20Web_CSS(%E1%84%8F%E1%85%A9%E1%84%83%E1%85%B3%E1%84%8B%E1%85%B4%20%E1%84%8C%E1%85%A2%E1%84%89%E1%85%A1%E1%84%8B%E1%85%AD%E1%86%BC)/main.html"> Web</a></h1>

		<div id="grid">
			<ol>
				<li> <a href="file:///Users/choi/Desktop/coding/web/CSS/%23%20Web_CSS(%E1%84%8F%E1%85%A9%E1%84%83%E1%85%B3%E1%84%8B%E1%85%B4%20%E1%84%8C%E1%85%A2%E1%84%89%E1%85%A1%E1%84%8B%E1%85%AD%E1%86%BC)/1.html" class="saw">HTML</a> </li>
				<li> <a href="file:///Users/choi/Desktop/coding/web/CSS/%23%20Web_CSS(%E1%84%8F%E1%85%A9%E1%84%83%E1%85%B3%E1%84%8B%E1%85%B4%20%E1%84%8C%E1%85%A2%E1%84%89%E1%85%A1%E1%84%8B%E1%85%AD%E1%86%BC)/2.html" class="saw" id="now">CSS</a> </li>
				<li> <a href="file:///Users/choi/Desktop/coding/web/CSS/%23%20Web_CSS(%E1%84%8F%E1%85%A9%E1%84%83%E1%85%B3%E1%84%8B%E1%85%B4%20%E1%84%8C%E1%85%A2%E1%84%89%E1%85%A1%E1%84%8B%E1%85%AD%E1%86%BC)/3.html">  JavaScript </a> </li>
			 </ol>

			<div>
				<br>
				<a href="https://ko.wikipedia.org/wiki/%EC%9B%94%EB%93%9C_%EC%99%80%EC%9D%B4%EB%93%9C_%EC%9B%B9" target="_blank" title="https://ko.wikipedia.org/wiki/%EC%9B%94%EB%93%9C_%EC%99%80%EC%9D%B4%EB%93%9C_%EC%9B%B9"> <h2> Web</h2> </a>

		    <p><h4>월드 와이드 웹(World Wide Web, WWW, W3)은 인터넷에 연결된 컴퓨터를 통해 사람들이 정보를 공유할 수 있는 전 세계적인 정보 공간을 말한다. 간단히 웹(Web)이라 부르는 경우가 많다. 이 용어는 인터넷과 동의어로 쓰이는 경우가 많으나 엄격히 말해 서로 다른 개념이다. 웹은 전자 메일과 같이 인터넷 상에서 동작하는 하나의 서비스일 뿐이다. 그러나 1993년 이래로 웹은 인터넷 구조의 절대적 위치를 차지하고 있다.</h4></p>
		    <br><br>
		    <img src="main.jpg" width="70%">
			</div>
		</div>
	</body>
</html>

``` 

## 키워드

link : link Tag 는 CSS 파일을 다운받아 코드상에서 사용할수있도록 해주는 기능을 말한다.

## 참고

[생활코딩](https://opentutorials.org/course/3086/18327)

