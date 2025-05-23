# Credit Transaction Fraud Detection

이 프로젝트는 신용카드 거래 데이터를 바탕으로 **사기 거래(Fraud Transaction)**를 탐지하기 위한 분석 및 머신러닝 모델링을 수행한 작업입니다.  
비정상적인 구매 패턴, 시간대, 거리, 결제 금액 등을 분석하여 **정상 거래와 사기 거래를 분류**하는 것이 주요 목표입니다.

---

## 데이터 개요

| 항목              | 설명                                                         |
|-------------------|--------------------------------------------------------------|
| 라벨 컬럼         | `isFraud` (0 = 정상 거래, 1 = 사기 거래)                     |
| 주요 특성 (Features) | - `purchase_amount`: 구매 금액<br>- `purchase_time`: 결제 시간<br>- `distance`: 고객과 매장 간 거리<br>- `category`, `gender`, `age`, `id` 등 |

---

## 주요 분석 내용

| 분석 항목             | 설명                                                                 |
|------------------------|----------------------------------------------------------------------|
| 이상치 탐지 (Z-Score)  | `purchase_amount`의 Z-score를 계산하여 이상 거래 시각화 및 탐지 수행 |
| 결제 시간 패턴 분석    | 시간대별 거래량 및 사기 비율 분석<br>새벽 시간대에 사기 비율이 높음   |
| 거리 기반 분석         | 고객과 매장 간 거리(`distance`)와 사기 여부의 관계 시각화            |

---

## 사용된 기술

- Python (pandas, numpy, matplotlib, seaborn, scipy)
- Z-Score 기반 이상치 탐지
- 데이터 시각화 및 트렌드 분석

---

## 회고

이번 프로젝트를 통해 거래 사기 탐지를 위해 단순한 수치뿐만 아니라  
**시간, 거리, 금액 등의 다양한 관점에서 데이터를 분석하는 능력의 중요성**을 느꼈습니다.  
데이터에 숨겨진 패턴을 이해하고 해석하는 경험을 통해  
**데이터 기반 사고력과 전처리 역량**을 더욱 키울 수 있었습니다.
