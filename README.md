# 스마트워치 센서 데이터 기반 행동 분류 프로젝트

## 📋 프로젝트 개요
스마트워치의 센서 데이터를 활용하여 6가지 인간 행동 패턴을 분류하는 머신러닝 프로젝트입니다.

## 🎯 목표
- 스마트워치 센서 데이터로부터 인간의 행동 패턴을 정확하게 분류
- 실무 적용 가능한 견고한 모델 개발
- 클래스별 성능 분석을 통한 현장 활용성 검증

## 📊 분류 대상 행동
1. **STANDING** (서기)
2. **SITTING** (앉기)
3. **LAYING** (눕기)
4. **WALKING** (걷기)
5. **WALKING_UPSTAIRS** (계단 오르기)
6. **WALKING_DOWNSTAIRS** (계단 내려가기)

## 🔧 기술 스택
- **Python**: 데이터 분석 및 머신러닝
- **Pandas**: 데이터 전처리
- **Scikit-learn**: 머신러닝 모델링
- **XGBoost**: 앙상블 모델
- **SMOTE**: 클래스 불균형 해결
- **Matplotlib/Seaborn**: 데이터 시각화

## 📈 주요 성과
- **초기 정확도**: 97.5%
- **개선 후 정확도**: 99%
- **클래스 불균형 문제 해결**: SMOTE 기법 적용
- **특성 선택**: 562개 변수 중 중요도 상위 변수 선별

## 🚀 핵심 기술
### 1. 클래스별 성능 분석
- 전체 정확도뿐만 아니라 각 행동별 성능 분석
- 현장 활용 가능성을 고려한 접근

### 2. SMOTE 기법 적용
- 클래스 불균형 문제 해결 (LAYING: 1,115개 vs 계단 내려가기: 791개)
- KNN 기반 합성 데이터 생성

### 3. 특성 선택 및 최적화
- 562개 센서 특성 중 중요도 상위 50, 100, 150개 선별
- Random Forest, XGBoost 등 다양한 알고리즘 실험

## 📁 프로젝트 구조
```
smartwatch-activity-classification/
├── README.md
├── data/                    # 데이터 파일
├── notebooks/              # Jupyter 노트북
│   ├── 01_EDA.ipynb       # 탐색적 데이터 분석
│   ├── 02_Feature_Selection.ipynb  # 특성 선택
│   ├── 03_Modeling.ipynb  # 모델링
│   └── 04_Evaluation.ipynb # 모델 평가
├── models/                 # 저장된 모델
├── results/               # 결과 파일
└── requirements.txt       # 필요한 패키지 목록
```

## 🛠️ 설치 및 실행
```bash
# 저장소 클론
git clone https://github.com/rkawr99/smartwatch-activity-classification.git

# 필요한 패키지 설치
pip install -r requirements.txt

# Jupyter 노트북 실행
jupyter notebook
```

## 📊 결과 분석
- **혼동 행렬(Confusion Matrix)** 분석을 통한 클래스별 성능 확인
- **특성 중요도** 분석으로 핵심 센서 특성 파악
- **SMOTE 적용 전후** 성능 비교

## 💡 주요 인사이트
1. **클래스 불균형**이 모델 성능에 미치는 영향
2. **특성 선택**의 중요성
3. **현장 적용 가능성**을 고려한 모델 평가의 필요성

## 🔮 향후 계획
- 실시간 분류 시스템 구축
- 다양한 스마트워치 기기에서의 검증
- 모바일 앱 연동

## 👨‍💻 개발자
**김진수** - 머신러닝 엔지니어

## 📄 라이선스
이 프로젝트는 MIT 라이선스 하에 배포됩니다. 