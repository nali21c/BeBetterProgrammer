##### 13.2.4 설계 관련 결정 연기하기

YAGNI('dont do anything if You Arent Going to Need It')
초기에 중요하고 필요한 부분만 처리하고, 나머지는 미뤄라. 결정을 미루는 것은 설계에 대한 대단히 강력한 접근이며 자유로운 것이다.

- 발생할 수 있는 가장 나쁜 상황 중 하나는 아직 모르는 것을 설계하는 경우다. YAGNI 원칙에 따르면 문제가 정확히 무엇이고 이를 설계에 어떻게 반영해야 하는지 알 때까지 결정을 미뤄야 한다.
- 이런 현상 추후 설계 작업의 낭비, 유지보수의 짐이 될 수 있다.

##### 13.2.5 품질 유지

- 페어 프로그래밍
- 페어 프로그래밍을 거치지 않은 모든 코드나 설계에 대한 리뷰
- 모든 코드에 대한 유닛 테스트

개발자들은 설계를 믿었고 반드시 보호해야 할 만큼 소중하다고 여겼다.

- 설계 품질을 반드시 유지해야 한다. 이는 개발자들이 의무감을 가지고 진지하게 대할 때에만 가능하다.

##### 13.2.6 기술 부채 관리

임시 방편 처리를 기술 부채로 표시해두었다가 이후 버전에서 수정하도록 했다. 겉으로 드러난 표시들을 처리하기 전까지 개발자들은 기분이 찜찜할 수밖에 없었다.
-> 개발자들의 설계 품질에 대한 책임감

기술 부채
- 은유적 표현은 소프트웨어를 빠르게 출시하기 위한 결정을 내리는 것은 부채를 지는 것과 같다는 의미를 가지고 있다. 즉 지금 무언가를 할 수 있게 해주는 것으로, 그 것이 없었다면 무언가를 할 수 없었다는 뜻.
부채는 무시해서는 안 되며 반드시 되갚아야 하는 것. 기술 부채란 리펙토링이나 설계 조정의 지연, 다음 업데이트까지 라이브러리나 빌드 도구의 업데이트를 미루는 것,
로깅이나 디버깅을 대충 처리한 부분을 합리화 하는 것. 의식적으로 기술 부채를 다룬다면 개발팀에게는 강력한 무기가 될 수 있다. 부채가 쌓이지 않도록 하되 항상 그것을 가시화하라.
실제 부채처럼 최대한 빨리 갚아서 과도한 이자와 비용이 들지 않도록 하라.