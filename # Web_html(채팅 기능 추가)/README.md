# Web_html (채팅 기능 추가)

오늘은 방문자와 더 적극적으로 피드백을 할 수 있도록 채팅을 할 수 있는 시스템을 적용해 볼 것이다. 

우리도 여러 웹사이트에서 이러한 시스템을 접해 보았다 예로 상담원과 QnA 와 같은 기능이 바로 이러한 채팅기능이다.

하지만 이 기능또한 댓글 기능과 마찬가지로 굉장히 복잡하고 높은 수준은 기술을 요한다.

그렇기 떄문에 우리는 조금더 현명한 방법으로 전과같이 누군가 만들어 놓은 코드를 복사해서 넣음으로 그 수고를 덜어낼수 있다.

우리는 이번엔 Tawk 이라는 곳을 이용해 채팅기능을 가져와 보자

https://www.tawk.to/ 

위의 주소에서 가입을 하고 적용하고자 하는 주소에 적용을 시킨면 소스를 알 수 있을것이다.

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

우리는 우리가 이전에 만들었던 위 index.html 파일에 채팅기능을 추가해보자

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

	<p>
			<!--Start of Tawk.to Script-->
		<script type="text/javascript">
		var Tawk_API=Tawk_API||{}, Tawk_LoadStart=new Date();
		(function(){
		var s1=document.createElement("script"),s0=document.getElementsByTagName("script")[0];
		s1.async=true;
		s1.src='https://embed.tawk.to/57a72994c11fe69b0bd8fa90/default';
		s1.charset='UTF-8';
		s1.setAttribute('crossorigin','*');
		s0.parentNode.insertBefore(s1,s0);
		})();
		</script>
		<!--End of Tawk.to Script-->
	</p>
	</body>
</html>
```

이러한 방식으로 tawk 의 코드를 적용시켜 채팅을 할 수 있도록 적용 할 수 있다.

* 하지만 이 방법또한 file 형태의 주소가 아닌 Server 를 이용하여야 적용이 가능하다.

## 키워드

채팅 : 실시간으로 방문자와 운영자, 상담자간의 소통이 가능하도록 만든 시스템

# 참고
[생활코딩](https://opentutorials.org/course/3084/18597)
