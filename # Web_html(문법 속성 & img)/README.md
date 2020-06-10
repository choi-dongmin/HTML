# html 문법 속성 & img

우리는 text 를 이용해서 지금까지 html 을 작성했다 물론 text 는 정보 전달을 하는데 있어 좋은 도구중 하나이다 

그러나 만약 그 text 와 사진까지 같이 있다면 사용자 입장에서 그 정보를 이해하는 것은 2~3배로 쉬워 질 것이다.

우리는 오늘 사진을 첨부하는 Tag 에 대해서 알아보자.


## img

이미지를 첨부하는 Tag 는 img 이다.

```
파일명 : 1.html

<h1>Web_html</h1>

<p>Hello World , This is just practice for my Web_html.</p>

<img>

<p>This is practice <strong> <u>Not Real </u> </strong>  And you can't see this page.</p>

```
그럼 위와 같이 작성을 한다면 page 에서 이미지가 출력이 될까? 그렇지 않다 이 경우 단순히 Tag 만으로 이미지를 출력 할 수없다.

그럼 어떻게 해야할까? 우리는 그떄 source 를 지정해주어 이미지를 출력 할 수있다.


```

파일명 : 1.html

<h1>Web_html</h1>

<p>Hello World , This is just practice for my Web_html.</p>

<img src = "1.jpg" width="100%">

<p>This is practice <strong> <u>Not Real </u> </strong>  And you can't see this page.</p>


* unsplash : 저작권에 구애받지 않고 이미지를 다운 할 수 있는 페이지

```

이렇게 같은 폴더에 1.jpg 라는 것을 불러와 출력한다 하지만 출력 해본다면 사진이 너무 크거나 혹은 너무 작을것이다.

그럴때 width="100%" 이것처럼 width 를 이용하면 페이지의 크기에 맞게 사진을 조정한다.


## 문법의 속성

우리는 이 img 를 통해 Web_html 의 문법적 속성(Attribute)을 알 수 있다.

바로 src = "1.jpg" width="100%" 이것 들이 속성이다 그리고 이 속성의 위치는 변동이 가능하다 

예를 들어 <img width="100%" src = "1.jpg" > 이런 식으로 가능하다.

한마디로 Tag 가 단순히 Tag가 가진 정보가 부족하다면 바로 이 속성을 이용해서 정보를 채워줌으로 Tag를 완성 시킬수 있다.

## html 이 중요한 이유

html 은 Tag 로 이루어져 있고 검색엔진은 그 Tag 를 이용하여 검색결과를 보여준다, 그렇기 때문에 정확한 Tag로 web 을 작성시 훨씬 정보를 빠르고 정확하게 받을 수 있다.

이것은 단순해 보이지만 가장 단순해 보이는것이 가장 중요하듯이 이 기능은 정말로 중요하다

또 하나는 바로 접근성이다 Web 은 어느 운영체제, 누구나 접근 할 수있고 저작권이 없다. 


## 키워드

img : 이미지를 web 에 출력 하도록 하는 Tag src 로 경로를 지정 해주어야 한다.

src : source 의 약자로 Web 에선 경로를 지정 해주는 속성이다.

width : 이미지의 크기를 조절하는 속성이다. 

속성(Attribute) : 단순히 Tag 가 자신이 가진 정보만으로 결과를 출력하지 못 할때 속성을 추가함으로 Tag 를 완성 시킬수 있다.


## 참고

[생활코딩](https://opentutorials.org/course/3084/18407) 