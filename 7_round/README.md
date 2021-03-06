##### 8.1 메커니즘

* 코드 응답

오류에 대한 반환 코드는 무시되기 십상이다. 반환 코드는 가장 보편적인 오류 검출 방법이다.

* 예외

예외는 언어 자체에서 기원하는, 보다 구조적으로 오류를 전달하고 다루는 방법이다. 예외는 완벽하지 않다.
예외를 효과적으로 사용하기 위해서는 많은 규칙을 따라야 한다.

##### 8.2 광기

오류를 잘 처리하지 않으면

* 불안정한 코드
* 불안전한 코드
* 나쁜 구조 - 인터페이스를 개선하면, 반복적인 오류가 성가시지 않을 것이다.

사용자 인터페이스도 마찬가지로 모든 잠재적인 잘못된 상황을 노출시켜야 한다. 어떤 부지런한 사용자가 오류를 알아채고 조치하길 기대하는 것은 좋지 않다.
만약 프로그램 강제 종료 외에 다른 선택이 없을 때는, 자연스럽고도 명확하고 무시할 수 없는 방법으로 알려야한다.

##### 8.3 감형 사유

는 없다.

##### 8.4 마치며

오류를 무시하지 말라.

## 9. 예상하지 못한 것을 예상하기

모든 단계에서, 조금이라도 발생할 가능성이 있는 특이 사항들은 모두 고려해야 한다.

##### 9.1 오류

호출되는 어떤 함수도 예상대로 작동하지 않을 수 있다.

* 오류코드가 운이 좋게 확인되었다 하더라도 절대 무시하지 말라
* 함수에 예외가 생성되었을 때 예외 발생에 대처하도록 코드가 정확히 작동하도록 하라(리소스 누수가 없고, 부적절한 상태가 되지 않도록)

항상 오류를 고려한 코드를 작성하여 그로부터 복구할 수 있도록 하라. 복구하지 못할 오류도 고려하라.
방어적인 코딩을 하는 대신 오류로 인해 시끄럽고 눈에 잘 띄는 실패 상황이 발생하도록 그대로 놔둠으로써, 프로세스 수준에서 오류가 처리되도록 하는 것을 권장한다.

##### 9.2 스레딩

기본적인 동시 실행의 원리와 함께, 스레드 간의 결합도를 완화하여 위험하게 상호 작용하지 않도록 하는 방법을 반드시 이해해야 한다.
경합 조건을 발생시키거나 불필요하게 스레드를 막지 않은 채, 스레드 간에 안정적이고도 신속하게 메세지를 전달하는 메커니즘에 대해서도 숙지해야 한다.

##### 9.3 셧다운

시스템을 종료하고 모든 객체를 파기하는 것은 다중 스레드 시스템에서는 특히 어려운 일이다. 앱이 종료되면서 작업자 객체를 파기하므로, 그 과정에서 이미 파기한 객체를 사용하면 안 된다.
목표 객체가 이미 다른 스레드에 의해 제거된 콜백을 작업 큐에 넣으면 안 된다.

##### 9.4 이야기의 교훈

예상하지 못한 것은 결혼 이상한것이 아니다. 개발 초기에 고려해야 한다. 시간이 지나면 해당 이슈를 적절히 처리하기 어렵다. 이는 괴물이 된다.

##### 9.5 마치며

직접해보라. 마지막으로 작업한 코드를 점검해보라. 꼼꼼히 오류를 처리하였는지 확인하고, 가능성 있는 비정상적 상호 작용을 확인하라. 그리고 개선법은?

## 10. 버그 사냥하기

처음부터 완벽할 수 없기 때문에 버그가 생긴다. 피하지 말라. 어차피 많은 디버깅을 하게 될 것이다. 점차 이에 익숙해질 것이고 잘해낼 것이다.

##### 10.1 경제적 우려

실제로 프로그래머들이 소프트웨어를 디버깅하는데 연간 약 3000억달러에 달하는 엄청난 비용이 소모된다. 
즉 세계 경제를 살리기 위해서라도 개발자에게는 버그를 좀 더 빨리 해결해야 할 책임이 있다.

##### 10.2 대비책 

버그가 생기지 않도록 적극적으로 예방하는 편이 좋다. 섬세한 설계, 코드 검토, 페어 프로그래밍, 심사숙고한 테스트 전략은 가장 중요한 방법론들이다. 도구를 이용해 보라.
디버깅이 코드 작성보다 두배는 힘들다. "미련한 프로그래머는 컴퓨터가 이해할 수 있는 코드를 만들고, 좋은 프로그래머는 사람이 이해할 수 있는 코드를 만든다."

 






