## Prim's Algorithm  

**프림 알고리즘이란?**  
Kruskal Algorithm과 같은 MST(Minimal Spanning Tree)를 만들기 위한 방법이다.
탐욕적인 방법(Greedy Method)을 이용한다.  

>**Spanning Tree(스패닝 트리)**  
>방향이 없는 그래프에서 모든 Node를 포함하면서 Cycle을 이루지 않는 경우 Spanning Tree라고 한다.  

> **MST(Minimal Spanning Tree, 최소 비용 신장 트리)**  
>1. Spanning Tree 조건을 충족  
>2. Edge의 합이 최소  

>**Greedy Method**  
>- 결정을 해야 할 때마다 그 순간에 가장 좋다고 생각되는 것을 선택함으로써 최종적인 해답에 도달하는 것  
>- 탐욕적인 방법은 그 순간에는 최적이지만, 전체적인 관점에서 최적이라는 보장이 없기 때문에 반드시 검증해야 한다.  
>- 다행히 Kruskal 알고리즘은 최적의 해답을 주는 것으로 증명되어 있다.  

**[프림 알고리즘의 동작](https://ko.wikipedia.org/wiki/%ED%94%84%EB%A6%BC_%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98)**  
1. Graph의 한 Node를 선택한다.  
2. Node에 연결된 가중치가 가장 작은 Edge를 선택한다.  
3. 연결된 Node들과 연결된 가중치가 가장 작은 Edge를 선택한다.  
	새로운 Edge는 새로운 Node에 연결된다. 
4. 2로 돌아가 반복한다.  
	모든 정점이 연결될 때까지 반복한다.  

**크루스칼 vs 프림 비교**  
크루스칼과 프림 모두 가중치가 낮은 간선(Edge)을 선택한다. 즉, 순간의 최선을 선택하는 Greedy Method를 이용한다.  
| Kruskal| Prim |
|--|--|
| 크루스칼의 경우에는 간선(Edge)의 가중치를 오름차순으로 정렬한 뒤, 순차적으로 선택하여 MST를 만든다. | 프림의 경우에는 양 끝단의 Node(정점)을 통해 가중치가 낮은 간선을 이어붙이며 MST를 만든다. |

**프림의 시간 복잡도**   
- O(Elog N)  
	- Extract-Min : O(Nlog N)  
	- Search and Decrease-Key : O(Elog N)  
	- O(Nlog N + Elog N) = O(Elog N)  
- O(E + logN)  
	- 피보나치 힙 사용 시 

>**Extract-Min**  
>Extract-Min : 가장 작은 요소를 반환한 후, 삭제한다.  
>Extract-Max : 가장 큰 요소를 반환한 후, 삭제한다.  

>**Search and Decrease-Key**  
>Search : 트리의 길이(Node 수)만큼 탐색(O(log N))해야한다.  
>Decrease-Key : 모든 Node에 대해 Edge 가중치 업데이트(O(E/Vlog V))가 실행되므로 O(E logV)의 시간복잡도를 갖는다.  

>**Fibonacci heap(피보나치 힙)**  
>우선순위 큐(priority queue) 연산을 위한 자료 구조로, 힙-정렬된 트리를 모아놓은 자료 구조이다.  
>힙이 결합하는 과정이 피보나치 수열과 유사하여 피보나치 힙으로 불린다. 

참고문서  
[https://ko.wikipedia.org/wiki/%ED%94%84%EB%A6%BC_%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98](https://ko.wikipedia.org/wiki/%ED%94%84%EB%A6%BC_%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98)  
[https://m.blog.naver.com/PostView.nhn?blogId=kimmy5000&logNo=220635475967&proxyReferer=https:%2F%2Fwww.google.com%2F](https://m.blog.naver.com/PostView.nhn?blogId=kimmy5000&logNo=220635475967&proxyReferer=https:%2F%2Fwww.google.com%2F)  
[https://www.cs.auckland.ac.nz/software/AlgAnim/prim.html](https://www.cs.auckland.ac.nz/software/AlgAnim/prim.html)  
[https://journee912.tistory.com/67](https://journee912.tistory.com/67)   