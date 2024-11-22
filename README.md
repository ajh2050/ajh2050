<h1 align="center">Hi 👋, I'm jeonghyeokAhn</h1>
<h3 align="center">I"m currently leaning AI MACHINE-LEARNING!</h3>
 
<h3 align="left">Connect with me:</h3>
<p align="left">
<a href="https://instagram.com/stabilityhyeok" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/instagram.svg" alt="stabilityhyeok" height="30" width="40" /></a>
</p>

</p>
<h3>Things I code with</h3>
<p>
<img alt="Python" src ="https://img.shields.io/badge/Python-3776AB.svg?&style=for-the-badge&logo=Python&logoColor=white"/>
<img alt="HTML5" src="https://img.shields.io/badge/HTML5-E34F26.svg?&style=for-the-badge&logo=HTML5&logoColor=white"/>
<img alt="CSS3" src="https://img.shields.io/badge/CSS3-1572B6.svg?&style=for-the-badge&logo=CSS3&logoColor=white"/>
<img alt="JavaScript" src="https://img.shields.io/badge/JavaScript-F7DF1E.svg?&style=for-the-badge&logo=JavaScript&logoColor=black"/>
</p>

<a href="file:///C:/Users/drema/Downloads/%EC%95%88%EC%A0%95%ED%98%81-%EA%B3%84%EC%82%B0%EA%B8%B0_%EC%B5%9C%EC%A2%85caculator%20(6).html">

<h3>Inspiring Video</h3>
<a href="https://www.youtube.com/watch?v=T6z-0dpXPvU&t" target="_blank">
    <img src="https://img.youtube.com/vi/T6z-0dpXPvU/0.jpg" alt="Inspiring Video Thumbnail" width="400"/>
</a>
<a href="https://www.youtube.com/watch?v=w9DfC2BHGPA&t" target="_blank">
    <img src="https://img.youtube.com/vi/w9DfC2BHGPA/0.jpg" alt="Inspiring Video Thumbnail" width="400"/>
</a>
<a href="https://www.youtube.com/watch?v=SZcjvjrdomE" target="_blank">
    <img src="https://img.youtube.com/vi/SZcjvjrdomE/0.jpg" alt="Inspiring Video Thumbnail" width="400"/>
</a>

<a href="https://www.youtube.com/watch?v=s7FY3K5b3DU" target="_blank">
    <img src="https://img.youtube.com/vi/s7FY3K5b3DU/0.jpg" alt="Inspiring Video Thumbnail" width="400"/>
</a>


## 통계 분석 및 전처리 도구, 시각화 도구
* numpy
* pandas
* matplotlib

## 호출 방법
```python
import numpy as np
import panas as pd
import matplotlib.pyplot as plt
```

| 랭크(Rank) | 이름         | 예시                |
|:-----------|:-------------|:--------------------|
| 0          | 스칼라(Scalar)       | 1, 7               |
| 1          | 벡터(Vector)  | [3,1,2,5] |
| 2          | 행렬(matrix)  | [[1,3],[5,2]] |
| 3          | 3차원 텐서(3-order tensor)  | [[[1,5,9],[2,6,10]],[[3,7,11],[4,8,12]]]|
| n          | n차원 텐서(n-order tensor)  |       |

## 넘파이 배열의 구조 표기 방법
<img width="700" alt="KakaoTalk_20241122_215712905" src="https://github.com/user-attachments/assets/31377657-386a-4942-9804-ef34f5fba9a8">

## 랭크 2,3 배열 생성하기
```python
A = np.array([[3,2],[5,2]])  #랭크 2 배열 생성
B = np.array([[[1,5,9],[2,6,10]],[[3,7,11],[4,8,12]]]) #랭크 3 배열 생성
```

## arange와 reshape함수
```python
A = np.arange(10) #range10 짜리 배열 생성
A.reshape(2,5) #2*5 배열 생성
```

## 인덱싱
```python
x = np.array([[1,2,3],[4,5,6]])
x
-->array([[1,2,3],
         [4,5,6]])
x[0][0]
-->1
x[1][2]
-->6
```

## 브로드캐스팅 연산
```python
x = np.arange(1,10).reshape(3,3)

print(x+10)
-->
[[11 12 13]
 [14 15 16]
 [17 18 19]]

print(x-2)
-->
[[-1  0  1]
 [ 2  3  4]
 [ 5  6  7]]
 
print(x // 3)
-->
[[0 0 1]
 [1 1 2]
 [2 2 3]]

print(x ** 2)
-->
[[ 1  4  9]
 [16 25 36]
 [49 64 81]]
```
## 연결함수 hstack(수평), vstack(수직)
```python
v1 = np.array([1,2,3])
v2 = np.array([4,5,6])
print(np.vstack((v1,v2)))
-->
[[1 2 3]
 [4 5 6]]
print(np.hstack((v1,v2)))
-->
[1 2 3 4 5 6]
```
## 데이터프레임
![download](https://github.com/user-attachments/assets/a4621666-beff-4078-b94a-4894a65b7b11)

## 선형대수학 기말고사 대비 예제
## ch01 exercise2: 벡터의 노름을 계산하는 알고리즘을 작성하고 , np.linalg.norm()과 동일한 결과를 얻는지 확인
``` python
import numpy as np
def find_vector_norm(v):
    return np.sqrt(np.sum(np.square(v)))

print(find_vector_norm([2,1,3]))
print(np.linalg.norm([2,1,3]))
```

## ch04 excercise1: 3*4 행렬을 생성하고 두 번째 행, 네 번째 열의 원소를 추출
```python
x = np.arange(12).reshape(3,4)
print(x[1][3])
```
## ch04 exercise2: 행렬 c를 만들고 c 행렬을 슬라이싱한 c1을 만들기
```python
x = np.arange(100).reshape(10,10)
print(x[0:5,0:5])
```
## 편향-분산 트레이드오프
<img width="545" alt="KakaoTalk_20241122_220528724" src="https://github.com/user-attachments/assets/f62f895d-f189-4173-94ca-d7f9febc3369">

## 홀드아웃 메서드 기법
<img width="671" alt="KakaoTalk_20241122_220645529" src="https://github.com/user-attachments/assets/d0f6e236-5889-42a3-b515-cb5438089f32">


## 혼동행렬
<img width="327" alt="KakaoTalk_20241122_220305011" src="https://github.com/user-attachments/assets/e96c7e6b-aaeb-46e7-a6e2-8d1c796363d3">


