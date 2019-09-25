### 문제
어떤 양의 정수 X의 자리수가 등차수열을 이룬다면, 그 수를 한수라고 한다. 등차수열은 연속된 두 개의 수의 차이가 일정한 수열을 말한다. N이 주어졌을 때, 1보다 크거나 같고, N보다 작거나 같은 한수의 개수를 출력하는 프로그램을 작성하시오. 

### 입력
첫째 줄에 1,000보다 작거나 같은 자연수 N이 주어진다.

### 출력
첫째 줄에 1보다 크거나 같고, N보다 작거나 같은 한수의 개수를 출력한다.

### 풀의과정
입력 N에 대하여 1의자리수와 10자리수의 차이를 저장하여 N/10과 같은지 N<10작을때까지 반복한다.  

1. 숫자 N이 들어온다
 2. 숫자 N이 10보다 작으면 정답
 3. gap값과 현재 1의자리와 10자리 차이를 비교 같으면 hansu(number/10, gap) 호출 틀리면 종료

``` c++
#include <stdio.h>
#include <iostream>
#include <algorithm>

using namespace std;

int input, result = 0;
bool hansu(int number, int gap)
{
    if (number < 10)
        result++;

    else if ((number / 10) % 10 - (number % 10) == gap)
        hansu(number / 10, gap);
}
// 1의자리수와 2번째자리수만 확인해 나가자 라는 생각으로 풀었음
int main()
{
    scanf("%d", &input);
    for (int i = 1; i <= input; i++)
        hansu(i / 10, (i / 10) % 10 - (i % 10));

    printf("%d", result);
}
```
