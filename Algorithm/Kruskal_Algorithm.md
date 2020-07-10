## Kruskal's Algorithm (MST)  

**ũ�罺Į�̶�?**  
Spanning Tree�� ���� �ּҷ� �ϴ� MST(Minimal Spanning Tree)�� ����� ���� ����̴�.  
Ž������ ���(Greedy Method) �� �̿��Ѵ�.  

>**Spanning Tree(���д� Ʈ��)**  
>������ ���� �׷������� ��� Node�� �����ϸ鼭 Cycle�� �̷��� �ʴ� ��� Spanning Tree��� �Ѵ�.  

> **MST(Minimal Spanning Tree, �ּ� ��� ���� Ʈ��)**  
>1. Spanning Tree ������ ����  
>2. Edge�� ���� �ּ�  

>**Greedy Method**  
>- ������ �ؾ� �� ������ �� ������ ���� ���ٰ� �����Ǵ� ���� ���������ν� �������� �ش信 �����ϴ� ��  
>- Ž������ ����� �� �������� ����������, ��ü���� �������� �����̶�� ������ ���� ������ �ݵ�� �����ؾ� �Ѵ�.  
>- ������ Kruskal �˰����� ������ �ش��� �ִ� ������ ����Ǿ� �ִ�.  

**[ũ�罺Į�� ����](https://ko.wikipedia.org/wiki/%ED%81%AC%EB%9F%AC%EC%8A%A4%EC%BB%AC_%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98)**  
1. Graph�� Edge���� ����ġ�� ������������ �����Ѵ�.  
2. ����ġ�� ���� ���� Edge�� �����Ѵ�.  
	Cycle�� ����� ��� �����Ѵ�.  
3. �ΰ��� Node�� ���� �����Ѵ�.  
	Edge�� �̹� ������ ��� �����Ѵ�.  
4. �� ������ �ݺ��Ѵ�.  

>**Graph**  
>�׷����� Vertex��� �Ҹ��� ����(Node)��, Edge�� �Ҹ��� �������� �������� �̷�����ִ�.  

>**���ǻ���**  
>- ���ο� Edge�� �̹� ����Ǿ� �ִ� Node�鿡 ����� �� Cycle�� �����ȴ�.  
>	- ��, �߰��� Edge�� �� Node�� ���� ���տ� ���� ������ Cycle�� �����ȴ�.  
>- Cycle ���� ���θ� Ȯ���ϴ� ���  
>	- �߰��ϰ��� �ϴ� Edge�� �糡 Node�� ���� ���տ� ���� �ִ����� ���� �˻��ؾ� �Ѵ�.  
>	- 'union-find �˰���' �̿�  

**ũ�罺Į�� �ð� ���⵵**  
- O(Elog N)
	- Edge ���� : O(Elog E)
	- Union-FInd : O(Elog N)
	-  O(Nlog N + Elog N) = O(Elog N)
	
������  
[https://ko.wikipedia.org/wiki/%ED%81%AC%EB%9F%AC%EC%8A%A4%EC%BB%AC_%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98](https://ko.wikipedia.org/wiki/%ED%81%AC%EB%9F%AC%EC%8A%A4%EC%BB%AC_%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98)  
[https://gmlwjd9405.github.io/2018/08/29/algorithm-kruskal-mst.html](https://gmlwjd9405.github.io/2018/08/29/algorithm-kruskal-mst.html)  
[https://yabmoons.tistory.com/186](https://yabmoons.tistory.com/186)  
