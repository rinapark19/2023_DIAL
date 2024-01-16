2023 DIAL Lab Intern Project 3: BM25, DPR를 이용한 문서 검색
==================================================

1. 프로젝트 목적
- 정책지원AI프로젝트 사전 학습
- Text Ranking과 그에 사용되는 모델(BM25, DPR) 학습 및 구현
- 각 모델에서의 성능 비교

2. 파일 설명
- [BM25.ipynb](https://github.com/rinapark19/Text_ranking/blob/main/BM25_new.ipynb)
: BM25를 이용한 문서 검색

- [DPR.ipynb](https://github.com/rinapark19/Text_ranking/blob/main/DPR_new.ipynb)
: DPR를 이용한 문서 검색

3. 결과
# BM25 실험 결과
- B: 0.75, K1: 1.4
- Recall@1: 0.5451
- Recall@10: 0.7841
- Recall@20: 0.8196
- Recall@100: 0.8777

# DPR 실험 결과
- batch_size = 2 / epoch = 10 / learning_rate = 1e-5 / dataset = 50,000
- Recall@1: 0.1
- Recall@10: 0.33
- Recall@20: 0.419
- Recall@100: 0.623