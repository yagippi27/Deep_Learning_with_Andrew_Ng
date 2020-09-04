# 학습내용

- J(a,b,c)=3(a+bc) 의 계산 그래프 만드는 과정
<br>&nbsp; u = bc
<br>&nbsp; v = a+u
<br>&nbsp; J = 3v

![image](https://cphinf.pstatic.net/mooc/20180615_270/1529026981725rnVc0_PNG/image.PNG?type=w760)


- 정방향 패스, 정방향 전파는 신경망의 출력값을 계산하고, 이는 역방향 패스, 역방향 전파로 이어져 경사나 도함수를 계산함

- 계산 그래프는 J 같은 특정한 출력값 변수를 최적화하고 싶을 때 유용함
- 로지스틱 회귀인 경우 J는 당연히 최적화할 비용 함수임.
