
# 인터넷의 시작

1969년 미국 국방부의 주도하에 만들어진 ARPAnet(Advanced Research Projects Agency)이 등장하며 인터넷의 시작을 알렸습니다.  
이후로 ARPAnet 이 민간에 공개되었고, TCP/IP 가 등장하며 일반인들이 인터넷을 사용할 수 있게 되었습니다.  
이제는 인터넷의 규모는 너무나도 커져 현대인들 중에 인터넷을 사용해보지 않은 사람을 찾기가 힘들게 되었는데요,  
이러한 인터넷을 공부한다는건 단순히 웹을 공부하는 것이 아닌 TCP/IP 기반의 전 세계적인 컴퓨터 네트워크를 이해하는 과정이라 생각해야 할 것입니다.

# 인터넷의 동작

## 개념 정리하기

### IP Address

컴퓨터가 네트워크상에서 서로 통신하기 위해서는 고유한 식별 주소가 필요합니다.  
이러한 식별 주소로 IP 를 사용하는데 이를 통해 컴퓨터들은 서로 통신할 수 있습니다.  
IP 는 ISP 를 통하여 할당 받을 수도 있고 LAN 환경이라면 직접 할당하거나 DHCP 를 통해 할당 받을 수도 있습니다.

### Domain Name

IP 주소는 숫자로 이루어져 있어서 사람이 사용하기에는 불편합니다.  
그래서 IP 주소에 일종에 별명을 붙여서 사용할 수 있는데 이를 Domain Name 이라고 합니다.  
좋은 예로는 `www.google.com` 이 있습니다.

### DNS

Domain Name 은 실제 IP 주소를 가리키지는 않고 있습니다.  
때문에 Domain Name 을 Domain Name System (DNS) 을 통해 IP 주소로 번역하여 사용해야 합니다.

### Packet

이제 컴퓨터의 주소를 알 수 있으니 data 를 전송할 수 있습니다.  
이러한 data 는 packet 이라는 단위로 나누어져 전송됩니다.

### Protocol

packet 을 아무렇게나 전송한다면 수신하는 측에서는 어떤 의미인지 알 수 없습니다.  
때문에 서로 어떤 규칙으로 packet 을 주고 받을지 정해야 하는데 이를 Protocol 이라고 합니다.  
TCP, UDP, HTTP, FTP 같은 것들이 대표적인 Protocol 입니다.  

## 인터넷 동작의 간단한 예시

위에서 Internet 에 관련된 간단한 개념을 정립했습니다.  
이제 이 개념들을 토대로 인터넷이 어떻게 동작하는지 예시를 통해 알아보겠습니다.  

1. 사용자가 브라우저를 통해 `www.google.com` 을 입력합니다.
2. 브라우저는 DNS 를 통해 `www.google.com` 의 IP 주소를 알아냅니다.
3. 브라우저는 알게된 IP 주소를 통해 해당 서버에 HTTP 요청 packet 을 보냅니다.
4. 서버는 HTTP 요청 packet 을 받고 HTTP 응답 packet 을 보냅니다.
5. 브라우저는 HTTP 응답을 받고 화면에 표시합니다.

# 참고 자료

- <http://web.stanford.edu/class/msande91si/www-spr04/readings/week1/InternetWhitepaper.htm>{: target="\_blank"}