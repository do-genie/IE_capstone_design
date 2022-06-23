# IE_capstone_design
 
## 리셀 가격 예측 모델
- 해당 프로젝트에서 리셀 가능 여부, 리셀 가격 예측 중에서 리셀 가격 예측 파트를 맡아 진행
이미 출시되어 시장에서 거래되고 있는 제품의 시계열 데이터를 사용한 리셀 가격 예측 모델

- 사용 데이터 : 일별 "거래가, 포털검색량, 소비자물가지수, 나이키 주가"

### 파일 
- 해당 파일은 리셀 가격 예측 파트만을 담고있다. 
- human_data_mining.xlsx : 파일 안에서 나이키X사카이 LD와플 블루멀티, 조던1레트로하이OG블랙모카 sheet만을 사용해 진행하였다. 
- adaboost_tuning, gru_tuning, lstm_tuning : 각각 세가지 모델의 하이퍼파라미터 조정을 위해 사용한 코드
- adaboost_tuning : 변수 조합 확인을 위해서도 사용되었다. 
- 최종 보고서, 발표 파일 
### 수행 단계
1. KREAM 플랫폼의 2가지 상품의 거래가, 데이터 수집 및 전처리
2. 포털 검색량, 소비자 물가 지수, 나이키 주가 데이터 수집 및 전처리
3. 단일 변량 딥러닝 모델을 사용해 예측력 뛰어난 모델 결정
4. 다변량 딥러닝 모델을 사용해 단일변량보다 성능 좋은 변수 조합 선택
5. 최적의 딥러닝 모델과 구현 및 변수 확정

##### 사용한 모델 종류
- LSTM
- GRU 
- AdaBoost-GRU 앙상블 모델

해당 주피터노트북 파일은 모델의 파라미터를 조정하고, 입력 변수를 조정하며 성능을 파악했을 때 사용한 코드이다. 