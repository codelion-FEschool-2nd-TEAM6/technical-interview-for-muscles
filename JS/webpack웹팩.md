# 웹팩 Webpack

<img src="https://user-images.githubusercontent.com/92916958/190322287-95b40654-6060-4450-861e-22db446a4dda.png">

> ## Webpack

- webpack은 모던 자바스크립트 애플리케이션을 위한 <i>정적 모듈 번들러</i>이다.
- webpack이 애플리케이션을 처리할 때, 내부적으로는 프로젝트에 필요한 모든 모듈을 매핑하고 하나 이상의 번들을 생성하는 디펜던시 그래프를 만든다.
  <br />
  > 💡 모듈 번들러 Module Bundler
  - 웹 애플리케이션을 구성하는 자원(HTML, CSS, JavaScript, Images 등)을 모두 각각의 모듈로 보고 이를 조합해서 병합된 하나의 결과물을 만드는 도구를 의미한다.

> ## Webpack에서의 모듈

- 자바스크립트 모듈에만 국한되지 않고 웹 애플리케이션을 구성하는 모든 자원을 의미한다. 웹 애플리케이션을 제작하기 위해 필요한 HTML, CSS, JavaScript, Images, Font 등 많은 파일들 하나하나가 모두 모듈이다.

> ## 모듈 번들링

- 웹 애플리케이션을 구성하는 자원들을 하나의 파일로 병합 및 압축해주는 동작

> ## 웹팩의 4가지 주요 속성

 웹팩의 빌드(파일 변환) 과정을 이해하기 위해서는 4가지 주요 속성에 대해 이해하고 있어야한다.

 <img src='https://user-images.githubusercontent.com/92916958/190337070-e64903f2-b471-4ff3-ac61-634c4881363c.png'>

- entry : 웹팩을 실행할 대상 파일. 진입점
- output : 웹팩의 결과물에 대한 정보를 입력하는 속성. 일반적으로 `filename`과 `path`를 정의.
- loader : CSS, 이미지와 같은 비 자바스크립트 파일을 웹팩이 인식할 수 있게 추가하는 속성. 로더는 오른쪽에서 왼쪽으로 적용.
- plugin : 웹팩으로 변환한 파일에 추가적인 기능을 더하고 싶을 때 사용하는 속성. 웹팩 변환 과정 전반에 대한 제어권을 갖고 있음.

> ## 🗒 참고사이트

- 웹팩의 간단한 개념은 위와 같고, 좀 더 정확히 이해하기 위해 밑의 링크에서 좀 더 자세한 설명을 읽어보시길 추천드립니다!
  (직접 해보지 않으면 글만 읽고 이해하기 어려우실 것 같습니다.)

<a href="https://joshua1988.github.io/webpack-guide/concepts/entry.html#entry">웹팩 핸드북 - Introduction</a>

<a href="https://joshua1988.github.io/webpack-guide/getting-started.html#%EC%9B%B9%ED%8C%A9-%EB%A7%9B%EB%B3%B4%EA%B8%B0-%ED%8A%9C%ED%86%A0%EB%A6%AC%EC%96%BC">웹팩 맛보기 튜토리얼</a>
<br />
-> 튜토리얼 진행 후 밑의 링크를 통해 이어지는
아티클을 읽으며 웹팩 완벽 이해하기✨
(넉넉히 1시간 정도면 충분합니다!)

<a href="https://joshua1988.github.io/webpack-guide/concepts/entry.html#entry">웹팩 핸드북 - Concepts</a>
