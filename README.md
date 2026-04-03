# Korean TTS — VITS

> End-to-end 한국어 Text-to-Speech 모델 학습

<br>

[VITS](https://arxiv.org/abs/2106.06103)(Variational Inference with adversarial learning for end-to-end Text-to-Speech)를 한국어 단일 화자 데이터셋인 KSS(Korean Single Speaker)로 학습한 TTS 모델입니다.

## 📊 Dataset


| 항목 | 내용 |
|------|------|
| 데이터셋 | KSS (Korean Single Speaker Speech) |
| 화자 수 | 1명 (여성) |
| 총 발화 수 | 12,853문장 |
| 총 길이 | 약 12시간 |
| 샘플링 레이트 | 44,100 Hz |


 
## 📉 Training Loss
 
![Training Loss](assets/training_curves.png)

| 항목 | 내용 |
|------|------|
| GPU | NVIDIA RTX 4090 |
| 학습 스텝 | 200,000 steps |
| Batch size | 64 |

## Training Exmaple

```sh
# KSS
python train.py -c configs/kss_base.json -m kss_base
```

## Inference Exmaple
[inference.ipynb](./inference.ipynb)


## References
* [VITS 공식 레포지토리](https://github.com/jaywalnut310/vits)
* [KSS 데이터셋 다운로드](https://www.kaggle.com/datasets/bryanpark/korean-single-speaker-speech-dataset)
* [논문: Variational Inference with adversarial learning for end-to-end Text-to-Speech](https://arxiv.org/abs/2106.06103)# Korean-vits
# Korean-vits
