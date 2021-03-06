## Meeting #12 [18/05/09]
### 프로토타이핑 방법 논의

- 현재 연구의 2가지 Main 과제 
 1. 어떻게 센싱할 것인가
 2. 수합된 정보로 부모에게 무엇을 Return할 것인가

- 대화 데이터를 통해 얻을 수 있는 정보 정리 및 이를 통해 분석할 수 있는 결과는 무엇일지 정리

- 센싱은 완전하게 구현하지 못하더라도 어떤 것을 Return 해줄 수 있을지에 대해 집중

<img src="/img/24.jpeg" style="width: 200px;">

----

## Meeting #13 [18/05/13]
### 센싱 기술 리서치

- 교수님 미팅 피드백
 1. 센싱을 간단하게 할 수 있는 방법을 찾아볼 것. 즉, 장비를 추가하지 않고 핸드폰만으로 센싱할 수 있는 정보가 있는지 정의해보고 기술 구현 가능성 검토
 2. 식사 후 정보 제공시 전문가가 아닌 우리가 원인과 결론 형태로 데이터를 가공해서 주는 것은 불확실한 정보를 제공할 가능성이 있음
 3. 세션을 Review하고 사용자가 Reflection할 수 있을 정도의 시각화와 정보 제공을 목표로 삼는 것이 좋을 것

- **스마트폰을 이용한 센싱 방법론 리서치**

<img src="/img/26.jpeg" style="width: 200px;">

 1. **음성 시그널**
 - 스마트폰의 마이크 + Google SpeechToText API를 이용하여 음성 데이터를 문자화 하고, 감정 키워드 추출 가능

 2. **Magnetometer**
 - 쇠 숟가락에 자석을 부착하여 스마트폰의 Magnetometer를 활용한 트래킹 가능. 숟가락이 식판에 가까이 왔다가 떨어지는 패턴을 분석할 수 있고 자기장 변화량에 따라 어떤 구역으로 움직였는지까지 트래킹할 수 있는 가능성이 있음

<img src="/img/25.jpeg" style="width: 200px;">

 3. **시간**
 - 이 부분은 사용자가 식사 세션이 시작되고 끝날 때 Input을 제공해 줌으로써 트래킹 가능