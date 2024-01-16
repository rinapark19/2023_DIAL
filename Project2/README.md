2023 DIAL Lab Intern Project 2: CarotidAS
==================================================

1. 프로젝트 목적
- 국내 무증상 성인에서 경동맥의 동맥경화증의 예측을 위한 기계학습모델의 개발에 대한 연구
- Decision Tree, Logistic Regression, Random Forest, Xgboost, SVM, Adaboost, Naive Bayes, KNN 성능 비교

2. 파일 설명
- [SVM.ipynb](https://github.com/rinapark19/CarotidAS_models/blob/main/SVM.ipynb)
: SVM 기반 분류

- [XGboost.ipnyb](https://github.com/rinapark19/CarotidAS_models/blob/main/XGboost.ipynb)
: XGboost 기반 분류

- [random_forest.ipnyb](https://github.com/rinapark19/CarotidAS_models/blob/main/random_forest.ipynb)
: random forest 기반 분류

3. 결과
# Random forest feture group 1
- Accuracy: 0.7389
- Precision: 0.6899
- Recall: 0.4862
- F1-score: 0.5704

# Random forest feature group 2
- Accuracy: 0.7263
- Precision: 0.6335
- Recall: 0.5512
- F1-score: 0.5895

# XGboost feature group 1
- Accuracy: 0.7326
- Precision: 0.6730
- Recall: 0.4862
- F1-score: 0.5646

# XGboost feature group 2
- Accuracy: 0.7467
- Precision: 0.6971
- Recall: 0.5118
- F1-score: 0.5902

# SVM featrue group 1
- Accuracy: 0.7059
- Precision: 0.6369
- Recall: 0.5034
- F1-score: 0.5623

# SVM feature group 2
- Accuracy: 0.6684
- Precision: 0.8135
- Recall: 0.5530
- F1-score: 0.6584