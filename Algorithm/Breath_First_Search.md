## BFS(Breath-First Search)
**너비 우선 탐색이란?**    
그래프 탐색에 있어 인접 Node를 먼저 탐색하는 방법이다.  

**너비 우선 탐색의 특징**    
- Queue를 통해 구현한다.  
- 방문여부를 체크해야 한다.   
	Edge가 여러개 연결된 경우 재방문을 막는다.  
- ‘Prim’, ‘Dijkstra’ 알고리즘과 유사  

> **Queue(큐)**  
> 먼저 집어 넣은 데이터가 먼저 나오는 FIFO(First In First Out)구조의 자료구조이다.  

**너비 우선 탐색의 동작**   
1. 임의의 Node를 Queue에 추가한다.  
2. Queue에서 하나의 Node를 꺼내 확인한다.   
	원하는 결과를 얻었다면 종료.  
3. 2에서 꺼낸 Node와 인접한(Edge로 연결된) Node를 Queue에 추가한다.  
	이미 방문한 경우, Queue에 추가하지 않는다.  
4. 2부터 다시 반복한다.  
 
참고문서   
[https://sarah950716.tistory.com/13](https://sarah950716.tistory.com/13)    