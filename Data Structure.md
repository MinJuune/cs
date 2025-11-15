## 1. 연결리스트(Linked List)와 배열(Array)의 차이점에 대해 설명해 보세요.

**배열**은 고정된 크기의 연속된 메모리 공간을 사용하는 선형 자료구조입니다.     
**연결리스트**는 노드들이 데이터와, 다음 노드를 가리키는 포인터로 구성된 선형 자료구조입니다.  
시간복잡도는 배열이, 접근 시 O(1)으로 빠르고, 삽입/삭제 시 O(N)으로 느린 반면,   
연결리스트는, 접근 시 O(N)으로 느리고, 삽입/삭제 시 O(1)으로 빠릅니다.   
     
<p align="center">
  <img src="./img/Data%20Structure/array.png" width="200"><br>
  <em>Array</em>
</p>
<br><br>        
<p align="center">
  <img src="./img/Data%20Structure/linked_list.png" width="200"><br>
  <em>Linked List</em>
</p>

<br><br>
       
## 2. 동적 배열(Dynamic array) 개념과 그 장점에 대해 설명해 보세요.

**동적 배열**은 크기가 가변적인 배열로, 배열이 꽉 차면 자동으로 크기를 증가시키는 자료구조 입니다.  
메모리를 효율적으로 사용하고, 배열의 크기를 동적으로 조정할 수 있는 장점이 있습니다.  

<p align="center">
  <img src="./img/Data%20Structure/Dynamic_Array.png" width="200"><br>
  <em>Dynamic Array</em>
</p>

<br><br>

## 3. 우선순위 큐(Priority Queue)와 힙(Heap)에 대해 설명해 보세요.

**우선순위 큐**는 각 데이터가 우선순위를 가지고 있으며, 일반적인 큐와 달리, 데이터가 들어온 순서가 아니라 우선순위에 따라 먼저 나가는 자료구조입니다.  
**힙**은 완전 이진 트리 기반의 자료구조로, 부모 노드가 자식 노드보다 항상 크거나 작다는 특징을 가집니다.  
부모 노드가 자식 노드보다 크면 Max Heap, 작으면 Min Heap이라 부릅니다.  
우선순위 큐를 구현할 때 Heap을 사용할 수 있습니다.   

<p align="center">
  <img src="./img/Data%20Structure/priority_queue.png" width="200"><br>
  <em>Priority Queue</em>
</p>
<br><br>
<p align="center">
  <img src="./img/Data%20Structure/heap.png" width="200"><br>
  <em>Heap</em>
</p>

<br><br>

## 4. 이진 트리에 대해 설명해 보세요.

**이진 트리**는 각 노드가 최대 2개의 자식 노드를 가지는 트리 자료구조로,  
완전 이진 트리, 포화 이진 트리, 편향 이진 트리 3가지 형태가 있습니다.  
<strong>완전 이진 트리(complete binary tree)</strong>는 마지막 레벨을 제외한, 모든 노드들이 채워진 형태,    
<strong>포화 이진 트리(full binary tree)</strong>는 모든 노드가 0개 또는 2개의 자식을 가지는 형태,    
<strong>편향 이진 트리(skewed binary tree)</strong>는 한쪽으로만 치우친 형태입니다.     

<p align="center">
  <img src="./img/Data%20Structure/binary_tree.png" width="200"><br>
  <em>Binary Tree</em>
</p>
<br><br>
<p align="center">
  <img src="./img/Data%20Structure/complete_binary_tree.png" width="200"><br>
  <em>Complete Binary Tree</em>
</p>
<br><br>
<p align="center">
  <img src="./img/Data%20Structure/full_binary_tree.png" width="200"><br>
  <em>Full Binary Tree</em>
</p>
<br><br>
<p align="center">
  <img src="./img/Data%20Structure/skewed_binary_tree.png" width="200"><br>
  <em>Skewed Binary Tree</em>
</p>
<br><br>

<br><br>

## 5. 이진 탐색 트리(Binary Search Tree)에 대해 설명해 보세요

**이진 탐색 트리**는,  
왼쪽 서브 트리에 있는 모든 노드의 값이 부모보다 작고,  
오른쪽 서브 트리에 있는 모든 노드 값이 부모보다 큰 이진 트리입니다.  

<p align="center">
  <img src="./img/Data%20Structure/binary_search_tree.png" width="200"><br>
  <em>Binary Search Tree</em>
</p>
<br><br>

## 6. 균형 이진 트리(Balanced Binary Tree)에 대해 설명해 보세요.

**균형 이진 트리**는 모든 노드에서 왼쪽과 오른쪽 서브 트리의 높이 차이가 1 이하인 트리로, 대표적인 예로 AVL 트리, Red-Black 트리가 있습니다.   
**AVL 트리**는 균형을 유지하기 위해 노드를 삽입하거나 삭제한 후, 높이 차이가 2 이상이면, 회전 연산(LL,RR,LR,RF)을 수행하여 균형을 유지합니다.    
**Red-Black 트리**는 각 노드에 빨강/검정 색 속성을 추가한 균형 이진 탐색 트리로, 균형 조건을 느슨하게 해서, 회전이 적고, 효율적이라는 특징이 있습니다.  

<p align="center">
  <img src="./img/Data%20Structure/AVL_tree.png" width="200"><br>
  <em>AVL Tree</em>
</p>
<br><br>
<p align="center">
  <img src="./img/Data%20Structure/red-black_tree.png" width="200"><br>
  <em>Red-Black Tree</em>
</p>
<br><br>

## 7. 해시 테이블이랑 충돌에 대해 설명해 보세요.

**해시 테이블**은 데이터를 key-value 쌍으로 저장하고, 해시 함수를 사용하여 key를 배열의 인덱스로 변환하는 자료구조입니다.  
이때 서로 다른 key들이 같은 해시 인덱스로 계산될 수 있는데, 이를 충돌(collision)이라 합니다.  
충돌을 해결할 수 있는 방법으로는 Open Addressing이랑 Chaining이 있는데,    
**Open Addressing**은 충돌이 나면, 빈 슬롯을 찾아 이동해서 저장하는 방법이고,  
**Chaining**은 각 슬롯에 연결리스트를 두고, 같은 인덱스에 여러 데이터를 저장하는 방법입니다.   

<p align="center">
  <img src="./img/Data%20Structure/hash_table.png" width="200"><br>
  <em>Hash Table</em>
</p>
<p align="center">
  <img src="./img/Data%20Structure/open_addressinge.png" width="200"><br>
  <em>Open Addressing</em>
</p>
<br><br>
<p align="center">
  <img src="./img/Data%20Structure/chaining.png" width="200"><br>
  <em>Chaining</em>
</p>
<br><br>

## 8. 그래프와 cycle에 대해 설명해 보세요.

**그래프**는 정점(Vertex)과 간선(Edge)로 이루어진 비선형 자료구조로, 객체들간의 관계나 연결을 표현하는 데 사용됩니다.  
그래프에 cycle이 있다는 것은, 한 정점에서 시작해 다시 그 정점으로 돌아오는 경로가 있는 경우를 말하는데, DFS로 방문한 노드를 추적해 cycle 여부를 탐지할 수 있습니다.  

<br><br>

## 9. 최소 신장 트리(Minimum Spanning Tree, MST)에 대해 설명해 보세요.

**최소 신장 트리**는 모든 노드들을 연결하면서, 총 가중치가 최소인 트리입니다.   
이를 구하는 대표적인 알고리즘으로 Kruskal 알고리즘과 Prim 알고리즘이 있습니다.  
**Kruskal**은 간선(Edge)을 오름차순으로 정렬해, cycle이 생기지 않도록 하나씩 선택하는 방식이고,  
**Prim**은 하나의 정점에서 시작해, 연결된 간선 중, 가장 가중치가 작은 간선(Edge)을 추가하여 확장해 나가는 방식입니다.  
(이 둘의 차이점은 Kruskal은 간선 정렬 후 선택, Prim은 한 정점에서 확장)   

<p align="center">
  <img src="./img/Data%20Structure/Minimum_Spanning_tree.png" width="200"><br>
  <em>Minimum Spanning Tree</em>
</p>
<br><br>

## 10. 위상 정렬(Topological Sort)에 대해 설명해 보세요.

**위상 정렬**은 cycle이 없는 방향 그래프에서, 정점들을 순서에 따라 나열하는 정렬 알고리즘입니다.   

<p align="center">
  <img src="./img/Data%20Structure/topology_tree.png" width="200"><br>
  <em>Topology Tree</em>
</p>
<br><br>

## 11. 다익스트라 알고리즘에 대해 설명해 보세요.

**다익스트라 알고리즘**은 가중치가 양수인 그래프에서, 하나의 시작 노드로부터 다른 모든 노드까지의 최단 경로를 구하는 알고리즘입니다.  
Greedy 접근 방식을 사용하며, 매 단계마다 가장 가까운 노드를 선택하고, 그 노드와 연결된 이웃 노드의 거리를 업데이트해 나갑니다.  
음수 가중치의 경우, 벨만-포드 알고리즘을 사용하여 최단 경로를 찾을 수 있습니다.  

<br><br>

## 12. BFS와 DFS의 차이에 대해 설명해 보세요.

<strong>BFS(Breadth-First Search)</strong>는 시작 노드에서 가까운 노드부터 차례대로 탐색하는 알고리즘으로, 최단 경로를 탐색하고자 할 때 사용됩니다.  
<strong>DFS(Depth-First Search)</strong>는 한 경로를 끝까지 탐색한 뒤 다른 경로를 탐색하는 알고리즘으로, 모든 가능한 경로를 탐색하고자 할 때 사용됩니다.  

<p align="center">
  <img src="./img/Data%20Structure/BFS_DFS.png" width="300"><br>
  <em>BFS and DFS</em>
</p>
<br><br>

## 13. Bitmap 자료구조에 대해 설명해 보세요.

**Bitmap**은 데이터의 존재 여부를 0,1의 비트로 표현하는 자료구조입니다.  
특정 값의 존재 여부를 빠르게 확인 가능하다는 특징이 있습니다.   

<p align="center">
  <img src="./img/Data%20Structure/Bitmap.png" width="200"><br>
  <em>Bitmap</em>
</p>
<br><br>

## 14. 이진 탐색(Binary Search)에 대해 설명해 보세요.  

**이진 탐색**은 정렬된 데이터에서, 원하는 값을 효율적으로 찾는 알고리즘입니다.  
탐색 구간의 중간값을, 찾는 값과 비교하고, 찾는 값이 중간 값보다 더 작으면 왼쪽 구간, 찾는 값이 중간 값보다 더 크면 오른쪽 구간만 탐색하도록, 구간을 절반씩 줄여나갑니다.  
시간복잡도는 매번 탐색 범위가 절반으로 줄기 때문에 O(log N)입니다.  

<br><br>

## 15. 트리(Tree)에 대해 설명해 보세요.  

**트리**는 노드와 간선으로 이루어진 비선형 자료구조로, 계층적인 관계를 표현할 때 사용됩니다.  
cycle이 없는 구조를 가집니다.  

<br><br>