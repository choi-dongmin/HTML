# 문서의 구조

예를들면 지금까지 우리는 하나의 문장을 완성 시키는 법을 공부했다 그리고 그 문장들은 하나의 페이지가 되고 하나의 페이지는 한권의 책이된다.

이 구조에 대해서 알아보고 또 Web 을 사용하면서 가장 많이 사용하는 Tag 5가지를 알아보자.


## 1. title 

만들어온 Web 에는 아직 명확한 제목이 없다(Web Page) 그래서 우리는 title 이라는 Tag 를 이용해서 제목을 만들어 줄것이다.


```
파일명 : 1.html

<title> Web html </title>

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

<h1>Web_html</h1>

<p>Hello World , This is just practice for my Web_html.</p>
<img src="1.jpg" width="100%">
<p>This is practice <strong> <u>Not Real </u> </strong>  And you can't see this page.</p>

```  

위와 같이 title Tag 를 사용하면 Web Page 의 공식적인 제목을 설정 할 수있다.

제목을 만드는것은 정말로 중요한 일이다 단순히 하나의 페이지에 제목을 짓는게 아니다, 만약 누군가 검색엔진에 검색을 한다고 하자

그러면 그 엔진은 Title 을 제일 먼저 검색을 해서 결과를 보여준다 그만큼 제목을 만들어 주는것은 중요한 일이고 해야하는 일이다.

## 2. mata

```
파일명 : 2.html

<title> Web html </title>

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

<p>Hello World , This is just practice for my Web_html.</p>
<img src="1.jpg" width="100%">
<p>This is practice <strong> <u>Not Real </u> </strong>  And you can't see this page.</p>

```  
만약 이러한 Page 가 있다고 해보자 그렇다면 아마 "HTML 이란 무엇인가?" 이 부분이 이상한 글자로 나오는것을 볼 수 있을것이다.

그것은 컴퓨터는 2진법으로 저장하고 불러오는 과정에서 생기는 오류이다 그렇다면 어떻게 하면 해결 할 수있을까?

바로 그 파일에게 직접 불러울 형식을 지정해주는 것이다.

필자는 Atom 을 사용하고 UTF-8 이라는 형식으로 작성했음으로 Web 에게 UTF-8 으로 불러오라는 Tag를 작성 할 것이다.

그렇다면 Web browser 에서도 UTF-8 형식으로 불러옴으로 오류가 없을것이다.

```
파일명 : 3.html

<title> Web html </title>
<mata charset="utf-8">


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

<p>Hello World , This is just practice for my Web_html.</p>
<img src="1.jpg" width="100%">
<p>This is practice <strong> <u>Not Real </u> </strong>  And you can't see this page.</p>

```  

mata charset="utf-8" 이 부분을 추가 해주었다. char 은 문자형식 set 은 설정 utf-8 형태로 라는 뜻을 가진 Tag 이다.


지금 배운 title, mata 와 본문과는 다르다 이 두가지는 본문을 설명해주는 역할을 한다.

title 은 본문의 내용을 mata 는 본문이 어떠한 형식으로 저장되었는가 알려주는 역할을 한다.


## 3. body, head

이제 우린는 본문과 아닌것을 알았다 그래서 Web 사용자들은 본문에 body 를, 설명에 head 를 작성해 주도록 약속을 하였다.

```
파일명 : 4.html

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

	<p>Hello World , This is just practice for my Web_html.</p>
	<img src="1.jpg" width="100%">
	<p>This is practice <strong> <u>Not Real </u> </strong>  And you can't see this page.</p>
</body>

```  

즉 html 의 대다수의 Tag 는 head tag 또는 body tag 아래에 놓이게 된다는것이다.

## 4. html

body, head 에 안에 놓이지 않는 Tag 가 하나 있는데 그것이 바로 html Tag 이다.

html 이 가장 상위에서 head 와 body 를 묶어주는 역할을 한다.

그리고 이 문서가 html 이라는 것을 알리기 위해 약속적으로 !doctype html 이라는 것을 말머리에 명시해준다.


```
파일명 : 5.html
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

		<p>Hello World , This is just practice for my Web_html.</p>
		<img src="1.jpg" width="100%">
		<p>This is practice <strong> <u>Not Real </u> </strong>  And you can't see this page.</p>
	</body>
</html>
```
 
## 키워드

title : Web Page 의 제목을 지정해주는 Tag.

mata : web browser 에 파일을 불러올때 어떠한 형식으로 불러올 것인지 지정하게 해주는 Tag.

head : 본문을 설명하기 위해 존재하는 Tag 를 묶어주는 Tag

body : 본문을 묶어주도록 약속된 Tag.

html : html 로 작성된 Tag 에서 가장 최상위로 묶어주는 Tag.

!doctype : 사용자간 약속으로 이 문서의 type 을 알려주는 역할을 한다.


## 참고
[생활코딩](https://opentutorials.org/course/3084/18409)
