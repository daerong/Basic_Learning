
## Graph  

**그래프의 정의** 
Node, Vertex라고 불리는 정점과, Edge로 불리는 간선들의 조합으로 이루어진 자료구조이다.  

> **Node**  
> 각각이 하나의 객체를 의미하는 점이다.  

> **Edge**  
> Node와 Node를 연결하는 선이다.  

**그래프의 특징**  
- Node와 Edge로 관게를 표현할 수 있다.  
	- 지도, 노선도, 회로 등  
- BFS, DFS로 탐색한다.

> **BFS(Breath-First Search)** 
> 인접 Node를 먼저 방문하는 탐색방법이다.  

> **DFS(Depth-First Search)**  
> 더 이상 방문할 Node가 없을 때까지 순회하고 분기(Branch)를 바꾼다.  

**그래프의 종류**  
- 완전 그래프(Complete Graph)  
	- 모든 Node가 서로 연결되어 있는 그래프   
- 가중치 그래프(Weighted Graph)  
	- Edge마다 가중치 값을 가지고 있는 그래프  
- 부분 그래프(Sub-Graph)  
	- 전체 네트워크에서 각각이 그래프를 이룰 때 이를 부분 그래프라고 한다.  
- 순환 그래프(Cyclic Graph)  
	- Cycle을 가지고 있음  
- 비순환 그래프(Acyclic Graph)  
	- Cycle이 없음  
- 방향 그래프(Directed Graph)  
	- 양방향 이동이 가능하다.  
	- A와 B가 인접한 경우, (A,B)로 표현  
	- (A,B)=(B,A)  
- 무방향 그래프(UnDirected Graph)  
	- 한방향으로만 이동가능하다.  
	- A에서 B로 이동 시, <A,B>로 표현  
	- (A,B)!=(B,A)   
- 연결 그래프(Connected Graph)  
	- 무방향 그래프의 모든 노드가 연결되어 있음  
- 비연결 그래프(Disconnected Graph)  
	- 특정 노드에 대한 경로가 없음  

> **Cycle**  
> 그래프 순회하며 출발 Node를 다시 방문하는 경우 Cycle을 이룬다고 한다.  
  
**그래프 관련 용어**    
- Degree(차수)  
	- 무방향 그래프에서 하나의 Node와 인접한 Node의 수  
	- 차수의 합은 모든 Edge의 수의 2배이다  
- 진입 차수(In-Degree)  
	- 방향 그래프에서 외부에서 오는 간선의 수  
- 진출 차수(Out-Degree) 
	- 방향 그래프에서 외부에서 오는 간선의 수  
- Self-loop  
	- Edge의 양 Node가 같을 때, Self loop라고 한다.  
- Adjacent(인접)  
	- Node가 Edge를 통해 연결되어 있다면 인접했다고 한다.  
- Incident(부속)  
	- 무방향 그래프에서 Node에 연결된 Edge는 부속한다고 한다.  
- Path(경로)  
	- 임의의 Node에서 특정 Node로 가는 방법을 말한다.  
- Simple Path(단순 경로)  
	- Path의 양 끝을 제외하고 중복된 Node가 없는 경우, 이를 단순 경로라고 한다.  
- Cycle  
	- 그래프 내에 생기는 고리를 말한다. Path의 처음과 끝 Node가 같은 경우 Cycle을 형성했다고 한다.  
- Eulerian Trail(오일러 경로)  
	- 그래프에 존재하는 모든 Edge를 한번씩만 방문하는 Path이다.  
- Eulerian Circuit(오일러 회로)  
	- 시작점과 도착점이 같은 Eulerian Trail입니다.  

참고문서  
[https://gmlwjd9405.github.io/2018/08/13/data-structure-graph.html](https://gmlwjd9405.github.io/2018/08/13/data-structure-graph.html)  
