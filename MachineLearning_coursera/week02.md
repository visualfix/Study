# Week2
## 1. Multivariate Linear Regression
### 1.1. Multiple Features
**Multivariate Linear Regression(다변량 선형 회귀)**
다중 변수를 사용하는 선형회귀를 다변량 선형회귀라 한다

$$\begin{align*}x_j^{(i)} &= i\text{번째 학습 예제의 }  j \text{번째 피처 값} \newline x^{(x)} &=  i\text{번째 학습 예제의 피처 입력 값들} \newline m &= \text{학습 예제의 수} \newline n &= \text{피처의 수} \end{align*}$$

다중변수가 적용된 가설 함수는 아래와 같다
$$\begin{align*}h_{\theta}(x) &= \theta_0 + \theta_1x_1 + \theta_2x_2 + \theta_3x_3 + ... + \theta_nx_n  \end{align*}$$