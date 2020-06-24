# Web_html (link)

현재 Tag 약 150개 이다 그러나 link 는 그중에서도 가장 상위라고 할 수 있다.

HTML 의 약자 Hyper Text Markup Language 의 Hyper Text 가 바로 이 link 를 의미한다.

## 1. link

link 는 무엇일까? 정보와 정보를 연결하는 역할을 하는 link 는 링크를 사용했을때 다른 링크가 걸어진 다른 Web 으로 연결이 된.

```
파일명 : 1.html

<!doctype html>
<html>
	<head>
		<title> Web html </title>
		<mata charset="utf-8">
	</head>

	<body>
		<ol>
			<li> HTML</li>
			<li> CSS</li>
			<li> JavaScript</li>
		</ol>
		<ol>
			<li> Java </li>
			<li> Python </li>
			<li> MySQL </li>
		</ol>

		<h1>HTML 이란 무엇인가? </h1>

		<p><h4>HTML</h4></p>
		<p> <strong> H</strong>yper <strong>T</strong>ext <strong>M</strong>arkup <strong>L</strong>anguage</p>
		<img src="1.jpg" width="100%">
		
	</body>
</html>

```

이러한 Web 에서 Hyper Text Markup Language 이곳에 Html 을 설명하는 링크를 연결하고 싶다면 어떻게 할 수 있을까?

링크를 만드는데 필요한 Tag 는 a 이다. 

```
파일명 : 2.html


<!doctype html>
<html>
	<head>
		<title> Web html </title>
		<mata charset="utf-8">
	</head>

	<body>
		<ol>
			<li> HTML</li>
			<li> CSS</li>
			<li> JavaScript</li>
		</ol>
		<ol>
			<li> Java </li>
			<li> Python </li>
			<li> MySQL </li>
		</ol>

		<h1>HTML 이란 무엇인가? </h1>

		<p><h4>HTML</h4></p>
		<p> <a href="https://terms.naver.com/entry.nhn?docId=1168097&cid=40942&categoryId=32838" target="_blank" title="https://terms.naver.com/entry.nhn?docId=1168097&cid=40942&categoryId=32838"> <strong> H</strong>yperT</strong>ext <strong>M</strong>arkup <strong>L</strong>anguage</a></p>
		<img src="1.jpg" width="100%">

	</body>
</html>

```

위와 같이 링크를 연결하고 싶은 곳에 a 를 통해 묶어주고 그 뒤에 h(hypertext)ref(refernce) = "add" 를 입력해주면 링크가 걸린다.

* 그리고 만약 새로운 페이지에서 연결된 link 를 열고 싶다면 target = "_blank" 를 통해 새로운 페이지로 열 수 있다.

## 키워드

link : Tag a 를 통해서 표현하며 페이지와 페이지를 연결시켜주는 역할을 힌다.

a :  link 를 걸어줄때 쓰이는 Tag

href : h(hypertext)ref(refernce) = "add" 로 add 부분에 주소를 넣어주면 그곳을 참조해라 즉 연결해라 라는 뜻이다.

target : target = "_blank" 만약 link 로 연결할시 새로운 페이지에 연결하라는 명령

title : title="info"
만약 a 뒤에 title 을 넣는다면 tooltip 으로서 링크가 어디로 연결 되는지 확인 할 수 있도록 표시된다. 

## 참고
[생활코딩](https://opentutorials.org/course/3084/18418)
