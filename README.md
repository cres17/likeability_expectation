# likeability_expectation

#연애 예능 프로그램 기반 호감도 예측 모델

연애 예능 프로그램의 1대1 대화 장면과 인터뷰 발화를 기반으로 참가자의 호감도 증감 변화를 정량적으로 예측하기 위한 프로젝트입니다.

---

##개요

*Pipe Line

Input Dialogue

   ↓
   
Tokenization (KoBigBird / BERT)

   ↓
   
Transformer Encoder

   ↓
   
Pooling + MLP Regression Head

   ↓
   
Soft Label Regression (MSE / Pearson)


###1. 데이터 라벨링
데이터 수집 기준
남녀 참가자가 1대1 대화 후 인터뷰에서 양측 다 상대방에 대한 호감도 증감 여부를 드러낸 경우만 데이터로 사용

