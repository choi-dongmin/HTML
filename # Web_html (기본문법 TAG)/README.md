# Web_html (기본문법 TAG)


## html 을 이용해서 web 에 내가 원하는 정보를 출력해보자.

우리가 만약 Hello World 라는 것을 출력하고 싶다면 어떻게 할 수 있을까? 가장 간단한 방법으로 메모장, 텍스트 편집기 등 을 이용 할 수 있다.

그곳에서 우리는 Hello World 라는 것을 입력하고 저장을 하면서 파일의 확장자를 html 로 지정 할 것이다.

Windows : control + o  

Mac OS : commend + o 

저장경로를 통해서 우리가 방금 만든 html 파일을 실행 시킨다면 web 을 통해서 Hello World 가 실행 될 것이다.

우리는 그 파일에 원하는 입력값을 입력함으로써 원하는 출력값을 가질수 있다.

그럼 우리의 Web 에 출력하려 하는 목적을 달성한 것이다 그러나 만약 Hello 라는 입력값이 중요해서 그 텍스트를 더 진하게 표시하고 싶으면 어떻게 할까?

```
파일명 : 1.html


Hello World 

``` 

위 코드가 바로 우리가 만든 Hello World 를 출력해 주는 1.html 파일이다 .

자 그럼 저 코드에서 우리가 Hello 에 더 힘을 주고 싶다면 어떻게 해야할까??

```
파일명 : 2.html


<strong> Hello </strong> World

``` 

이런식으로 입력해주고 다시 웹 파일을 실행시키면 Hello 라는 값이 World 보다 더 진하게 강조된 표현 될 수 있는걸 볼 수 있다.

우리는 더 나아가서 만약 그곳에 밑줄을 만들고 싶다면 어떻게 해야할까?

```
파일명 : 3.html


<strong><u> Hello </u></strong>World 

``` 

밑줄은 영어로 Underline 이다 그럼 <u> </u> 를 통해서 밑줄을 만들어 줄 수 있다.

## TAG

우리는 여기서 TAG 라는 것을 배웠고 또한 사용도 해보았다 그러면 TAG 란 것은 무엇일까?

<strong> </strong>, <u> </u> ...

이러한 것들이 TAG 이다.

그렇다면 TAG는 무엇일까? 만약 우리가 새로운 옷을 샀다고 한다면 그곳에는 분명해 TAG 가 있을 것이다 그것은 그 옷 또는 상품을 설명하기 위함이라고 할 수 있다.

그렇다면 Web 에서 Tag 가 하는 역할도 바로 설명을 하기 위함이다 <strong> </strong> 는 Strong 강하게, 즉 진하게 표시하는것을 설명하는것이다.

TAG 에는 열린 Tag , 닫힌 Tag 가 있다 

```
<strong> Hello </strong>World

<strong> : 열린 Tag

</strong> : 닫힌 Tag 
```

말 그대로 시작과 끝에 넣어주는 Tag 인데 닫히는 Tag 에는 / 를 넣어서 닫힌 Tag 가 어떤것인지 알게 해준다.

## 키워드

html : web 문서를 만들기 위한 기본적인 확장자, 웹 언어

strong : 강조하고 싶은 text 를 진하게 표현 해주는 TAG

u : 강조하고 싶은 text 밑에 밑줄을 표현 해주는 TAG


## 참고 
[생활코딩](https://opentutorials.org/course/3084/18392)
