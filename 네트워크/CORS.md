# CORS
: Cross Origin Resource Sharing의 준말로, 한 사이트에서 다른 사이트 서버로 api와 같은 요청을 보낼 때 자주 접할 수 있는 에러이다.


브라우저에 저장된 정보를 가지고 타 사이트에서 악의적인 행위를 하는 것을 방지하기 위해 **SOP(Same Origin Policy)** 라는 동일한 출처끼리만 api 등의 데이터 접근이 가능하도록 막는 정책이 디폴트로 설정되어 있어, <br>다른 사이트의 리소스를 가져오려면 CORS를, 즉 다른 출처간 리소스 공유를 허용하라는 에러가 뜨는 것이다.

CORS를 허용하기 위해선 요청을 받는 백엔드단에서 CORS를 허락할 다른 출처들을 미리 명시하면 된다. <br>
가장 쉬운 방법은 Express 등의 프레임워크를 쓰는 것인데, 왜냐하면 cors라는 서드 파트 미들웨어를 지원해주기 때문이다. <br>
프레임워크에서 CORS 응답 헤더를 추가해 주기 때문에 개발자가 별도의 CORS 응답 헤더를 추가해 주지 않아도 된다. 

그 외 CORS 에러를 해결할 응답 헤더를 적는 방법은 다음과 같다.
1. Access-Control-Allow-Origin 헤더에 적는 방법
브라우저는 다른 출처에게 요청을 보낼 때 요청에 origin이라는 header를 추가한다. 이 header에는 요청하는 쪽의 scheme, 도메인, port 가 담기는데, <br>
이 요청을 받은 서버는 답장 header에 지정된 Access-Control-Allow-Origin 정보를 실어서 보낸다.<br>
그래서 브라우저가 요청에 origin값이 Access-Control-Allow-Origin 값과 동일한 경우 안전한 요청으로 간주하고 응답 데이터를 받아온다.

2. Access-Control-Request-Method를 추가해주는 방법
 Access-Control-Allow-Methods 헤더에 GET, PUT, POST, DELETE 등의 HTTP 메서드를 ,로 구분하여 넘겨준다.
 
3. 응답 헤더에 Access-Control-Expose-Headers를 추가해주는 방법
4. Access-Control-Allow-Headers 를 추가해주는 방법
5. 그외) 프론트엔드와 백엔드 사이에 프록시 서버를 두는 방법으로 CORS를 해결할 수도 있다. 개발 환경에서 CORS를 해결해야 한다면, Webpack Dev Server 등의 라이브러리를 사용해서 프록시 설정을 하는 방법도 있다.

CORS에서는 simple request와 preflighted 요청이 있는데,
전자는 요청을 보내는 것은 허용하되, 통과를 못하면 서버 응답을 못받아오는거고
후자는 요청에 의해 서버데이터가 변경될 수 있기 때문에 요청을 보내는 것도 허락을 받도록 하는 것이다.


##### [참고링크]
- https://www.youtube.com/watch?v=bW31xiNB8Nc&t=249s
- https://beomy.github.io/tech/browser/cors/
- https://developer.mozilla.org/ko/docs/Web/HTTP/CORS
- 참고링크를 모두 보시는 것을 추천합니다 :)
