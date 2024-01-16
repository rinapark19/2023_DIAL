2023 DIAL Lab Intern Project 1: Transformer Translator
==================================================

1. 프로젝트 목적
- Transformer 모델 이해 및 구현
- BART 모델 이해 및 파인 튜닝
- 기계번역 태스크 수행

2. 파일 설명
- [KoBART_translator.ipynb](https://github.com/rinapark19/2023_DIAL/blob/main/Project1/KoBART_translator.ipynb)
: BART 모델 파인 튜닝 코드

- [dataset.py](https://github.com/rinapark19/2023_DIAL/blob/main/Project1/dataset.py)
: transformer dataset 구축 코드

- [train_model.py](https://github.com/rinapark19/2023_DIAL/blob/main/Project1/train_model.py)
: transformer 모델 학습 코드

- [transformer.py](https://github.com/rinapark19/2023_DIAL/blob/main/Project1/transformer.py)
: transformer 모델 구축 코드

- [translation.py](https://github.com/rinapark19/2023_DIAL/blob/main/Project1/translation.py)
: transformer 번역 수행 코드

- [util.py](https://github.com/rinapark19/2023_DIAL/blob/main/Project1/util.py)
: transformer 데이터 구축 및 학습에 필요한 함수들

3. 결과
# transformer 한영 번역
- Head_num = 8 / N = 6 / epoch = 50 / batch_size = 4 / dataset  = 80,000
- 예시 번역: 안녕하세요, 출장은 잘 다녀오셨나요? -> Hello, did you went well?
- BLEU score: 0.35

# transformer 제주도 방언 번역
- head_num = 8 / N = 6 / epoch = 50 / batch_size = 4 / dataset  = 30,000
- 예시 번역: 뭐가 맞는 건지 잘 모르겐. -> 잘 모르겠어. 잘 모르겠어.
- BLEU score: 0.38

# KoBART fine tuning 한영 번역
- batch_size = 4 / learning_rate = 3e-4 / epoch = 10 / dataset = 80,000
- 예시 번역: 너희 아빠랑 이번 주말에 보러 다녀와야겠네 그럼 -> I'll go watch it with your d
- BLEU score: 0.35

# KoBART + random encoder 한영 번역
- batch_size = 2 / learning_rate = 3e-5 / epoch = 10 / dataset = 30,000
- 예시 번역: 너희 아빠랑 이번 주말에 보러 다녀와야겠네 그럼 -> Then I will go on the store, and
- BLEU score: 0.22