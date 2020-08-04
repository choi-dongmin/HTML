Web_CSS (속성과 선택자)

CSS 를 사용하려면 속성, 선택자 2가지중 1가지를 알아야 사용 할 수 있다, 이번에는 몇가지의 속성을 알아보고 그것을 활용해서 적용 할 것이다.

만약 우리가 Web 이라는 h1 Tag 로 묶인 제목과 같은 가장 큰 글자 Web 을 CSS 를 통해 변화를 주고 싶다면 어떻게 할 수 있을까?

```
<!doctype html>
<html>
	<head>
		<title> Web html </title>
		<mata charset="utf-8">
		<style>
			a {
				color : black

			}
		</style>
	</head>

	<body>
		<h1><a href="main.html"> Web </a></h1>

		<ol>
			<li> <a href="1.html">HTML</a> </li>
			<li> <a href="2.html" style="color:red">CSS</a> </li>
			<li> <a href="3.html">JavaScript</a> </li>
		</ol>

    <a href="https://ko.wikipedia.org/wiki/%EC%9B%94%EB%93%9C_%EC%99%80%EC%9D%B4%EB%93%9C_%EC%9B%B9" target="_blank" title="https://ko.wikipedia.org/wiki/%EC%9B%94%EB%93%9C_%EC%99%80%EC%9D%B4%EB%93%9C_%EC%9B%B9"> <h2> Web</h2> </a>

    <p><h4>월드 와이드 웹(World Wide Web, WWW, W3)은 인터넷에 연결된 컴퓨터를 통해 사람들이 정보를 공유할 수 있는 전 세계적인 정보 공간을 말한다. 간단히 웹(Web)이라 부르는 경우가 많다. 이 용어는 인터넷과 동의어로 쓰이는 경우가 많으나 엄격히 말해 서로 다른 개념이다. 웹은 전자 메일과 같이 인터넷 상에서 동작하는 하나의 서비스일 뿐이다. 그러나 1993년 이래로 웹은 인터넷 구조의 절대적 위치를 차지하고 있다.</h4></p>
    <br><br>
    <img src="main.jpg" width="70%">
	</body>
</html>
```

먼저 위의 코드에서 우리가 변화를 주고 싶은 부분은 Web 이라는 글로 표시된 부분이다 그 부분은 곧 h1 tag 에 속해 있다는것을 볼 수 있다.

그렇다면 우리는 style Tag 에서 선택자를 h1{ } 를 통해 지정 할 수있다.

그리고 우리가 h1 Tag 에 속한 글자의 크기를 조절하고 싶다면 우리는 CSS text size property 이렇게 검색 할 수 있을것이다.

우리는 속성을 찾아볼수 있다 글자의 크기를 조절하는 것은 font-size 라는 속성을 이용해야한다.    

그리고 우리는 그 제목을 가운데 정렬을 하고 싶다면 또 어떻게 해야할까? 우리는 다시한번 이렇게 검색 할 수 있을것이다.

CSS text center property 그러면 우리는 text-align 을 찾을수 있을 것이다 그러면 우리는 정렬을 할 수 있게된다.

그 외에도 글자의 밑줄을 관리하는 text-decoration 속성을 이용한다면 아래와 같은 CSS Tag 를 만들수 있을것이다.

```
<style>
	a {
		color : black;
		text-decoration:none;
	}
	h1 {
		text-size : 75px;
		text-align:center;
	}
</style>
``` 
위의 방식으로 우리는 제목의 디자인을 간단히 바꿀수 있었다.

## 선택자 (class, id)

```
파일명 : 2.html

<!doctype html>
<html>
	<head>
		<style>
			#now{
					color : red
			}

			a{
				color : black;
				text-decoration : none;
			}
			.saw{
				color : gray
			}
		</style>

    <h1><a href="main.html"> Web</a></h1>

    <ol>
      <li> <a href="1.html" class="saw">HTML</a> </li>
      <li> <a href="2.html" class="saw" id="now">CSS</a> </li>
      <li> <a href="3.html">JavaScript</a> </li>
    </ol>
	</head>
	<body>
    <h2>CSS </h2>

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
* 위의 예문은 우리가 이 전 예문에서 필요한 부분만 남긴것이다.

예문에는 지금 모든 글씨가 검은색이다 , 만약 우리가 HTML, CSS 를 설명하는 Page 를 링크를 통해 이미 방문했고 

그 Page 가 이미 방문한 Page 라는것을 회색으로 표현하고 싶다면 어떻게 해야할까?

그럴때 우리는 속성을 이용해서 문제를 처리 할 수 있다.

```
<body>
	<h1><a href="main.html"> Main</a></h1>
	<ol>
		<li> <a href="1.html" style="color : gray" >HTML</a> </li>
		<li> <a href="2.html" style="color : gray" >CSS</a> </li>
		<li> <a href="3.html">JavaScript</a> </li>
	</ol>
</body>
``` 

위와같이 한다면 해결 될 것이다 그러나 위 코드는 중복이 발생하였다 그래서 우리는 "class" 라는 것을 이용해서 중복을 제거 할수있다.

## class

class 는 여러 코드를 하나의 집합으로 묶어주는 역할을 한다.
```
 <body>
	<h1><a href="main.html"> Main</a></h1>
	<ol>
		<li> <a href="1.html" class="saw" >HTML</a> </li>
		<li> <a href="2.html" class="saw" >CSS</a> </li>
		<li> <a href="3.html">JavaScript</a> </li>
	</ol>
</body>
```

위와 같이 saw 라는 class 를 만들면서 CSS, HTML 을 포함 시켰다.

그 다음 우리는 위의 style Tag 에서 한번에 saw class 를 지정해서 명령을 내릴수 있다.

```
<!doctype html>
<html>
	<head>
		<style>
			a{
				color : black;
				text-decoration : none;
			}
			.saw{
				color : gray
			}
		</style>

    <h1><a href="main.html"> Web</a></h1>

    <ol>
      <li> <a href="1.html" class="saw">HTML</a> </li>
      <li> <a href="2.html" class="saw">CSS</a> </li>
      <li> <a href="3.html">JavaScript</a> </li>
    </ol>
	</head>
	<body>
    <h2>CSS </h2>

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

위와 같이 style Tag 에서 saw class 를 지정해서 회색으로 바꾸어주고 있다 그런데 saw 앞에 . 이 있는것을 볼 수있다.

이것은 하나의 약속과도 같은것 인데 만약 우리가 지정한 class 를 선택자로 쓰고 싶다면 우리는 class 이름앞에 . 을 붙여야한다.

만약 또 우리가 지금 CSS 라는 Page 에 있고 현재있는 Page 의 색을 붉은색으로 표시하고 싶다면 어떻게 해야할까?

```
<!doctype html>
<html>
	<head>
		<style>
			a{
				color : black;
				text-decoration : none;
			}
			.saw{
				color : gray
			}
			.now{
				color : red
			}

		</style>

    <h1><a href="main.html"> Web</a></h1>

    <ol>
      <li> <a href="1.html" class="saw">HTML</a> </li>
      <li> <a href="2.html" class="saw now">CSS</a> </li>
      <li> <a href="3.html">JavaScript</a> </li>
    </ol>
	</head>
	<body>
    <h2>CSS </h2>

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

위의 예문을 보면 CSS Tag 의 class 는 2가지가 있다 saw , now 먼저 위 예문을 정상적으로 잘 작동한다

그로인해 우리가 알수 있는건 한개의 Tag 에 복수의 class 를 가질수 있다는것이며 saw 는 now 보다 우선순위가 낮다는것을 알수있다.

그건 now 라는 class 가 Style Tag 에서 더 늦게 나왔기 때문이다 또한 일반 선택자와 class 선택자가 있다면 우선순위는 class 선택자가 높다

그말은 만약 코드가 바뀌거나 후에 다른 Tag 가 중복되는 class 가 있다면 now 는 순위에서 밀리게 된다 그렇다면 이것을 어떻게 해결할까?

이럴때 우리는 id 라는것을 사용한다.

## id

id 는 하나의 Page 에 여러 id가 존재 할 수있다 하지만 그 값은 중복 되어서는 안된다, 그 말을 X page 에 x,y id 가 존재 할 수있지만 x,x id는 존재 할 수 없다는 것이다.  


```
<!doctype html>
<html>
	<head>
		<style>
			#now{
					color : red
			}

			a{
				color : black;
				text-decoration : none;
			}
			.saw{
				color : gray
			}
		</style>

    <h1><a href="main.html"> Web</a></h1>

    <ol>
      <li> <a href="1.html" class="saw">HTML</a> </li>
      <li> <a href="2.html" class="saw" id="now">CSS</a> </li>
      <li> <a href="3.html">JavaScript</a> </li>
    </ol>
	</head>
	<body>
    <h2>CSS </h2>

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
위 예문을 보면 CSS Tag 에 id 를 now 로 지정했다는 것과 style Tag 에서 #now 로 선택자로 지정하고 있는것을 알 수 있다..

위 예문도 우리가 원하는것 처럼 CSS 를 빨간색으로 출력이 된다, 그 말은 id 선택자가 class 선택자 보다 우선순위가 높은것을 알 수 있다.

즉, 우선순위는 Tag 선택자 -> class 선택자 -> id 선택자 순서로 높다는것을 알수있다. 

개발자들은 더 포괄하는 범위가 작을 수록 더 우선순위를 높게 만들었다. 


## 키워드

text - size : 글자의 크기를 조절하는 속성

text - align : 글자의 위치를 정렬하는 속성

text - decoration : 글지의 밑줄을 변경하는 속성

class : 지정한 Tag 들을 묶어서 하나의 집합의 형태로 만드는것 style Tag 에서 선택자로 사용하고 싶다면 . 을 써줘야 한다.

id : 지정한 Tag 가 유일한 Tag id 를 같도록 지정해 주는것을 의미한다. 

## 참고
[생활코딩](https://opentutorials.org/course/3086/18318)