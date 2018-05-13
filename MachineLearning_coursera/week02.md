# Week2
## 1. Multivariate Linear Regression
### 1.1. Multiple Features
**Multivariate Linear Regression(다변량 선형 회귀)**
다중 변수를 사용하는 선형회귀를 다변량 선형회귀라 한다

$$\begin{align*}x_j^{(i)} &= i\text{번째 학습 예제의 }  j \text{번째 피처 값} \newline x^{(x)} &=  i\text{번째 학습 예제의 피처 입력 값들} \newline m &= \text{학습 예제의 수} \newline n &= \text{피처의 수} \end{align*}$$

다중변수가 적용된 가설 함수는 아래와 같다
$$\begin{align*}h_{\theta}(x) &= \theta_0 + \theta_1x_1 + \theta_2x_2 + \theta_3x_3 + ... + \theta_nx_n  \end{align*}$$

이 함수의 각 인자는 같이 생각할 수 있다.

|||||
|-|-|-|-|
|$$\theta_0$$|기본 집 값| | |
|$$\theta_1$$|평당 가격|$$x_1$$|평수|
|$$\theta_2$$|층당 가격|$$x_2$$|층수|

행렬 곱의 정의에 따라 가설함수는 아래처럼 간결하게 표시할 수 있다.
$$\begin{align*}h_\theta(x) =\begin{bmatrix}\theta_0 \hspace{2em} \theta_1 \hspace{2em} ... \hspace{2em} \theta_n\end{bmatrix}\begin{bmatrix}x_0 \newline x_1 \newline \vdots \newline x_n\end{bmatrix}= \theta^T x \\ x_0 &= 0 \end{align*} $$


### Gradient Descent for Multiple Variables
 
 다변량 션형회귀의 기울기 하강 공식은 아래와 같다.
 (j번째 피처,  i번째 학습 예제) 

 $$\theta _{ j }\\ =\frac { \delta  }{ \delta \theta _{ i } } J(\theta _{ 0 },\theta _{ 1 })\\ =\alpha \frac { \delta  }{ \delta \theta _{ i } } \frac { 1 }{ 2m } \sum _{ i=1 }^{ m }{ \left\{ { h }_{ \theta  }(x^{ (i) })-y^{ (i) } \right\} ^{ 2 } } \\ =\alpha \frac { 1 }{ m } \sum _{ i=1 }^{ m }{ \left\{ { h }_{ \theta  }(x^{ (i) })-y^{ (i) } \right\} x_j^{ (i) } } $$