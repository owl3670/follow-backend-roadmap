# HTTP 의 특징

HTTP 는 TCP/IP 기반의 응용 계층 protocol 로 client 와 server 사이의 통신을 할 수 있게 해준다. HTTP 는 인터넷 안에서 contents 를 어떻게 주고 받을 것인가에 대한 규칙이며 표준이다. HTTP 를 통해 문서, 동영상, 음악, 기타 데이터 등을 주고 받을 수 있게 된다.

# HTTP 의 역사

HTTP (HyperText Transfer Protocol) 은 CERN 에서 연구하던 Tim Berners-Lee와 그의 팀이 정보를 주고 받기 위해 만든 protocol 이다. 1989년에 World Wide Web (WWW) 가 제안 되면서 정보를 교환하기 위한 방법을 고안하기 시작하였고, 1991 년의 HTTP V0.9 버전으로 최초로 문서화 되었다. 이후 1996년에 상용화 버전인 HTTP/1.0 이 발표되었고, 1999년 HTTP/1.1, 2015년 HTTP/2 등의 발표가 이루어 졌고 2022년 HTTP/3 가 표준화 되었다.

# HTTP Message

HTTP 의 Message는 Request Message 와 Response Message 가 있다.

## Request

- Start line
    - Method : client 가 원하는 형태의 요청이 무엇인지 나타냅니다. GET, POST 와 같은 것들입니다.
    - Path : 가져오기 원하는 Resource 의 URL 을 나타냅니다.
    - Version of the protocol : HTTP Protocol 의 버전을 나타냅니다.
- Headers : 추가 정보를 나타냅니다.
- Body : POST 와 같은 method  등에서 전송하는 data 를 나타냅니다.

## Response

- Status line
    - Version of the protocol : HTTP Protocol 의 버전을 나타냅니다.
    - Status code : 요청에 대한 처리 결과를 나타내는 코드입니다.
    - Status message : status code 에 대한 짧은 설명입니다.
- Headers : 추가 정보를 나타냅니다.
- Body : Resource data 를 나타냅니다.
- 
# 참고 자료

- <https://developer.mozilla.org/en-US/docs/Web/HTTP/Overview>
- <https://developer.mozilla.org/en-US/docs/Web/HTTP/Messages>

---

- [목록으로](../README.md#internet)

