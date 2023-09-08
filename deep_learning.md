# mixed precision training
## [mixed precision training](https://openreview.net/pdf?id=r1gs9JgRZ)
使用FP16训练神经网络，3种手段减小模型精度损失：
- 维护一份FP32权重拷贝
<img width="363" alt="image" src="https://github.com/zhangjun/paper-reading/assets/1312389/1ccfefc7-b0fe-4d91-86c7-dde62d0f8d1c">

- 损失缩放（loss-scaling）尽可能避免梯度值变为0
- FP16计算使用FP32进行累加
