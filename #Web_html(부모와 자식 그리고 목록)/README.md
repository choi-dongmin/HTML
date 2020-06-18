# Web_html(부모 자식과 목록)

```
<parent>
	<child></child>
</parent>
```

위 코드를 보면 parent, child 2개의 Tag 가 있다, 위의 경우 parent 가 child 를 포함하고 있는 형태이다.

이렇듯 포함을 시키고 있는 Tag 가 부모 Tag , 그리고 포함 된 Tag 가 자식 Tag 이다.

모든 부모,자식 Tag 가 그런것은 아니지만 어떠한 부모 Tag 가 있을때 항상 같이 있는 자식 Tag, 또 반대로 어떠한 자식 Tag 가 있을때 항상 있는 부모 Tag 가 있다.

## 목록
```
파일명 : 목록 1.html
HTML
CSS
JavaScript

<h1>Web_html</h1>

<p>Hello World , This is just practice for my Web_html.</p>
<img src="1.jpg" width="100%">
<p>This is practice <strong> <u>Not Real </u> </strong>  And you can't see this page.</p>

```   

위의 코드가 있다고 할때 어떻게 출력이 될까? 아마도 그냥 HTML CSS JavaScript 그 다음 본문이 밑에 나올것이다.

HTML CSS JavaScript 를 우리는 목록으로 만들고 싶다, 그럼 우리가 지금 활용 할 수 있는 것들을 우선 적용해 보자. 

```
파일명 : 목록 2.html
1. HTML<br>
2. CSS<br>
3. JavaScript<br>

<h1>Web_html</h1>

<p>Hello World , This is just practice for my Web_html.</p>
<img src="1.jpg" width="100%">
<p>This is practice <strong> <u>Not Real </u> </strong>  And you can't see this page.</p>

```   
위와 같은 식으로 목록을 만들고 싶은 내용을 줄바꿈과 번호를 통해 우리가 지금 할 수 있는 것들을 적용시켜 주었다.

그러나 이 Web 개발자들은 보다 편리하게 목록을 만들수 있도록 Tag를 만들었는데 그것이 바로 "<li></li>" 이다.

이 "<li>" 는 list 의 약자로 영어로 목록을 뜻한다.

```
파일명 : 목록 3.html

<li> 1. HTML</li>
<li> 2. CSS</li>
<li> 3. JavaScript</li>

<h1>Web_html</h1>

<p>Hello World , This is just practice for my Web_html.</p>
<img src="1.jpg" width="100%">
<p>This is practice <strong> <u>Not Real </u> </strong>  And you can't see this page.</p>
```

위와 같은 방식으로 만들어 주면 "<br>" 을 하지 않아도 각각의 항목이 줄이 바뀌고 앞에 * 가 붙음으로 좀 더 목록 다운 모습을 같게 된다

그런데 만약 이러한 목록이 여러개라면 우리는 관련 된 것들끼리 묶어주는것이 좀 더 보기가 편할것이다.

그럴때 우리는 문단을 나눌때 사용한 "<p>" 처럼 각각 목록마다 묶어주고 줄을 띄워주는 "<ul>" 을 사용 할 수 있다.
	
```
파일명 : 목록 4.html
<ul>
	<li> 1. HTML</li>
	<li> 2. CSS</li>
	<li> 3. JavaScript</li>
</ul>
<ul>
	<li> 1. Java </li>
	<li> 2. Python </li>
	<li> 3. MySQL </li>
</ul>

<h1>Web_html</h1>

<p>Hello World , This is just practice for my Web_html.</p>
<img src="1.jpg" width="100%">
<p>This is practice <strong> <u>Not Real </u> </strong>  And you can't see this page.</p>
```

하지만 만약 상상을 한번 해보자 우리가 만약 수정 혹은 삭제를 하게 되어 앞의 숫자를 하나씩 앞으로 당겨 와야 한다면

그리고 그것이 만약 수천, 수만개의 숫자라면?? 굉장히 번거러운 일이 될것임이 분명하다.

그래서 Web 개발자들은 목록에 숫자를 정렬 해줄수 있는 Tag 를 만들었다.

"<li>" 의 부모 Tag "<ol>" 이다.

```
파일명 : 목록 5.html
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
위 처럼 "<li>"의 부모 Tag 를 "<ol>" 로 바꾸어주고 숫자를 지워 주었다, 결과값을 확인해보면 앞에 숫자가 저절로 입력되고 이것은 숫자가 있는 목록을 수정을 하는데 아주 큰 역할을 한다.


## 키워드

부모 Tag : 어떠한 Tag 를 감싸고 있는 형태의 Tag

자식 Tag : 부모 Tag 에 포함 되어져있는 형태의 Tag

"<p></p>" : 문단을 지정해주는 Tag

"<li></li>" : 영어의 list 의 약자로 목록을 만들때 이용하는 Tag

"<ul></ul>" : Unordered list 의 약자로 큰 목록과 목록을 구분지어주는 Tag, <li> 의 부모 Tag 이다

"<ol></ol>" : Ordered list 의 약자로 <ul> 과 같이 목록을 구분해주고 목록에 숫자도 입력하고 자동으로 정렬해주는 Tag

"<br>" : 줄을 한칸 바꾸어주는 Tag
 
## 참고
[생활코딩](https://opentutorials.org/course/3084/18408)
