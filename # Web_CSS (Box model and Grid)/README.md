# Web_CSS (Box Model and Grid)

## Box Model 

Html 의 Tag 들은 각각의 성격에 따라서 화면 전체를 사용하기도하고 화면의 일부분을 사용하기도 한다.

화면 전체를 사용하는 것이 Block Level Element 라고 말하고, 자신의 부분을 사용하는 것을 Inline Element 라고 일컫는다.

그리고 우리는 이 2가지를 수정하거나 바꿀수 있는다 몇가지의 속성(property) 을 알아보자.

```
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title></title>
    <style>
      h1{
        border:5px solid red;
        padding:20px;
        margin:20px;
        display:inline;
        width:100px;
      }
    </style>
  </head>
  <body>
    <h1>CSS</h1>
    <h1>CSS</h1>
  </body>
</html>
```

위와 같은 Html 코드가 있다. style Tag 에 h1 이 선택자로 선택되어 있고 그안에 여러가지 속성들이 있다.


1. border : Tag 가 가진 공간에 테두리선을 관장하는 Tag 로 width, color, style 등의 value 값을 가진다.

2. padding : Tag 가 가진 테두리와 본문 사이의 공간의 크기를 수정 할 수 있다.(solid 실선)

3. margin : Tag 와 Tag 사이의 있는 공간의 크기를 관장한다.

4. display : 어떠한 Tag 가 가진 표시되는 기본적인 속성을 관장하는 Tag (display : inline, block... 등 으로 사용한다.) 

5. width : Tag 가 가진 공간의 폭을 관장하는 속성

## Grid

Tag 를 사용하다 보면 우리는 디자인 목적을 위해서 본문을 재배치 시켜야 한다 이럴때 사용하는 Tag 가 바로 div, span Tag 이다 우리는 필요한 상황에 맞춰 Tag 를 사용한다.

```
div : div Tag 는 display 가 block level element 이다.  

sapn : span Tag 는 display 가 inline element 이다.
```

위의 두 Tag 는 그저 빈 공간의 Tag 이다.

우리는 이것들을 이용해서 부모 Tag 를 만들고 그 안에 다시 Tag 를 넣어줄수 있다.

```
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title></title>
    <style>
      #grid{
        border:5px solid pink;
        display:grid;
        grid-template-columns: 1fr 2fr;
      }
      div{
        border:5px solid gray;
      }
    </style>
  </head>
  <body>
    <div id="grid">
      <div>NAVIGATION</div>
      <div>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</div>
    </div>
  </body>
</html>
``` 
위의 예문을 보면 우선 부모 div Tag 와 2 개의 자식 Tag 가 있다 부모의 div 는 id 값을 grid 로 주었다

그리고 style Tag 의 border Tag는 예문의 가시성을 높히기 위함이고 우리가 봐야 할것은 다른 속성들이다.

```
#grid{
border:5px solid pink;
display:grid;
grid-template-columns: 150px 1fr;
}
```
1. display : 어떠한 Tag 가 가진 표시되는 기본적인 속성을 관장하는 Tag, 이곳에 Grid 를 Value 값으로 선정한 후에 grid 속성을 이용한다.

2. grid-template-columns : grid 화 된 div 의 공간을 나누어 주는 역할을 한다 px , fr(ex 1/3 구역).


## 활용

``` 
<!DOCTYPE html>
<html><head><meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
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
				border-bottom:  3px skyblue solid;
				margin:0px;
				font-size: 70px;
				padding: 10px;

			}
			ol{
				font-size: 26px;
				border-right: 3px skyblue solid;
				width:160px;
				margin:0px;
				padding : 50px;
	    	padding-top: 30px;

				}
			h2{
				display: inline;
			}

			</style>
	</head>

	<body>
		<h1><a href="file:///Users/choi/Desktop/coding/web/CSS/%23%20Web_CSS%20(Box%20model%20and%20Grid)/main.html"> Web</a></h1>

		<div id="grid">
			<ol>
		      <li> <a href="file:///Users/choi/Desktop/coding/web/CSS/%23%20Web_CSS%20(Box%20model%20and%20Grid)/1.html" class="saw">HTML</a> </li>
		      <li> <a href="file:///Users/choi/Desktop/coding/web/CSS/%23%20Web_CSS%20(Box%20model%20and%20Grid)/2.html" class="saw" id="now">CSS</a> </li>
		      <li> <a href="file:///Users/choi/Desktop/coding/web/CSS/%23%20Web_CSS%20(Box%20model%20and%20Grid)/3.html">JavaScript</a> </li>
		  </ol>

			<div>
				<br>
	    	<h2>CSS <a href="https://ko.wikipedia.org/wiki/%EC%A2%85%EC%86%8D%ED%98%95_%EC%8B%9C%ED%8A%B8" target="_blank" title="https://ko.wikipedia.org/wiki/%EC%A2%85%EC%86%8D%ED%98%95_%EC%8B%9C%ED%8A%B8" id="CSShref"><strong>C</strong>ascading <strong>S</strong>tyle <strong>S</strong>heets</a></h2>
				<p>
		      종속형 시트 또는 캐스케이딩 스타일 시트(Cascading Style Sheets, CSS)는 마크업 언어가 실제 표시되는 방법을 기술하는 언어로, HTML과 XHTML에 주로 쓰이며, XML에서도 사용할 수 있다. W3C의 표준이며, 레이아웃과 스타일을 정의할 때의 자유도가 높다.

		      마크업 언어(ex. HTML)가 웹사이트의 몸체를 담당한다면 CSS는 옷과 액세서리 같은 꾸미는 역할을 담당한다고 할 수 있다. 즉, HTML 구조는 그대로 두고 CSS 파일만 변경해도 전혀 다른 웹사이트처럼 꾸밀 수 있다.

		      현재 개발 중인 CSS3의 경우 그림자 효과, 그라데이션, 변형 등 그래픽 편집 프로그램으로 제작한 이미지를 대체할 수 있는 기능이 추가되었다. 또한 다양한 애니메이션 기능이 추가되어 어도비 플래시를 어느 정도 대체하고 있다.
		    </p>
		    <br><br>
		    <img src="./2_files/2.jpg" width="70%">
			</div>
		</div>
</body></html>

```

* 그리고 Web page 에서 검사를 통해서도 CSS 변화가 가능하며 그것또한 저장이 가능하다.

## 참고
[생활코딩](https://opentutorials.org/course/3086/18322)
