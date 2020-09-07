# 학습내용
- 영상에 있는 코드를 따라서 실습 해보시길 바랍니다.
- SIMD(Single Instruction Multiple Data)는 병렬 프로세서의 한 종류로, 하나의 명령어로 여러 개의 값을 동시에 계산하는 방식입니다. 이는 벡터화 연산을 가능하게 합니다. 따라서 for문으로 하나의 값을 연산하는 것 보다 벡터로 만들어서 한번에 연산하는 것이 더 효율적입니다.


![image](https://user-images.githubusercontent.com/52098725/92386490-d7e3e000-f14e-11ea-9421-b8907031c4f9.png)


- 왼쪽은 벡터화되지 않은 구현, 오른쪽은 벡터화된 구현
- 벡터화된 구현은 w^Tx를 직접 계산함
- 파이썬의 numpy 메소드의 np.dot(w,x)를 이용하여 구할 수 있음
- CPU나 GPU는 SIMD를 사용할 수 있음. GPU가 훨씬 더 기능이 좋음.

```python
import numpy as np
import time

a = np.random.rand(1000000)
b = np.random.rand(1000000)

tic = time.time()
c = np.dot(a, b)
toc = time.time()

print(c)
print("Vectorized version:" + str(1000*(toc-tic)) + "ms")

c = 0
tic = time.time()
for i in range(1000000):
    c += a[i]*b[i]
toc = time.time()

print(c)
print("For loop:" + str(1000*(toc-tic)) + "ms")
```
- 1.5ms VS 481 처리 속도가 300배의 차이가 남
