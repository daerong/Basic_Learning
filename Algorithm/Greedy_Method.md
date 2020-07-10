## Greedy Method

**탐욕 알고리즘이란?**  
그 순간에 최적인 것을 선택하는 방식으로 최적해를 구하는 기법입니다.  
여러 경우 중 하나를 결정해야 할 때, 그 순간에 최적이라고 생각되는 것을 선택해 나가는 방식  

**탐욕 알고리즘의 특징**  
순간의 선택 지역적으로 최적이지만 최종적(전역적)인 해답이 최적이라는 보장은 없다.  
탐욕 알고리즘이 잘 작동하는 문제는 greedy choice property와 optimal substructure 두 가지 속성을 만족합니다.  

> **Greedy Choice Property**  
> 앞의 선택이 이후 선택에 영향을 주지 않는다는 걸 의미합니다.  

> **Optimal Substructure**  
> 문제 전체에 대한 최적해(global optimum)가 부분문제에 대해서도 역시 최적해가 된다는 걸 뜻합니다.  
> 즉, 지역적으로 최적이면서 전역적으로도 최적이 됩니다.  

**예시**  
- Activity-Selection Problem  
- Huffman Coding  

>**Activity-Selection Problem**  
> classroom assignment(교실할당)로도 불리는 한정된 교실에서 최대 수업을 배정하는 문제  
> 시간 복잡도는 O(n)  
	
> **Huffman Coding**  
> 허프만 코딩이란 Greedy Method을 사용해 데이터를 압축하는 기법  
> 시간 복잡도는 O(nlog n)  

참고문서  
[https://ratsgo.github.io/data%20structure&algorithm/2017/11/22/greedy/](https://ratsgo.github.io/data%20structure&algorithm/2017/11/22/greedy/)
