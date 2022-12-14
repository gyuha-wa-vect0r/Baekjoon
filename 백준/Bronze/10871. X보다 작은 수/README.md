# [Bronze V] X보다 작은 수 - 10871 

[문제 링크](https://www.acmicpc.net/problem/10871) 

### 성능 요약

메모리: 31732 KB, 시간: 48 ms

### 분류

구현(implementation)

### 문제 설명

<p>정수 N개로 이루어진 수열 A와 정수 X가 주어진다. 이때, A에서 X보다 작은 수를 모두 출력하는 프로그램을 작성하시오.</p>

### 입력 

 <p>첫째 줄에 N과 X가 주어진다. (1 ≤ N, X ≤ 10,000)</p>

<p>둘째 줄에 수열 A를 이루는 정수 N개가 주어진다. 주어지는 정수는 모두 1보다 크거나 같고, 10,000보다 작거나 같은 정수이다.</p>

### 출력 

 <p>X보다 작은 수를 입력받은 순서대로 공백으로 구분해 출력한다. X보다 작은 수는 적어도 하나 존재한다.</p>
 
### MY MEMO

 <p>우선 이 문제를 풀기위해서는 배열을 이용해야 한다. 배열 중에 리스트랑 튜플이 있지만 배열 원소를 한 줄로 입력받아 넣기 위해서는 리스트가 적당하다고 생각했다. 튜플은 초기에 한번 정의하면 수정이 불가하다. 배열에다 입력한 원소를 다 집어놓고 비교문을 이용하여 입력한 값보다 작은거만 새로운 리스트로 빼내는 방식을 이용했다.</p>
 <p>한 줄로 입력한 원소들을 배열에다가 집어넣는 방법 : arr = list(map(int, input().split())) 이용</p>
 <p>여기서 map(특정 자료형, 어느 리스트) 라 함은 어느 리스트의 모든 원소를 특정 자료형으로 변환해준다. 그리고 list(입력 값)는 입력한 값을 배열로 변환해준다.</p>
 <p>배열의 크기를 측정하는 함수 : len(), 이 함수는 배열용 함수가 아니라 파이썬의 일반적 내장함수이므로 arr.len()과 같이 이상한 방식으로 쓰지 말 것!. len(arr)이라 하면 arr의 크기를 알려준다.</p>

