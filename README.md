
# 종만북

## 문제해결 
방법
1. 문제를 읽고 이해 
 - 입출력을 보고 유추 x
2. 문제를 익숙한 용어로 재정의
3. 해결할 계획 수립
- 사용할 알고리즘 자료구조 선택
4. 계획 검증
5. 코딩
6. 피드백 및 개선
- 문제에 대한 경험을 적어야됨
- 무슨 알고리즘을 썻는지 왜 그렇게 생각했는지

전략
1. 직관과 체계적인 접근
 - 경험을 통해 직관을 쌓아야함
 - 체계적 접근
	- 비슷한 문제를 풀어봤는지
	- 무식하게 풀어보고 경우의수 줄이기
	- 수식화 해보기
	- 문제 자체를 단순화
	- 그림 그려보기
	- 문제 분해
	- 뒤에서부터 생각
	- 순서를 강제
## 코딩과 디버깅
코딩
- 간결한 코드 작성
- 코드 재사용
- 표준 라이브러리 stl등 사용
- 일관성있는 코드 작성
- 변수, 함수 등 명료한 명명
- 자료의 정규화
- 코드와 데이터 분리

디버깅

- 대부분의 경우 눈으로 디버깅 (코드가 짦으며 컴퓨터가 대수가 제한 될수 있어서)
- assert를 사용하여 디버깅 또는 출력

테스트
- 가장 작은 입력과 큰입력
- 스캐폴딩을 사용하여 디버깅( 테스트 코드를 작성하여 입력값을 랜덤으로 검증하는 함수와 비교)

## 알고리즘 분석
알고리즘을 평가하는 기준
- **시간복잡도** : 입력의 개수나 크기가 결정
	- 선형이하 : NlogM+c 
	- 선형시간 : 1차함수 N+M
	- 지수시간 : <a href="https://www.codecogs.com/eqnedit.php?latex=\inline&space;N^M" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\inline&space;N^M" title="N^M" /></a>
- 공간복잡도( 컴퓨터 하드웨어 발달로 자원이 넉넉해짐 )

점근적 표기법 : O 표기(반복문이 결정)
 - EX) <a href="https://www.codecogs.com/eqnedit.php?latex=\inline&space;\sqrt{5}/3N^2&space;-&space;NlogN&space;&plus;16N" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\inline&space;\sqrt{5}/3N^2&space;-&space;NlogN&space;&plus;16N" title="\sqrt{5}/3N^2 - NlogN +16N" /></a> 라는 수식이 있으면 최고차항이 가장 큰 영향을 끼치며 상수는 숫자가 커질수록 의미가 없기때문에 O(<a href="https://www.codecogs.com/eqnedit.php?latex=\inline&space;N^2" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\inline&space;N^2" title="N^2" /></a>)이 된다.

평가하는 이유
- 알고리즘 문제 해결에는 제한시간이 있다.
- 1초당 <a href="https://www.codecogs.com/eqnedit.php?latex=\inline&space;10^8" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\inline&space;10^8" title="10^8" /></a>으로 생각하면 편하다(절대적 기준이 아님)
