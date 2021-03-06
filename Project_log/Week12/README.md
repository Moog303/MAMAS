## Meeting #15 [18/05/24]
### Quantify 알고리즘 및 UI 개선

- **가족 섭외**
	- 구체적인 실험을 위해 가족 섭외 5/30까지 마무리
	- 6월 첫째 주말에 첫 실험 계획

- **Quantify 알고리즘**
	- 4가지 항목에 대한 평가 : 총 식사시간, 부모 기입 종합 만족도, 언어 사용, 도전 메뉴 식사 횟수, 식사 중단 구간
	- 4가지 항목에 대한 각각의 점수를 합산하여 100점 만점으로 Linear 매핑

	1. 총 식사 시간
		- 30~40분 구간을 100점 만점으로 하여 정규 분포 형태로 점수 환산


	2. 언어 사용 

		<img src="/img/27.png" style="width: 20px;">
		
		- P : 긍정 단어 수, T : 전체 단어 수, N : 부정 단어 수
		- 긍정 언어와 전체 대화양이 많을 수록, 부정적인 언어가 적을 수록 높은 점수 받도록 구성

	3. 도전 메뉴 식사 횟수
		- 메뉴별로 따로 DB화
		- Log scale로 점수화 (횟수가 낮은 구간에서 증가할 때, 점수 폭이 더 크게 상승)

	4. 식사 중단 구간
		- Follow-up 질문을 통해 부정적 식사 중단 구간 Filtering
		- 식사 중단 총 시간을 전체 식사 시간으로 나누어 점수로 환산

- **UI 수정**

	<img src="/img/28.jpeg" style="width: 200px;">

	- 데이터별로 사용자 confirm 따로 받는 것으로 변경
	- 편식 메뉴 워딩 --> 도전 메뉴로 변경
	- 하단 탭 디자인 --> Navigation Bar에서 Icon 형태로 변경
	- 편식 음식 접근의 단위를 횟수로 확정
	- 시간 흐름을 사용자가 알 수 있도록 변경
