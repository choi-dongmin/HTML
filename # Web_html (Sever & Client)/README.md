# Web_html (Sever & Client)

우리가 만약 인터넷을 사용한다고 하면 최소 몇대의 컴퓨터가 필요할까? 정답은 최소한 2대의 컴퓨터가 필요로 한다.

최소한 2대가 있어야지 컴퓨터에서 정보를 주고 받을수 있다, 이때 1대의 컴퓨터는 정보를 요구하고 1대의 컴퓨터는 정보를 제공한다

이때 정보를 요구하는 컴퓨터늘 client, 정보를 제공하는 컴퓨터를 Server 라고 일컫는다.  

우리는 평소에 Web browser 즉 Web client 는 일상 생활에서 많이 접하고 사용할 수 있다

예를 들면 게임같은 경우에 우리가 실행을 하면 client 가 되어 internet 을 이용해 게임회사의 Web Server 에 정보를 요청한다.

이렇듯 평소에 우리가 Web browser 를 사용하면서 우리도 모르게 client 를 사용하고 있던 것이다.

그렇다면 우리는 Web browser 가 아닌 우리가 잘 사용하지 않는 영역의 Server 에 대해서 좀 더 알아 보도록 하자.

Web Server 를 아는것은 내가 가진 정보를 internet 을 사용할 수 있는 사람이라면 전세계 어디에서든지 내가 가진 정보를 볼 수 있게 하는것 이다.

이렇게 Sever 를 이용 할 수 있는 방법에는 2 가지가 있다.

하나는 Web server 를 자신에 컴퓨터에 설치하여 하는방법, 또 하나는 Web server 의 일을 대행 해주는 곳에 위탁하는 방법이 있다.

## Web hosting 

우리가 Web server 를 운영하고 관리하는 일은 절대 쉽지 않은 일이다 단편적으로 컴퓨터가 있어야 하며 Server 컴퓨터는 항상 켜저있어야 한다.

그 외에 Server 설치, Client 접근성 등 신경써야 할 문제가 적지 않다 그렇기 때문에 이러한 일을 대신해주는 많은 기업들이 있다.

한마디로 Server 를 원하는 사용자에게 host 를 빌려주는것을 우리는 Web hosting 이라고 일컫는다.

### GitHub Pages 

이러한 Web hosting 을 하는 기업중에는 무료로 해주는곳이 있다. GitHub 이 대표적인 기업인데 우리가 이곳에 Repositoies 에 html 파일을 저장을 한 후에

Setting 에서 Github Pages 라는 곳에서 Source 에 none 이라고 설정 되어 있는것을 Master Branch 로 바꾸고 저장을 하면 주소가 생긴다.

그러면 GitHub 으로 부터 Web hosting 을 받고 있으며 그 주소는 저장한 Html 파일의, 즉 우리의 고유한 주소가 되는것이다 물론 다른 인터넷 사용자 또한 그 주소를 통해 저장된 Html 을 볼 수 있다.

다시 한번 구조를 설명하면 우리의 컴퓨터에는 우리가 만든 index.html 파일이 존재하지만 Server 가 존재 하지 않아 다른 사람이 개발자의 컴퓨터에 접근이 안됨으로

우리는 Web hosting 을 받아 Web Server 에 index.html 을 저장해 Github 으로부터 주소를 받고 우리가 방문자에게 주소를 알려준다면 저장된 index.html 에 접근 할 수있게 된다.

## Web server  

이번에는 Web hosting 과 반대로 나의 컴퓨터에 server 를 설치해서 누구나 나의 Web page 에 접속 할 수 있도록 하는것을 'Web server' 라고 일컫는다.



## 키워드

Server : 인터넷을 통해와 정보를 저장하고 송출해주는 역할을 하는 컴퓨터, 프로그램. 

Client : 인터넷을 통해 원하는 정보를 받는 컴퓨터 , 우리가 인터넷을 이용할 떄 주로 사용하는 기능들이 있다.

Host : Server 역할을 하는 컴퓨터들을 한대 한대 Host 라 일컫는다.   

Web hosting : Server 를 원하는 사용자에게 host 를 빌려주는것을 일컫는 말. 

Web sever : 나의 컴퓨터에 server 를 설치해서 누구나 나의 Web page 에 접속 할 수 있도록 하는것을 'Web server' 라고 일컫는다.

## 참고
[생활코딩](https://opentutorials.org/course/3084/18891)