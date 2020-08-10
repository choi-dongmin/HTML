## Web_html (media query)

현대적인 Web 을 만드는데 있어 반응형 디자인이라고 하는것을 알아 볼 것이다.

그렇다면 반응형 디자인은 무엇을까? 반응형 디자인이란 Web 의 화면의 크기에 따라서 디자인이 바뀌도록  하는 기능이다.

간단한 예로 Desktop 에서 보는 화면과 휴대전화에서 사용하는 화면이 같지 않다는것을 우리는 알 수 있다,

이렇듯 각각의 화면에 따라 Web 이 반응하여 기능을 변경하는 기능을 Media Query 그리고 그것을 우리는 반응형 디자인 , 반응형 Web 이라고 일컫는다.

```
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title></title>
    <style>
      div{
        border:10px solid green;
        font-size:60px;
      }
      @media(max-width:800px) {
        div{
          display:none;
        }
      }
    </style>
  </head>
  <body>
    <div>
      Responsive
    </div>
  </body>
</html>
```

위의 예문을 보면 본문에 div 를 만들고 그 안쪽에 Responsive 라는 글자를 넣었다 그리고 Style Tag에서

div 의 가시성을 높이고자 초록색 실선을 넣었다.

```
@media(max-width:800px) {
        div{
          display:none;
        }
      }
```

그리고 이 부분이 바로 media query 이다 위 예문에서는 위 문장은 이렇게 해석 할수있다.

 "화면의 너비가 800px 보다 크면 div 의 display 는 없다".(min-width : 800px / 화면의 너비가 800px 보다 작으면 display none 을 하여라)


## 활용
```
파일명 : 2.html
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

## 키워드

미디어 쿼리 : 화면에 따라 Web 이 반응하여 기능을 변경하는 기능을 Media Query 라고 일컫는다. 

반응형 웹 : 웹의 기능을 화면이 변화함에 따라 같이 변화시키는 기능

## 참고
[생활코딩](https://opentutorials.org/course/3086/18323)

