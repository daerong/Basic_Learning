##  Divide and Conquer
**분할정복법이란?**   
분할정복법은 주어진 문제를 풀기 위해 작은 문제로 나누고(Divide) 작은 문제를 해결하며 정복(Conquer)하는 과정이다.    

**분할정복법의 특징**    
- 하향식 접근법(Top-Down)으로도 불린다.  
- 분할정복법에서는 문제를 나누는 과정(Divide)이 가장 중요하다.   
	잘 나누어진 문제는 쉽게 해결할 수 있으며 이를 통합하는 과정 또한 쉽다.   
- 나누어진 작은 문제들은 서로 독립적이다.  

> **Top-Down(하향식 접근법)**  
> 최상위 사례(Top)의 해답을 하위(Down)로 내려가면서 구하기 때문에 이 같은 이름이 붙여졌다.  

**분할정복법의 동작**  
1. Divide : 문제를 더 작은 문제로 나눈다.  
	작은 문제의 해답을 쉽게 얻을 수 있으면 해를 구하고 아니면 더 작은 문제로 나눈다.   
2. Conquer : 작은 문제들을 각각 해결(정복)한다.  
3. Combine : 필요하다면, 작은 문제에 대한 해답을 통합하여 원래 문제의 해답을 구한다.   

**분할정복법의 장단점**  
- 장점  
	- 큰 문제의 해답을 찾기 어려울 때, 작은 문제에서 해답을 쉽게 구할 수 있다.  
	- 병렬적으로 문제를 해결하는 데 큰 강점이 있다.  
- 단점  
	- 해결 과정에서 재귀함수가 사용되는 데 이로인한 오버헤드가 발생한다.  
		호출 스택에 Overflow가 발생하거나 과도한 메모리 사용을 하게 되는 단점이 있다.  
	- 작은 문제에서 간단한 해결방법을 찾아야 하나, 이에 대한 명확한 기준을 정하기 어렵다.  

> **Stack Overflow**  
> 재귀함수는 함수안에서 함수를 호출한다. 이 과정에서 순차적으로 스택에 쌓이게 되는데 이를 보관하기 위한 메모리가 필요하다. 즉, 인자를 포함한 함수 내부의 정보가 누적되는 과정에서 Stack 크기를 넘어가는 현상이 발생한다. 이를 Stack Overflow라고 한다.  

**분할정복법 대표문제**  
- Binary Search  
- Merge Sort  
- Quick Sort  

참고문서
[https://kimch3617.tistory.com/entry/%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98-%EB%B6%84%ED%95%A0%EC%A0%95%EB%B3%B5%EB%B2%95-Divide-and-Conquer](https://kimch3617.tistory.com/entry/%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98-%EB%B6%84%ED%95%A0%EC%A0%95%EB%B3%B5%EB%B2%95-Divide-and-Conquer)  