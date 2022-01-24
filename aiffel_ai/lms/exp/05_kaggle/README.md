# 목차
- [들어가며](#들어가며)
- [정보 탐색](#정보-탐색)
- [baseline](#baseline)
- [update](#update)
- [project](#project)
---
# 들어가며
## 학습 목표
- kaggle 참가
- 데이터 다운 및 로컬에서 데이터 다루기
- 앙상블 기법 & 최종 결과 제출
- 하이퍼 파라미터 튜닝 기법
- 튜닝 기법을 통해 성능 올리기
## 학습 전제
- 정형 데이터 활용한 EDA와 분류, 회귀 문제 해결 경험
- numpy, pandas, matplotlib등의 라이브러리 사용 가능
- 정형 데이터를 활용한 다양한 학습 모델 구축 및 예측 결과 도출 경험
## 준비물
- 라이브러리
> - xgboost, lightgbm
> - missingno 
---
# 정보 탐색
## 캐글(Kaggle)이란?
- 데이터 사이언티스트들을 위한 경진대회 사이트
- 다양한 데이터와 예제 코드, 대회가 존재함
## Overview 대회 전반 소개
### Description 대회 소개
- [대회 링크](https://www.kaggle.com/c/2019-2nd-ml-month-with-kakr)
- 소개, 참여 방법 등등 다양한 정보를 기재함
### Evaluation 점수 평가 기준
- 다양한 평가 지표를 기술함
- 여기서는 RMSE를 사용
    - Root Mean Squared Error
### Prize 상품
- 상품 지급 기준이 적혀있음
### Timeline 일정표
- 시작, 종료 날짜가 명시되어 있음
### Rules 규칙
- 다양한 규칙이 존재할 수 있음
> - 계정 수
> - 외부 데이터 사용 유무
> - 하루 제출 횟수
---
## Data 데이터 소개
### Data Description 데이터 설명
- 다양한 데이터 값이 있음
- 경우에 따라 범주, 수치 등으로 변경이 가능할 것으로 예상됨
### Data Explorer 데이터 파일
- 데이터가 train, test, sample_submission
---
# baseline
- [baseline_code](https://www.kaggle.com/kcs93023/2019-ml-month-2nd-baseline)
- 이후 내용은 [code를 참고](./baseline.ipynb)
---
# update
- 관련 내용은 [code를 참고](./test.ipynb)
---
# project