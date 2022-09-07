# CI/CD

소프트웨어 개발 워크플로우와 좀 더 퀄리티 있는 코드 배포를 자동화한다.
지속적이고 반복적인 프로세스를 사용하면 빌드, 테스트 및 배포 시의 버그와 코드 오류를 방지하는 데 도움을 얻을 수 있다.

> ## CI (Continuous Integration)

<b>CI, 지속적 통합</b>은 모든 코드를 메인 브랜치에 조기(early)에 그리고 자주 통합하고 코드를 커밋하거나 머지할 때마다 각 change 변화를 자동으로 테스트하고 빌드하는 방법론이다.

CI를 사용하면 에러나 보안 문제를 더욱 쉽게 식별하고 고칠 수 있고, 소프트웨어 개발 수명 주기에서 훨씬 일찍 이러한 일들을 수행할 수 있다.

변경 사항을 자주 머지하고 자동 테스트 및 validation 과정을 trigger 함으로써 다수의 개발자가 같은 어플리케이션에서 작업하더라도 코드 컨플릭 가능성을 최소화할 수 있다.

CI가 도입되기 전에는 개발을 마치고 배포가 완료된 후에야 코드 오류를 살피고, 올바르게 동작하는지를 검증하며 코드 품질을 관리했다.
개발자가 개발을 마치고 직접 코드를 머지하고 테스트, 빌드를 검증하는 것을 자동화하여 배포 전에 변경된 코드를 머지하면 자동으로 테스트와 빌드 과정을 거쳐 발생하는 오류를 사전에 처리할 수 있게 되었다.

CI의 장점으로는 주기적으로 머지를 하기 때문에 개발 생산성을 향상할 수 있고, 버그를 빠르게 찾아 해결하고, 소프트웨어의 품질을 개선하고 새로운 업데이트의 검증 및 배포 시간을 단축하는 것이 있다.


> ## CD (Continuous Delivery or Continuous Deployment)

<br />

<p style='text-align:center'><img src='https://user-images.githubusercontent.com/92916958/188765421-8c57ba21-5275-4173-8e1c-342f40957573.png' width='500px'></p>

1.  ### <b>CD, 지속적 서비스 제공(Continuous Delivery)</b>
CI와 함께 사용하는 CD는 인프라 프로비저닝(provisioning, 공급) 및 어플 배포 과정을 자동화하는 소프트웨어 개발 방법론이다.

CI 과정에서 코드가 테스트 완료되면 최종 단계에서 CD는 언제 어떤 환경에 배포하든 필요한 모든 것이 패키지로 배포될 수 있도록 한다.

CD를 통해 소프트웨어는 언제든지 프로덕션에 배포될 수 있도록 구축된다.

단, 지속적 서비스 제공의 의미로 쓰는 CD는 코드가 CI 단계에서 머지, 테스팅, 빌드가 완료되면 수동적으로 배포한다.

2.  ### <b>CD, 지속적인 배포(Continuous Deployment))</b>

지속적인 배포의 의미에서 CD는 지속적 서비스 제공의 CD와 같은 역할을 하지만,
코드가 CI 단계에서 머지, 테스팅, 빌드가 완료된 후 자동 배포한다는 점에서 차이가 있다.

> ## CI/CD의 다양한 툴들

- Jenkins
- BuildKite
- GitHub Actions
- Butbucket Pipelines
- GitLab CI/CD
- circleci

> ## 참고 사이트 & 영상

 <a href='https://www.youtube.com/watch?v=0Emq5FypiMM'>드림코딩 엘리 CI/CD 5분 개념 정리(현업에서 쓰는 개발 프로세스)</a>
 <br />
 <a href='https://about.gitlab.com/topics/ci-cd/'>깃랩 공식페이지</a>
 <br />
 <a href='https://tecoble.techcourse.co.kr/post/2021-08-14-ci-cd/'>우테코 블로그</a>
