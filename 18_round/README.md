##### 13.2.7 설계 방향을 잡는 테스트

코드는 유닛 테스트를 거쳐야 하고 시스템은 통합 테스트와 인수 테스트를 거쳐야 한다는 것이다.
유닛 테스트를 통해 많은 이득을 볼 수 있었다.
예를 들면, 데이터 파이프라인에서 스레드 모델과 상호 연결을 위한 인터페이스를 근본적으로 변경할 때, 테스트를 해봄으로써, 상호작용을 알 수 있었고 설계를 변경할수 있었다.

훌륭한 자동화 테스트를 시스템에 적용하면 최소한의 위험만으로 근본적인 구조 변경을 수행할 수 있다. 이는 작어베 여유를 보장해준다.

유닛 테스트의 또 다른 커다란 장점은 코드 설계에 있어 훌륭한 윤곽을 그려준다. 유닛 테스트를 작성함으로써, 각 모듈이 내부적으로는 응집도가 높으면서도 시스템의 나머지 부분과는 결합도가 낮도록 만들 수 있다.
유닛 테스트에 따라 각 단위의 인터페이스를 신중하게 설계해야 하고, API는 유의미하면서도 내부적으로 일관되도록 설계해야 한다.

테스트가 가능한 설계를 하라.

##### 13.2.8 설계를 위한 시간

성공에 기여한 요소 중 하나는 적절히 할당된 개발 일정이다. 충분한 시간을 들여야 하지만 너무 많은 시간은 실현될 수 없는 예술작품을 설계할 수도 있다.

##### 13.2.9 설계를 가지고 작업하기

일관성 있고 이해하기 쉬워야 한다. 이해하기 어렵고 불필요하게 복잡한 상호 작동이나 이상한 현태의 러거시 코드는 없어야 한다.
개발자들이 설계에 대한 주인의식을 가지고 일할 수 있었다. 모든 개발자가 시스템의 어디에서나 작업할 수 있었다.

##### 13.3 마치며

구조가 소프트웨어 프로젝트에 얼마나 심대한 영향을 끼치는지 보이는 두 예이다. 이는 모든 것에 영향을 미친다.

- 코드 작성에 앞서 계획적으로 설계하기
- 설계작들의 역량과 경험 : 실수를 미리 경험해두면 이후 적절한 결정을 내릴 수 있다.
- 개발 진행에 맞춰 설계를 명확하게 유지하기
- 소프트웨어의 전체 설계에 대한 책임감을 팀 단위로 모두에게 지우기
- 설계 변경을 두려워 하지 않기 : 변하지 않는 것은 없다
- 적절한 구성원으로 팀 짜기 : 관계는 코드 구조에 영향을 미친다
- 적절한 시점에 설계에 대해 결정하기 : 아직 만들 수 없다면 설계에 대한 결정 미루기
- 적절한 프로젝트 관리와 일정

# Part 2. 연습을 통해 완벽해진다

## 14. 소프트웨어 개발이란

##### 14.1 소프트웨어(음식) 성분

양심적인 소프트웨어 개발자로서, 우리는 적절한 방식으로 적절한 제품을 작성하길 갈망해야 한다. 훌륭한 프로그래머의 주용 특징 중 하나는 작성한 소프트웨어와 그 작성법에 대해 진심으로 주의를 기울이는 것이다.
애정 어린 장인 정신을 바탕으로 코드를 작성해야 한다.

소프트웨어의 특성을 알아보고, 알파벳 모양 파스타같은 것을 만들지 않도록 냄비 속을 볼 것이다.

당신은 프로그래머로서 나아지길 원하는가? 적절한 방식으로 적절한 코드를 작성하기를 실제로 원하는가?
만약 아니오라면 당장 하던 일을 때려치우고 멈춰야 한다.

##### 14.2 소프트웨어 개발은 예술이다.

훌륭한 프로그래머는 어느 정도는 위대한 예술가가 되어야 한다. 소프트웨어 개발 절차 중 많은 부분이 예술 작품을 창조하는 것과 유사하다.

- 창조적 : 상상력이 필요하다. 능숙하게 구축하고 정확하게 설계해야 한다. 프로그래머는 자신이 만들고자 하는 코드에 대한 비전, 만드는 방법에 대한 계획이 있어야 한다. 이는 독창성을 필요로 한다.
- 미학적 : 좋은 코드의 특징은 우아함, 아름다움, 균형에서 찾을 수 있다. 좋은 코드의 기준이 특정 문화적 관례의 프레임워크 안에 있음을 의미한다. 코드 외관 역시 고려한다.
- 기계적 수동적
- 팀 기반 




