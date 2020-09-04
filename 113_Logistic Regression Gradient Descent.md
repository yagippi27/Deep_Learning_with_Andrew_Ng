# 학습내용

- 그래프
- 수식
<br>&nbsp; da = − ( y / a ) + ( ( 1 - y ) / (1 - a ) )
<br>&nbsp; dz = a - y  
<br>&nbsp; dw1 = dL / dw1 = x1dz  
<br>&nbsp; db= dL / db = dz

![image](https://user-images.githubusercontent.com/52098725/92247295-facd8480-ef01-11ea-9cd7-694f7bb3ecbc.png)

- a : 로지스틱 회귀의 출력값
- y : 참 값 레이블

![image](https://user-images.githubusercontent.com/52098725/92247357-189ae980-ef02-11ea-9161-2b1a73905904.png)

- 역방향 전파의 마지막 단계는 w와 b를 얼마나 바꾸어야하는 지 계산하는 것.
- w1에 대한 도함수("dw1")는 x1dz와 같고, w2의 변화량을 나타내는 "dw2"는 x2dz와 같음. 그리고 "db" 는 dz.
- 단일 샘플에 대해서만 경사 하강법을 사용한다면, 
<br>&nbsp; α는 학습률
<br>&nbsp; w1 := w1 - αdw1
<br>&nbsp; w2 := w2 - αdw2
<br>&nbsp; b := b - αdb
<br>&nbsp; 와 같다.

![image](https://user-images.githubusercontent.com/52098725/92247472-3bc59900-ef02-11ea-8600-ddee1626036e.png)
