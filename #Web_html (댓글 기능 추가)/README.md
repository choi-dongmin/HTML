# Web_html(댓글 기능 추가)

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

지금까지 우리가 만든 Website 는 우리가 일방적으로 제작자가 방문자에게 정보를 전달하고 있다, 그렇다면 방문자가 사용자에게 피드백 혹은 다른 정보 전달을 할 순 없을까?

그때 가장 간단하게 정보 전달을 받을 수 있는 기능이 바로 댓글 기능이다.

하지만 이 댓글 기능은 html 에서는 불가능하고 , 댓글 기능은 다른 언어 php, python 등에서 만들어서 연계시켜야 하는데 그 과정이 복잡하다.

하지만 우리는 조금 더 똑똑하게 Website 를 만들수 있다, 다른 사람들이 만들어 놓은 Website 의 댓글기능을 우리의 Website 에 적용시켜 보는것이다.

우리가 오늘 도움을 받을 사이트는 바로 disqus 이다. 앞서 말한것과 같이 댓글기능은 복잡한 기능이기 떄문에 disqus 댓글기능을 만들어서 도움을 주고 있다.

* [disqus 댓글 시스템 적용법](https://blog.naver.com/yunjookim97/221926564625) 

위와 같은 방법으로 disqus 에서 제공하는 code 를 복사해 우리의 Website 에 붙여넣는다면 댓글기능을 활용 할 수 있게된다.

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

	<p>
	<div id="disqus_thread"></div>
	<script>

	/**
	*  RECOMMENDED CONFIGURATION VARIABLES: EDIT AND UNCOMMENT THE SECTION BELOW TO INSERT DYNAMIC VALUES FROM YOUR PLATFORM OR CMS.
	*  LEARN WHY DEFINING THESE VARIABLES IS IMPORTANT: https://disqus.com/admin/universalcode/#configuration-variables*/
	/*
	var disqus_config = function () {
	this.page.url = PAGE_URL;  // Replace PAGE_URL with your page's canonical URL variable
	this.page.identifier = PAGE_IDENTIFIER; // Replace PAGE_IDENTIFIER with your page's unique identifier variable
	};
	*/
	(function() { // DON'T EDIT BELOW THIS LINE
	var d = document, s = d.createElement('script');
	s.src = 'https://wabstie-1.disqus.com/embed.js';
	s.setAttribute('data-timestamp', +new Date());
	(d.head || d.body).appendChild(s);
	})();
	</script>
	<noscript>Please enable JavaScript to view the <a href="https://disqus.com/?ref_noscript">comments powered by Disqus.</a></noscript>

	</p>

	</body>
</html>
```   
* 만약 오류가 발생한다면 그것은 아마도 Website 가 file 의 형태로 나타나 있기 때문일 것이다, 그럴때는 server 를 이용해서 실행한다면 문제없이 작동된다.

## 키워드

댓글 : 사용자의 피드백 혹은 정보를 전달 받을수 있는 가장 단순한 형태의 기능

## 참고

https://blog.naver.com/yunjookim97/221926564625

