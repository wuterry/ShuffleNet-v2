This is a MXNet(gluon) implementation of ShuffleNet-v2.

reference paper: [ShuffleNet V2: Practical Guidelines for Efficient CNN Architecture Design](https://arxiv.org/abs/1807.11164)

This project mainly refer to Pytorch implementation of [ericsun99/Shufflenet-v2-Pytorch](https://github.com/ericsun99/Shufflenet-v2-Pytorch/blob/master/ShuffleNetV2.py)

---
## Testing Environment
- Python 3.6
- MXNet 1.3.0

---
## Testing Case 
setting *multiplier=0.5*, the shape of feature map are as follow:
```
feature_conv0            	(2, 24, 112, 112)
feature_batchnorm0       	(2, 24, 112, 112)
feature_relu0            	(2, 24, 112, 112)
feature_pool0            	(2, 24, 56, 56)
feature_invertedresidual0	(2, 48, 28, 28)
feature_invertedresidual1	(2, 48, 28, 28)
feature_invertedresidual2	(2, 48, 28, 28)
feature_invertedresidual3	(2, 48, 28, 28)
feature_invertedresidual4	(2, 96, 14, 14)
feature_invertedresidual5	(2, 96, 14, 14)
feature_invertedresidual6	(2, 96, 14, 14)
feature_invertedresidual7	(2, 96, 14, 14)
feature_invertedresidual8	(2, 96, 14, 14)
feature_invertedresidual9	(2, 96, 14, 14)
feature_invertedresidual10	(2, 96, 14, 14)
feature_invertedresidual11	(2, 96, 14, 14)
feature_invertedresidual12	(2, 192, 7, 7)
feature_invertedresidual13	(2, 192, 7, 7)
feature_invertedresidual14	(2, 192, 7, 7)
feature_invertedresidual15	(2, 192, 7, 7)
feature_conv55           	(2, 1024, 7, 7)
feature_batchnorm49      	(2, 1024, 7, 7)
feature_relu36           	(2, 1024, 7, 7)
feature_pool1            	(2, 1024, 1, 1)
```
