# 학습내용

- Logistic Regression Gradient Descent  강의에서  dz^(i) = a^(i) - y^(i) 를 통해 계산할 수 있음을 배웠습니다.
- for문을 사용한다면 아래와 같이 계산해야 합니다.


![image](https://cphinf.pstatic.net/mooc/20180615_244/1529028895251WEzUQ_PNG/pic1.PNG?type=w760)


- 계산 속도의 향상을 위해 벡터를 사용한다면 아래와 같이 계산할 수 있습니다.


![image](https://cphinf.pstatic.net/mooc/20180615_8/152902893889842v4T_PNG/pic2.PNG?type=w760)




![image](https://user-images.githubusercontent.com/52098725/92475846-03330180-f219-11ea-8466-fc75c8939f7e.png)


- dZ는 dz^(m)까지 모든 dz를 가로로 쌓은 것. m차원 열 벡터(1, m)


![image](https://user-images.githubusercontent.com/52098725/92475881-11811d80-f219-11ea-950f-ea8b1b976902.png)


- 로지스틱 회귀를 위한 경사 하강법의 한 반복을 만드는데는 for 문이 필요 없다는 것을 증명했지만, 경사 하강법을 여러번 반복하고 싶다면 횟수에 따라 for문이 필요함. 가장 밖의 for문이 될 것임.
