# Web_html (Web Server)

그럼 우리가 지금까지 html 을 통해 만든 Web Page 를 컴퓨터의 Web Server 를 설치해 인터넷에 출력해보자.

## bitnami Apache

프리웨어 bitnam 의 mamp의 Apache 를 통해 server 를 설치하고 Page 를 인터넷에 출력해보자.

Mamp 를 설치하고 실행 시키면 Managemaent Servers 라는 항목에 Apache Web Server 라는 항목이 있다

그 항목이 Running 중이라면 이제 그 컴퓨터는 Server 를 할 수 있게 된것이다.

만약 그 Apache 가 종료 된다면 그 컴퓨터는 Web Server 를 할 수 없게 된다.

그런데 이 Apache 로 Server 를 한다면 인터넷 주소창에  

```
http://127.0.0:8080/main.html    
```

와 같은 주소가 있을것이다 여기서 앞쪽의 127.0.0 은 ip add 즉 internet protocol address 이고

8080 은 Port 라는것인데 사실상 Mac 은 서버가 자체적으로 내장 되어 있지만 필자는 butnami 를 통해 Server 를 하나 더 설치 했음으로 

구분하여 어떤 Server 로 접속한 것인지 보여주는 것이다.

그렇다면 Web Browser 가 Web Server 에 접촉하는 진행 방향을 알아보자.

만약 Browser 에서 add 를 인터넷에서 입력한다면 Web Server 에 있는 index.html 파일을 찾고

Web Server 는 bitnami 가 있는 폴더에 htdoc 즉, htper text document 에 index.html 을 찾고 결과를 출력한다.

그전 우리가 만든 html 파일을 우리가 자체 스스로 출력했을때와 다른점은 http:// 바로 이 부분이다.

Hyper Text Transfer Protocal 의 약자로 즉 내가 가진 Web page 를 전송 시킬 수 있다는 규약을 표시하는 것이다.

이전에 우리가 html 파일을 Server 없이 실행 시킨다면 File 이라고 표시 되었을 것이다.

## Web browser 와 Web Server 의 통신

하지만 위와 같은 방법을 거친다고 해도 아직 다른 사람의 컴퓨터에서 우리가 만든 Web Page 를 출력할 수 없다.

지금까지의 우리가 배운것을 쉽게 정리하자면 Web browser 는 Web Server 에게 main.html 의 파일을 원하고 Web Server 는 그것을 제공해야 한다.

그런데 가장 중요한것이 그럼 어떻게 불러오는가? 우리는 주소가 필요하다 만약 Web browser 는 어떤  Server Computer 에 접속 하는가 즉, Ip add 가 필요하다.

```
html://192.168.1.13:8080/main.html
```

위와 같은 방식으로 다른 사람의 컴퓨터 즉 다른 인터넷에서 Server 사용자의 ip add 를 가지고 Wab Page 를 볼 수 있다.

## 키워드

HTTP : Hyper Text Transfer Protocal,Web Server 와 사용자 사이에 Web page 를 전송하기 위한 규약

ip add : 각각 고유한 인터넷 번호 , 주소

## 참고
[생활코딩](https://opentutorials.org/course/3084/18894) 
