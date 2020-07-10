## Kruskal's Algorithm (MST)  

**크루스칼이란?**  
Spanning Tree의 합을 최소로 하는 MST(Minimal Spanning Tree)를 만들기 위한 방법이다.  
탐욕적인 방법(Greedy Method) 을 이용한다.  

>**Spanning Tree(스패닝 트리)**  
>방향이 없는 그래프에서 모든 Node를 포함하면서 Cycle을 이루지 않는 경우 Spanning Tree라고 한다.  

> **MST(Minimal Spanning Tree, 최소 비용 신장 트리)**  
>1. Spanning Tree 조건을 충족  
>2. Edge의 합이 최소  

>**Greedy Method**  
>- 결정을 해야 할 때마다 그 순간에 가장 좋다고 생각되는 것을 선택함으로써 최종적인 해답에 도달하는 것  
>- 탐욕적인 방법은 그 순간에는 최적이지만, 전체적인 관점에서 최적이라는 보장이 없기 때문에 반드시 검증해야 한다.  
>- 다행히 Kruskal 알고리즘은 최적의 해답을 주는 것으로 증명되어 있다.  

**[크루스칼의 동작](https://ko.wikipedia.org/wiki/%ED%81%AC%EB%9F%AC%EC%8A%A4%EC%BB%AC_%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98)**  
1. Graph의 Edge들을 가중치의 오름차순으로 정렬한다.  
2. 가중치가 가장 작은 Edge을 선택한다.  
	Cycle을 만드는 경우 무시한다.  
3. 두개의 Node를 서로 연결한다.  
	Edge가 이미 형성된 경우 무시한다.  
4. 위 과정을 반복한다.  

>**Graph**  
>그래프는 Vertex라고 불리는 정점(Node)과, Edge로 불리는 간선들의 조합으로 이루어져있다.  

>**주의사항**  
>- 새로운 Edge가 이미 연결되어 있는 Node들에 연결될 때 Cycle이 형성된다.  
>	- 즉, 추가할 Edge의 양 Node가 같은 집합에 속해 있으면 Cycle이 형성된다.  
>- Cycle 생성 여부를 확인하는 방법  
>	- 추가하고자 하는 Edge의 양끝 Node가 같은 집합에 속해 있는지를 먼저 검사해야 한다.  
>	- 'union-find 알고리즘' 이용  

**크루스칼의 시간 복잡도**  
- O(Elog N)
	- Edge 정렬 : O(Elog E)
	- Union-FInd : O(Elog N)
	-  O(Nlog N + Elog N) = O(Elog N)
	
참고문서  
[https://ko.wikipedia.org/wiki/%ED%81%AC%EB%9F%AC%EC%8A%A4%EC%BB%AC_%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98](https://ko.wikipedia.org/wiki/%ED%81%AC%EB%9F%AC%EC%8A%A4%EC%BB%AC_%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98)  
[https://gmlwjd9405.github.io/2018/08/29/algorithm-kruskal-mst.html](https://gmlwjd9405.github.io/2018/08/29/algorithm-kruskal-mst.html)  
[https://yabmoons.tistory.com/186](https://yabmoons.tistory.com/186)  
