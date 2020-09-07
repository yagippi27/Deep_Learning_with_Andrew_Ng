# 학습내용
- 로지스틱 회귀에서 비용 함수는 다음과 같이 표현할 수 있습니다.
<br>&nbsp; J(w,b) = 1 / m ∑[i=1, i=m]( L ( a^(i), y^(i) ) )
- 이를 코드로 표현하면 아래와 같습니다.


![image](https://cphinf.pstatic.net/mooc/20180615_249/1529027949584hxeeh_PNG/image.PNG?type=w760)



- 현재 코드에서는 특성의 개수를 2개로 가정하였지만, 만약 특성의 개수가 많아진다면 이 또한 for문을 이용해 처리해야 합니다. 즉, 이중 for문을 사용하게 되며 이로인해 계산속도가 느려지게 됩니다.
- 다음 시간에는 vectorization을 통해 for문을 사용하지 않고 처리할 수 있는 방법을 배우겠습니다.


![image](https://user-images.githubusercontent.com/52098725/92381775-6c961000-f146-11ea-87fe-ca7345a0fac8.png)


- 비용함수는 각 손실의 평균이라 할 수 있음
- w_1에 대한 전체 비용 함수의 도함수도 w_1에 대한 각 손실 항 도함수의 평균임.


![image](https://user-images.githubusercontent.com/52098725/92381832-86375780-f146-11ea-8f3a-450c3c3b9d47.png)


- dw_1, dw_2, db는 w에 대한 전체 비용 함수의 도함수와 같음
- 즉 훈련 세트 전체를 합한 값을 저장하고 있다는 뜻
