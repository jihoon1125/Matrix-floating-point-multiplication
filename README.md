# Matrix-floating-point-multiplication
이 프로젝트의 목표는 [부스 알고리즘](https://en.wikipedia.org/wiki/Booth%27s_multiplication_algorithm)을 활용하여 부동소수점 정방행렬 곱셈연산의 성능(state * code size)을 최대로 끌어올려보는 것이다. 최종 성능은 어셈블리설계및실습 수업의 조교님들이 작성한 testcase로 평가된다.
* 30x30 사이즈의 행렬을 기준으로 잡고 진행할 것이다.
* Booth multiplication method: 4-Radix 
* 작업 IDE: uVision(ARM)
* Nan, Inf, divide by zero 예외처리
* 성능평가 결과: 100.0 / 100.0 (전체 수강생 33명 중 1위)
---
## Overall Flowchart 

![image](https://user-images.githubusercontent.com/67624104/118237513-552bd580-b4d2-11eb-93a1-b2561016c21d.png)


---


## Multiply Flowchart
![image](https://user-images.githubusercontent.com/67624104/118238196-28c48900-b4d3-11eb-8fd6-f0500d0c0fba.png)


---


## Addition Flowchart
![image](https://user-images.githubusercontent.com/67624104/118236845-8d7ee400-b4d1-11eb-9877-327f587509af.png)


---


## Performance & Result


* Code size


![image](https://user-images.githubusercontent.com/67624104/118237244-13029400-b4d2-11eb-9779-808481017e85.png)

### Data1
* State
States: 11152801

* Result


![image](https://user-images.githubusercontent.com/67624104/118237371-3594ad00-b4d2-11eb-8407-81c07954e66b.png)

### Data2
* State
States: 9370336

* Result


![image](https://user-images.githubusercontent.com/67624104/118238039-f3b83680-b4d2-11eb-9811-ef9ddfaa2fc0.png)

### Data3
* State
States: 667644

* Result


![image](https://user-images.githubusercontent.com/67624104/118238100-092d6080-b4d3-11eb-976c-7da80fdd8555.png)
