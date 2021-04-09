# Logistic Regression
## 다중선형회귀(Multiple Linear Regression) : 
수치형 설명변수 X와 연속형 숫자로 이뤄진 종속변수 Y간의 관계를 선형으로 가정하고
이를 가장 잘 표현할 수 있는 회귀계수를 데이터로부터 추정하는 모델
### 회귀 계수 결정법 
#### Direct Solution
- 선형회귀의 계수들은 실제값(Y)과 모델 예측값(Y’)의 차이, 오차제곱합(error sum of squares)을 최소로 하는 값을 회귀 계수로 선정
- X와 Y데이터 만으로 회귀 계수를 구할 수 있음
#### Numerical Search
- 경사하강법(gradient descent) 같은 반복적인 방식으로 선형회귀 계수를 구할 수 있음
- 경사하강법:   
  어떤 함수 값(목적 함수, 비용 함수, 에러 값)을 최소화하기 위해 임의의 시작점을 잡은 후 해당 지점에서의 그래디언트(경사)를 구하고, 그래디언트의 반대 방향으로 조금씩 이동하는 과정을 여러번 반복하는 것
- 경사 하강법 종류:
  - Batch Gradient Descent (GD) : 파라미터를 업데이트 할 때마다 모든 학습 데이터를 사용
  - Stochastic Gradient Descent (SGD) : 파라미터를 업데이트 할 때, 무작위로 샘플링된 학습 데이터를 하나씩만 이용
  - Mini Batch Gradient Descent: 파라미터를 업데이트 할때마다 일정량의 일부 데이터를 무작위로 뽑아
## 정규화 :
variance를 감소시켜 일반화 성능을 높이는 기법
- 회귀계수가 가질 수 있는 값에 제약조건을 부여하여 미래 데이터에 대한 오차 기대
- 미래데이터에 대한 오차의 기대 값은 모델의 Bias와 variance로 분해 가능
## Bias-Variance Decomposition :
일반화(generalization) 성능을 높이는 정규화(Regularization), 앙상블(ensemble) 기법의 이론적 배경
## 로지스틱 함수 (Logistic function) : 
=sigmoid function, S-커브 함수
![img](https://wikidocs.net/images/page/32046/ANN_Sigmoid.png)
## 승산 (Odds) : 
임의의 사건 A가 발생하지 않을 확률 대비 일어날 확률의 비율
## 이항 로지스틱 회귀 
- Y가 범주형 일 경우, 회귀 모델을 적용할 수 없음

## 이항 로지스틱 회귀의 결정 경계
![img2](https://i.imgur.com/tqQ3WdX.png)
