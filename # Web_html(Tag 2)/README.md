# Web_html (Tag 2)

## Tag 2

우리는 이전까지 'Tag' 가 무엇을 뜻하는지 알지 못했지만 이제는 알 수 있게 되었다. 

```
<h1>Hello</h1>
<h2>Hello</h2>
<h3>Hello</h3>
<h4>Hello</h4>
<h5>Hello</h5>
<h6>Hello</h6>

* 위 Tag 는 제목 지정하고 뒤의 숫자는 글자 크기를 조절한다.
```

무엇을 배우던지 가장 처음 배우는것이 가장 많이 사용하고 가장 실용적이고 그로인해 가장 중요하다 마치 수학을 배움에 있어 사칙연산이 가장 기본이며 중요하듯,  

Tag 는 Web 언어의 기본이자 가장 많이 사용한다.


```
파일명 : 1.html

<h1>Web_html</h1>

<strong><u> Hello World </u></strong>, This is just practice for my Web_html

```

위 방식으로 아래의 본문과 위의 제목을 간단하게 지정 해 줄수 있다.

약 Tag 는 150개 가량이 있다고 하는데 우리는 이 모든것을 다 외우고 알고 있으면 가장 좋겠지만 모든 사람이 그렇게 할 수는 없다

그래서 우리는 가장 사용 빈도가 높고 중요한 것을 알아두는것이 가장 좋다 그리고 우리는 모르는 Tag 가 있으면 그저 검색엔진에 손쉽게 검색함으로 궁금증을 풀 수 있는 시대에 살고 있다.

그렇다면 약 1개의 Web Page 는 평균 몇개의 Tag 로 이루어져 있을까 [참고1](https://www.advancedwebranking.com/html/) 를 보면 약 24~26 사이가 가장 빈번하다

그럼 우리는 지금 몇개의 Tag 를 알고 있는가?

- strong

- u

- h1 ~h6

약 8 개의 Tag를 알고 있다 그리고 그 말은 약 26개 정도를 알고 있으면 하나의 Web Page 의 소스를 보는데 어려움이 없다는 말이다.

그리고 참고1 을 본다면 어떠한 Tag 들이 가장 많이 사용이 되었는지 알 수 있다.

우리는 이러한 Tag 들을 후에 점진적으로 배울 것이다 그리고 오늘 우리는 2개의 Tag를 더 배울것이다.


## 줄바꿈 br vs p

```

<h1>Web_html</h1>

Hello World , This is just practice for my Web_html.

This is practice <strong> <u>Not Real </u> </strong> And you can't see this page
```

우리는 위와 같은 web 을 작성하였고 위 코드처럼 줄을 띄운곳에서 web 도 같이 줄을 바꿔주고 싶다. 

1. br

```
파일명 : 2.html

<h1>Web_html</h1>

Hello World , This is just practice for my Web_html.
<br><br>
This is practice <strong> <u>Not Real </u> </strong> And you can't see this page
```

우리는 br 이라는 Tag 를 사용해 줄을 바꿔주었다(br 한번에 한칸씩 내려간다).

이 br Tag 이 신기한 것은 그전까지 우리는 열린/닫힌 Tag 이 존재 했는데 이 br Tag 은 그저 단 한개의 Tag 으로만 이루어저 있다는 것이다.

그저 줄바꿈으로만 이용하기 때문에 어떠한 단어 혹은 문장을 감싸줄 필요가 없다.


2. p

그런데 단순한 줄 바꿈이 아닌 하나의 문단을 지정해준다면 자연스럽게 줄이 바뀌지 않을까? 개발자들은 한 문단 문단을 지정 할 때 사용할 Tag를 만들었다.

```
파일명 : 2.html

<h1>Web_html</h1>

<p>Hello World , This is just practice for my Web_html.</p>
<p>This is practice <strong> <u>Not Real </u> </strong> And you can't see this page.</p>

``` 

위와 같은 식으로 p 의 열린/닫힌 Tag 를 이용해 하나의 문단으로 지정을 해주어서 줄을 바꿔줄수도 있다.

## 키워드

h1~6 : 자주 사용하는 Tag 로 머릿말을 정하고 숫자를 통해 머릿말의 크기를 정한다.

br : 줄을 한칸 내려주는 기능을 하는 Tag 그렇기에 열린/닫힌 Tag 이 존재하지 않는다.

p : 하나의 문단을 지정해주는 Tag 이다.

## 참고
[생활코딩](https://opentutorials.org/course/3084/18403)




