##### 13.1.4 코드 문제

나쁜 설계로 읺나 문제는 코드에까지 영향을 미친다.
방만하고 명확하지 않은 구조는 각각의 컴포넌트가 잘못 작성되고 서로 들어맞지 않는 결과를 낳는다. 코드 복제와 반복된 작업 또한 가져온다.

##### 13.1.5 코드 외부 문제

개발팀 
- 직원이 쉽게 이직해버리는 이유는 있다.

느린 개발 주기
- 유지 보수의 일은 소름 끼치는 작업이었다.

지원 엔지니어
- 제품을 지원하려 애쓰며 힘든 시간을 보냈다.

서드파티 지원
- 많은 버그가 발생, 이해하기도 힘들었다.

회사 내부 정치

나쁜 구조로 인한 문제는 코드 내부에 한정되지 않는다. 외부와도 연계되어 개개인과 팀, 업무 처리 과정, 일정 산정 모두에 악영향을 미친다.

##### 13.1.6 대도시로부터의 엽서

재작업하고 리팩토링하며 구조적 문제를 바로잡는 데는 엄청난 비용이 필요했다. 임시로 땡빵질만 했다.
결국 회사 재정에도 심각한 문제를 일으키고 말았다.

- 낮음 품질의 비주기적인 제품 업데이트
- 어려워진 신규 기능 추가 및 변경
- 시스템 전반적으로 낮은 코드 수준
- 스트레스, 사기, 이직 등 사람의 문제
- 지저분한 정치적 문제
- 회사에 필요한 성공의 부재
- 엄청난 고뇌와 야근

##### 13.2 디자인 타운

초기 설계 방향을 크게 가져가기보다는 작동하기에 알맞은 수준으로 결정했다. 주요 기능 영역을 분리, 스레딩 모델과 같은 핵심적 설계 방향을 고안. 
가장 중요한 기능 영역에 대해서만 초기 설계 단계부터 집중하였다.

기본적인 유지 보수를 위한 부분에 있어서도 코드를 작성하기 쉽고 응집되도록 하는 방향으로 빠르게 결정했다.
예를 들어, 최상위 수준의 디렉토리 구조, 명명 규칙, 일반적 코딩 관례에 덧붙인 코드 작성 방법, 유닛 테스트 프레임워크 선택과 기반 구조가 되는 내부 구조등등.

설계와 코드 작성은 모두 페어 프로그래밍 방식으로 이루어졌고, 세밀하게 코드리뷰가 진행되었다.

##### 13.2.1 기능 위치 선정

코드가 어디에 있는지에 대한 질문은 필요하지 않았다. 
구조적 설계 계획으로 인해 개발자들은 더 열심히 일해야 했지만, 유지 보수의 어려움이 없었기에 이후의 삶은 더 나아졌다.

##### 13.2.2 일관성

시스템 전반에 걸쳐 일관성이 있었다. 모든 수준에서의 모든 결정을 전체 설계의 관점에서 수행했다.
작성된 모든 코드는 설계와 어울렸으며, 이미 작성된 코드와도 잘 어울렸다.

명확한 구조 설계를 통해 일관된 시스템을 구성할 수 있다. 모든 설계 결정은 전체 구조 설계의 관점에서 수행해야 한다.

명확하게 정의된 소프트웨어 설계에 힘입어 코드 복제는 일어나지 않았고, 비슷한 디자인 패턴이 일관되게 적용되었다.

##### 13.2.3 구조 확장

저장소 관리나 외부 제어 기능과 같은 완전히 새로운 몇몇 기능 영역을 '큰그림' 설계에 추가하게 되었다.
대도시 프로젝트와는 달리, 디자인 타운에서는 완전히 다른 이야기였다.

시스템 설계도 코드와 마찬가지로 적응성 있고 리팩토링 가능하도록 수행했다. 어떤 것도 변하지 않는 것은 없다. 필요한 경우 변경해야 할수도 있다.
결과적으로 코드는 빠르게 규모를 키워나가면서 적절한 내부 구조를 유지했다. 

간결성을 빼았는 변화에 저항하라.