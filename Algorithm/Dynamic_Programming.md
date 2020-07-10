## DP(Dynamic Programming)

**동적계획법이란?**  
큰 문제를 풀기 위해 작은 문제의 답을 이용하는 방법이다.   
이전 문제의 답을 다음 문제의 답을 구하는 데 사용한다.   

**동적계획법의 특징**  
- 문제를 단순화 한 뒤, 상향식 접근법(Bottom-Up)으로 원래문제를 해결한다.
- Memoization을 사용해 연산횟수를 크게 줄일 수 있다.

> **Bottom-Up(상향식 접근법)**  
> 작은 문제의 해답을 통해 상위 문제를 연속적으로 해결해 나간다. 이러한 방향성은 상향식 접근법과 일치한다.

> **Memoization**  
> 메모이제이션(Memoization)은 계산한 값을 메모리에 저장하는 방식입니다.
> 함수 호출 대신 메모리 접근을 사용해 값을 연산 횟수를 크게 줄일 수 있습니다.

**DP(동적계획법) vs Divide and Conquer(분할정복법)**  

|동적계획법|분할정복법|
|--|--|
|소문제가 독립적이지 않음|소문제가 독립적임|
|Memoization 활용 O|Memoization 활용 X|
|상향식 접근법|하향식 접근법|

**동적계획법 대표문제**  
- Fibonacci

참고문서   
[https://meteorbin.tistory.com/7](https://meteorbin.tistory.com/7)  
[https://velog.io/@polynomeer/%EB%8F%99%EC%A0%81-%EA%B3%84%ED%9A%8D%EB%B2%95Dynamic-Programming](https://velog.io/@polynomeer/%EB%8F%99%EC%A0%81-%EA%B3%84%ED%9A%8D%EB%B2%95Dynamic-Programming)  