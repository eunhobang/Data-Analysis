# 와인 품질 등급 예측하기

1. 목표 
-  와인 속성을 분석하여 등급 예측
2. 핵심 개념
- 기술 통계, 회귀 분석, t-검정, 히스토그램
3. 데이터 수집
- 레드/화이트 와인 데이터셋: 캘리포니어 어바인 대학읜 머신러닝 저장소에서 다운로드
- https://archive.ics.uci.edu/ml/machine-learning-databases/wine-quality/
4. 데이터 준비
- 수집한 데이터 파일 병합
5. 데이터 탐색
    - 정보확인: info()
    - 기술 통계 확인: describe(), unique(), value_counts()
6. 데이터 모델링
    - 데이터를 두 그룹으로 비교 분석
        - 그룹별 기술 통계 분석: describe()
        - t-검정: scipy 패키지의 ttest_ind()
        - 회귀 분석: statsmodels.formula.api 패키지의 ols()
    - 품질 등급 예측
        - 샘플을 독립변수(x)로 지정 ->
        - 회귀분석 모델에 적용 ->
        - 종속 변수(y)인 품질(quality) 예측