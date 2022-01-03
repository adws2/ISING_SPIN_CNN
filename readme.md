# Ising spin CNN

## 데이터
X : 이징 스핀 이미지 (batch X 64 X 64 X 1) - Single channel

Y : 0 or 1 (phase)

## CNN
초기 모델 : conv layer + fully connected layer : 8.5M param

현재 모델 : depthwise separable conv layer + fully connected layer (iterative pruning) : 1.1M

## Result
computing time : 12m 16s (colab gpu)

cross entropy loss : 0.0577

Accuracy : 0.9747

f1 score : 0.9751
