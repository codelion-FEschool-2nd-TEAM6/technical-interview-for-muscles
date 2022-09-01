# MVC 패턴이란?
- MVC란 Model-View-Controller의 약자로 애플리케이션을 세 가지 역할로 구분한 개발 방법론이다.

# mvc를 web에 적용하기
1. 사용자가 웹사이트에 접속 (Users)
2. Controller는 사용자가 요청한 웹페이지를 서비스하기 위해서 모델을 호출 (Manipulates)
3. Model은 데이터베이스나 파일과 같은 데이터 소스를 제어한 후 그 결과를 Return
4. Controller는 Model이 리턴한 결과를 View에 반영 (Updates)
5. 데이터가 반영된 View는 사용자에게 보여짐 (Sees)

# MVC패턴 방식 
1. 모델 1 방식: JSP에서 출력과 로직을 전부 처리한다.
- 장점 : 빠르고 쉽게 개발 가능하다.
- 단점 : JSP파일이 너무 비대해지며 Controller와 View가 혼재하므로 향후 유지보수에 어렵다.
https://blog.kakaocdn.net/dn/w08Lw/btrlbKqhWKO/qUYnM7xziHIQUE28L6WBZ1/img.png

2. 모델 2 방식: JSP에서 출력만 처리한다.
- 장점 : 디자이너와 개발자의 분업이 가능하며 유지보수 및 확장이 쉽다.
- 단점 : 설계가 어려우며 개발 난이도가 높다.
https://blog.kakaocdn.net/dn/bGZKd4/btrleqFoykC/kXkFFucLJdHJ4hNvfcmav0/img.png

# MVC 패턴을 사용해야 하는 이유
- 비즈니스 로직과 UI로직을 분리하여 유지보수를 독립적으로 수행가능하다.
- Model과 View가 다른 컴포넌트들에 종속되지 않아 애플리케이션의 확장성, 유연성에 유리하다.
- 중복 코딩의 문제점 제거한다.

# MVC 패턴의 한계
- MVC패턴에서 View는 Controller에 연결되어 화면을 구성하는 단위 요소이므로 다수의 View를 가질 수 있습니다. 그리고 Model은 Controller를 통해서 View와 연결되지만, Controller에 의해서 하나의 View에 연결될 수 있는 Model도 여러 개가 될 수 있어 View와 Model이 서로 의존성을 띄게 된다. 
- - 즉, Controller에 다수의 Model과 View가 복잡하게 연결되어 있는 상황이 발생할 수 도 있습니다.

# MVC 패턴 요약

- Model - 백그라운드에서 동작하는 비즈니스 로직(데이터) 처리한다

- View - 정보를 화면으로 보여주는 역할이다.

- Controller - 사용자의 입력 처리와 흐름 제어 담당. 화면과 Model과 View를 연결시켜주는 역할이다.