# BI_LSTM with RoBERTa Embedding

## Dacon competitions
- [문장 유형 분류 AI 경진대회](https://dacon.io/competitions/official/236037/overview/description)

## How to Use

- Run train.py

## Requirements

- `transformers == 4.25.1`
- `pandas == 1.3.5`
- `numpy == 1.21.6`
- `torch == 1.13.1+cu116`
- `scikit-learn == 1.0.2`
- `tqdm == 4.64.1`
- `pyperclip == 1.8.2`
- `selenium == 4.7.2`

## Metric

- weighted F1 score

## Score

- Public score : 74.78 (35/565) (with koElectra ensemble seed = 777) (it isn't public 6th solution)
- Private score : non checked

## Future works

- loss can't coverge with klue/RoBERTa-large (I think it's because of hyperparameter. it can be get higher score)

## Workers

### [노영준](https://github.com/youngjun-99)
- Seed ensemble
- CV ensemble
- Exploratory Data Analysis
- Code refactoring
- Project Managing
- Focal Loss function debug
- RoBERTaForSequenceClassification debug

### [이가은](https://github.com/gaeun5744)
- Backtranslatation function for data augmentation
- Focal Loss function (for fix data imbalance)

### [이재윤](https://github.com/pixygear)
- Add BI_LSTM layer in RoBERTaForSequenceClassification

## Citation

- [Focal Loss for Dense Object Detection](https://arxiv.org/abs/1708.02002)
- [RoBERTa: A Robustly Optimized BERT Pretraining Approach](https://arxiv.org/abs/1907.11692)
