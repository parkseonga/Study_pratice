# 시계열 분석

### 시계열 데이터?
 - 관측치가 시간적 순서를 가진 데이터   
 ex)  주식가격 데이터, 실업률, 기후 데이터 등
 
 ### 시계열 변동요인?
- 추세요인: 장기간&점진적으로 상승하거나 하강
- 순환요인: 수년간의 간격으로 주기적인 패턴
- 계절요인: 단기적이고 주기적인 패턴을 갖고 반복적인 경향
- 불규칙요인: 명확히 설명할 수 없는 요인에 의한 우연변동



### 시계열 자료의 예측방법
1. 양적예측방법(경헙적 법칙을 추정하여 예측)
- 과거의 패턴은 미래에도 지속될 것이라 가정
  - 전통적 시계열 분석 방법: 평활법, 분해법
  
  ![image](https://user-images.githubusercontent.com/33725048/76771968-7bc58200-67e3-11ea-9760-0593afb03ae0.png)

  - 확률적 시계열 분석 방법: ARIMA
  
  
  ![image](https://user-images.githubusercontent.com/33725048/76772025-926bd900-67e3-11ea-96b7-e4394530e739.png)
  
  
 2. 질적예측방법(주관적 견해를 사용하여 예측)
 - 과거의 정보가 없거나 불충분한 경우
 
 ### 시계열 자료분석 순서
1. 시계열 자료 구조파악
2. 시계열 자료의 구조와 특성을 토대로 미래의 값 예측   
cf)  ARIMA 모형은 정상성 데이터로만 미래의 값 예측 가능   
- 정상성의 기준 ?
  - 모든 시점에 대해 일정한 평균을 가짐
  - 평균이 일정하지 않고 분산도 시점에 의존하지 않음
  - 공분산도 단지 시차에만 의존할 뿐 실제 특정 시점 t,s에 의존하지 않음   
    -> 목적: 시계열이 갖고 있는 법칙성을 발견하여 이를 모형화하고 추정된 모형을 통해 미래 예측
    
 ### 시계열 데이터 평가 방법
1. 데이터를 관측가능기간과 예측기간으로 구분
- 관측가능기간의 데이터를 사전평가, 예측기간의 데이터를 사후평가로 구분   
(미래의 데이터는 구할 수 없으므로 사후평가데이터로 가정)
2. 사전평가에서 모형을 추정하고 사후평가에서 추정된 모형으로 예측   
  cf) 시계열 데이터는 시간을 갖고 있기 때문에 순서가 바뀌면 안됨 -> 샘플링 X

### 모형을 평가하는 척도
- MAE(평균절대오차), MSE(평균제곱오차), RMSE(평균제곱근오차), MAPE(평균절대백분비오차) 등







