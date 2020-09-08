# 학습내용

- 컴퓨터의 계산 효율성을 위해서 가능하면 “for loop” 을 피하는 것이 좋습니다.
- 자주 쓰는 넘파이(numpy) 함수:
<br>&nbsp; log
<br>&nbsp; abs
<br>&nbsp; maximum
<br>&nbsp; **
<br>&nbsp; zeros

# 학습자료
- [numpy 수학 관련 함수](https://docs.scipy.org/doc/numpy-1.13.0/reference/routines.math.html)


![image](https://user-images.githubusercontent.com/52098725/92469873-856af800-f210-11ea-9f0c-ff623466b478.png)


- A는 행렬, v는 벡터
- 왼쪽은 비벡터화된 버전, 오른쪽은 벡터화된 버전


![image](https://user-images.githubusercontent.com/52098725/92470835-fb239380-f211-11ea-8bad-dd09b37c046d.png)


- np.exp(v) 함수는 밑(base)이 자연상수 e인 지수함수 y=e^v로 변환해줌.
- np.log(v) 원소의 로그값을 구함. 지수함수의 역함수인 로그함수를 만들어줌. 자연상수 e가 밑.
- np.abs(v) 원소의 절대값을 구하는 함수.
- np.max(v, 0) v의 원소와 0 중에서 더 큰 값을 반환해줌.
- v**2 모든 원소를 제곱한 벡터를 반환.
- 1/v 원소의 역수로 이루어진 벡터를 반환.


![image](https://user-images.githubusercontent.com/52098725/92470887-0bd40980-f212-11ea-8d45-5e46ae3e363e.png)


- for문 두 개 중에 하나를 줄일 수 있음
