# [Bronze V] 행렬 덧셈 - 2738 

[문제 링크](https://www.acmicpc.net/problem/2738) 

### 성능 요약

메모리: 30616 KB, 시간: 48 ms

### 분류

구현(implementation), 수학(math)

### 문제 설명

<p>N*M크기의 두 행렬 A와 B가 주어졌을 때, 두 행렬을 더하는 프로그램을 작성하시오.</p>

### 입력 

 <p>첫째 줄에 행렬의 크기 N 과 M이 주어진다. 둘째 줄부터 N개의 줄에 행렬 A의 원소 M개가 차례대로 주어진다. 이어서 N개의 줄에 행렬 B의 원소 M개가 차례대로 주어진다. N과 M은 100보다 작거나 같고, 행렬의 원소는 절댓값이 100보다 작거나 같은 정수이다.</p>

### 출력 

 <p>첫째 줄부터 N개의 줄에 행렬 A와 B를 더한 행렬을 출력한다. 행렬의 각 원소는 공백으로 구분한다.</p>

### MY MEMO

 <p>행렬 문제니까 우선 이차원 배열을 생각할 것이다. 나 또한 그랬다. 행렬 내부의 원소들을 각각 받을 수는 있겠지만 입력 조건 상 한 줄에 한 행의 원소를 입력하는 것이다. 그래서 반복문을 사용하여 한 행씩 넣어줬다.</p>
 <p>배열 관련 문제를 풀다보니 느낀거는 내가 배열 입력을 이상하게 하고 있었다는 것이다. 5596번처럼 input1 = list(map(int, input().split()))로 입력받고 그 입력받은 데이터를 mat1.append(input1)를 통해 넣어주는 방식으로 해야한다. 처음에는 mat1.append(int(input().split()))라 해놓고 왜 안되지 그랬었는데, 이거는 리스트를 다루기 때문에 리스트 변환해주는 함수인 list()를 이용해야 한다.</p>
 <p>행렬 문제를 풀 때에는 행과 열의 변수를 꼭! 확실하게 인지하도록 하자.</p>
 <p>파이썬의 특징이라 할 만큼 간략하고 유연하게 표현할 수 있도록 하자. 출력문 안에 바로 행렬 내 원소들간의 합을 구하면 되겠지.?</p>

