##### 10.3.9 도망가지 말라

버그를 발견했다면 해당 코드 구역에 숨어 있는 또 다른 관련된 문제들이 있는지 고려해보라.
이미 해결한 문제는 코드의 다른 구역에서도 반복되는 패턴일 것이다. 코드의 어느 부분에 더 많은 문제가 있는지 메모해라.
이 메모들은 충분한 시간을 들인 다음 코드를 다시 작성하거나 심도 있게 검토하면서 문제 영역에 시간을 할애하는 편이 좋다.

##### 10.4 재현할 수 없는 버그

* 실패를 유발하는 요소들을 기록해두라. 이를 반복하다보면, 어떤 패턴을 찾아내게 되어 공통된 원인들을 식별하는데 도움이 될 것이다.
* 더 많은 정보를 수집하다 보면 결론을 그릴 수 있게 될 것이다.
* 출시 버전이나 베타버전에 더 많은 로그와 assert를 추가하여, 실제 사용자의 사용 시 정보를 획득하는 방법을 검토하라.
* 시스템을 자동화하여 가동할 수 있다면, 버그 사냥 작업이 더 가속화될 수 있다.

_스레드를 이용하는 코드_

_네트워크 상호 작용_

_저장 장치의 다양한 속도_

네트워크의 지연, 느리게 회전하는 디스크, 데이터베이스 작동 등으로 프로그램의 행태가 바뀔 수 있다. 이는 특히 타임아웃의 범위 끝에서 아슬아슬하게 프로그램이 작동하도록 만든 경우 발생한다.

_메모리 손상_

_전역 변수/싱글톤_

##### 10.5 마치며

버그를 만들어내는 것은 우리 자신이다. 효과적인 디버깅은 모든 프로그래머들을 위한 필수적 기술이다.

## 11. 테스트하기

과연 TDD란 무엇일까? TDD는 더 나은 소프트웨어를 만들기 위한 중요한 기법이다.

##### 11.1 왜 테스트하는가

자신의 코드는 자신이 테스트 해야하는 것은 생각할 필요도 없는 당연한 일.
