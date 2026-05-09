# 🌿 고객 구매 특성을 반영한 맞춤형 판매전략 수립으로 수익성 향상


## 📌 프로젝트 개요

B2C 구조 기반 **친환경 이커머스 플랫폼**의 매출 하락 문제를 해결하기 위해,  
고객 구매 데이터를 분석하여 **맞춤형 판매 전략**을 수립한 빅데이터 분석 프로젝트입니다.

- 글로벌 이커머스 시장은 지속 성장 중이나, 경쟁 심화로 당사 매출 **-30% 급락**
- 경쟁사 대비 낮은 구독률(14% vs 26%), 20대 이하 고객 비중 저조(12% vs 38%)
- 데이터 기반의 차별화된 판매 전략 필요



## 🎯 과제 수행 목표 (KPI)

| 측정지표 | 가중치 | 목표수준 |
|---|---|---|
| 월 고객 이탈율 | 30% | 15% 이하 |
| 월간 신규 유입율 | 30% | 2% 이상 |
| 고객 1인당 평균 결제 금액 | 40% | 5만원 이상 |



## 🔍 분석 내용

### 1. 전체 변수 분포 확인
- 연령대별·지역별·성별·구독 여부 등 데이터 전반 탐색
- Pie Chart, Histogram, Bar Chart, Chi-square Test 활용

### 2. VIP 선정을 위한 고객 세분화 (RFM 분석)
- RFM Score = 0.2·R + 0.4·F + 0.4·M
- 상위 50% 고객이 전체 매출의 **90%** 차지
- Random Forest 모델로 VIP 전환 예측 (Accuracy 0.96, F1-Score 0.78)

### 3. 고객 이탈 분석
- 휴면고객 비율 20.3% → 잠재 이탈군으로 간주
- 1회 구매 고객의 휴면 전환율이 가장 높음 (56%)
- 고가 품목 구매 후 휴면 전환율 89%로 품질 관리 필요
- Random Forest 이탈 예측 모델 (Accuracy 0.98)

### 4. 요일·연령대별 구매 특성 분석
- 연령대별 선호 품목이 요일에 따라 상이함
- 개인 맞춤형 프로모션 전략 수립에 활용

### 5. 연관규칙 분석 (Association Rule)
- 연령대별 함께 구매되는 상품 조합 도출
- 40대: 중파·당근·양파 구매 시 콩나물 추천 등

### 6. 배송 지연 분석
- 신선식품 배송 지연율(2.25%)이 일반식품(1.89%)보다 높음
- 경상도 지역 지연율 가장 높음 (0.27%)
- 보리살림돼지(20.16%), 무항생제닭(19.69%) 지연율 개선 필요

### 7. 구매 취소 분석
- 고가 제품 취소율(4.93%)이 타 가격대 대비 높음
- 흑염소진액(8.25%), 한우국거리(5.50%) 품질 관리 필요

### 8. 수요 예측 (ARIMA)
- 변동성 높은 상품의 재고 부족 방지를 위해 ARIMA 모델 적용
- 공급사 선제적 재고 확보 및 입고 스케줄 최적화

### 9. 친환경 제품 분석
- 고객 친환경 제품 지불 의사 67%로 높으나, 친환경 상품 비중 18%로 낮음
- 인기 일반 상품의 친환경 라인업 확대 필요



## 💡 개선안

| 개선 영역 | 개선안 |
|---|---|
| 고객 등급 관리 | VIP~Family 5단계 등급별 차별화 혜택 제공 |
| 이탈 방지 | 휴면고객 로그인 시 재구매 유도 쿠폰 자동 지급 |
| 개인화 추천 | 연령대·요일별 선호도 기반 맞춤 추천 시스템 |
| 구독 서비스 강화 | 잘 팔리는 식재료 꾸러미 제공 + 친환경 제품 할인쿠폰·적립률 제공 |
| 친환경 확대 | 인기 일반 상품 기반 PB 친환경 제품 도입 + 마이 에코 리포트 시스템 |
| 공급사 관리 | 공급사 평가 시스템(Platinum~Red) + 전용 앱으로 수요 예측 정보 제공 |

---

## 🛠 사용 기술

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=flat&logo=scikit-learn&logoColor=white)

- **분석**: Pandas, NumPy, SciPy
- **시각화**: Matplotlib, Seaborn
- **머신러닝**: Scikit-learn (Logistic Regression, Decision Tree, Random Forest, XGBoost)
- **시계열**: Statsmodels (ARIMA)
- **통계 검정**: Chi-square Test



## 👥 팀원

| 이름 | 역할 |
|---|---|
| 김세희 | 데이터 전처리, 연관규칙 분석 |
| 송노건 | RFM 분석, 이탈 위험 고객 예측 모델|
| 양호준 | 팀장, 시연 앱 개발 |
| 이소현 | ARIMA 분석, PPT |
| 이호원 | 카이제곱 검정, PPT |

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/7f3a0345-17a0-4582-94e9-4e87f28fba95" />
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/d7976901-c857-4a67-b671-4c99c6cf8e6f" />
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/fad8929f-5ec6-48e9-b937-4c147a2c97fc" />
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/00e8f338-de4d-47d4-9947-a697814ba40f" />
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/b0172720-bf29-433e-9f45-1de7936273e2" />
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/4f83c8dd-8618-4d83-adf2-270fdb7500c1" />
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/30f3513e-2dd9-461e-a7e6-5f0e49e3ee39" />
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/24bac530-d3d0-4f40-a9a9-db7c8b5ed909" />
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/072f9893-c381-4216-b989-5661dd2016a3" />
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/f9a75563-3734-4195-99cf-0496e07847c4" />
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/c9dca4fa-2e61-49b3-b736-682b6c8ea1e2" />
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/d88c5b9c-9cc0-40e1-96c7-251a05eda953" />
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/e1e5dacd-095f-464d-8b36-43ccbdde12bc" />
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/db10f022-ff4b-42c3-bde1-5ad0bbd25923" />
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/9dfb3e5e-5761-47d7-a0fa-374dc8f9dcb9" />
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/e40d0378-7920-4733-88dd-c55bf3e66296" />
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/e3ea973d-0394-493b-ba66-25a97f37b621" />
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/ef420130-635b-4041-8adb-3d818658484c" />
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/0dbb136d-7341-4a33-b7af-8f46422ba9c0" />
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/fdb8e127-c5ab-4823-8bd0-28be2b58021c" />
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/4c03c2f0-d2f5-48fd-a61d-22a2608a9b4b" />
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/eb59d86c-545f-44b9-914a-07157dfd1869" />
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/cfa68b1b-ad62-4313-bb8f-c67fd30b6c75" />
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/f59b9cae-60b0-4675-b87a-771cb5e69a34" />
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/6ea1a31b-f86f-4378-8f35-59f4bc4bd3d8" />
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/0c00cf5c-db31-4241-9cb8-02fa01ff8627" />
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/9f1f8a9c-93f0-4817-b454-ffd403b8a610" />
