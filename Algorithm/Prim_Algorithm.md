## Prim's Algorithm  

**���� �˰����̶�?**  
Kruskal Algorithm�� ���� MST(Minimal Spanning Tree)�� ����� ���� ����̴�.
Ž������ ���(Greedy Method)�� �̿��Ѵ�.  

>**Spanning Tree(���д� Ʈ��)**  
>������ ���� �׷������� ��� Node�� �����ϸ鼭 Cycle�� �̷��� �ʴ� ��� Spanning Tree��� �Ѵ�.  

> **MST(Minimal Spanning Tree, �ּ� ��� ���� Ʈ��)**  
>1. Spanning Tree ������ ����  
>2. Edge�� ���� �ּ�  

>**Greedy Method**  
>- ������ �ؾ� �� ������ �� ������ ���� ���ٰ� �����Ǵ� ���� ���������ν� �������� �ش信 �����ϴ� ��  
>- Ž������ ����� �� �������� ����������, ��ü���� �������� �����̶�� ������ ���� ������ �ݵ�� �����ؾ� �Ѵ�.  
>- ������ Kruskal �˰����� ������ �ش��� �ִ� ������ ����Ǿ� �ִ�.  

**[���� �˰����� ����](https://ko.wikipedia.org/wiki/%ED%94%84%EB%A6%BC_%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98)**  
1. Graph�� �� Node�� �����Ѵ�.  
2. Node�� ����� ����ġ�� ���� ���� Edge�� �����Ѵ�.  
3. ����� Node��� ����� ����ġ�� ���� ���� Edge�� �����Ѵ�.  
	���ο� Edge�� ���ο� Node�� ����ȴ�. 
4. 2�� ���ư� �ݺ��Ѵ�.  
	��� ������ ����� ������ �ݺ��Ѵ�.  

**ũ�罺Į vs ���� ��**  
ũ�罺Į�� ���� ��� ����ġ�� ���� ����(Edge)�� �����Ѵ�. ��, ������ �ּ��� �����ϴ� Greedy Method�� �̿��Ѵ�.  
| Kruskal| Prim |
|--|--|
| ũ�罺Į�� ��쿡�� ����(Edge)�� ����ġ�� ������������ ������ ��, ���������� �����Ͽ� MST�� �����. | ������ ��쿡�� �� ������ Node(����)�� ���� ����ġ�� ���� ������ �̾���̸� MST�� �����. |

**������ �ð� ���⵵**   
- O(Elog N)  
	- Extract-Min : O(Nlog N)  
	- Search and Decrease-Key : O(Elog N)  
	- O(Nlog N + Elog N) = O(Elog N)  
- O(E + logN)  
	- �Ǻ���ġ �� ��� �� 

>**Extract-Min**  
>Extract-Min : ���� ���� ��Ҹ� ��ȯ�� ��, �����Ѵ�.  
>Extract-Max : ���� ū ��Ҹ� ��ȯ�� ��, �����Ѵ�.  

>**Search and Decrease-Key**  
>Search : Ʈ���� ����(Node ��)��ŭ Ž��(O(log N))�ؾ��Ѵ�.  
>Decrease-Key : ��� Node�� ���� Edge ����ġ ������Ʈ(O(E/Vlog V))�� ����ǹǷ� O(E logV)�� �ð����⵵�� ���´�.  

>**Fibonacci heap(�Ǻ���ġ ��)**  
>�켱���� ť(priority queue) ������ ���� �ڷ� ������, ��-���ĵ� Ʈ���� ��Ƴ��� �ڷ� �����̴�.  
>���� �����ϴ� ������ �Ǻ���ġ ������ �����Ͽ� �Ǻ���ġ ������ �Ҹ���. 

������  
[https://ko.wikipedia.org/wiki/%ED%94%84%EB%A6%BC_%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98](https://ko.wikipedia.org/wiki/%ED%94%84%EB%A6%BC_%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98)  
[https://m.blog.naver.com/PostView.nhn?blogId=kimmy5000&logNo=220635475967&proxyReferer=https:%2F%2Fwww.google.com%2F](https://m.blog.naver.com/PostView.nhn?blogId=kimmy5000&logNo=220635475967&proxyReferer=https:%2F%2Fwww.google.com%2F)  
[https://www.cs.auckland.ac.nz/software/AlgAnim/prim.html](https://www.cs.auckland.ac.nz/software/AlgAnim/prim.html)  
[https://journee912.tistory.com/67](https://journee912.tistory.com/67)   