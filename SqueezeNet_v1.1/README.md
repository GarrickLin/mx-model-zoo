SqueezeNet Mxnet Implementation
===============================
This is the Keras implementation of SqueezeNet using functional API (arXiv [1602.07360](https://arxiv.org/pdf/1602.07360.pdf)). SqueezeNet is a small model of AlexNet-level accuracy with 50x fewer parameters and <0.5MB model size. The original model was implemented in [caffe](https://github.com/DeepScale/SqueezeNet).  

**What's new in SqueezeNet v1.1?**

|                 | SqueezeNet v1.0                  | SqueezeNet v1.1                  |
| :------------- |:-------------:| :-----:|
| conv1:          | 96 filters of resolution 7x7     | 64 filters of resolution 3x3     |
| pooling layers: | pool_{1,4,8}                     | pool_{1,3,5}                     |
| computation     | 1.72 GFLOPS/image                | 0.72 GFLOPS/image: *2.4x less computation* |
| ImageNet accuracy        | >= 80.3% top-5                   | >= 80.3% top-5                   |    


SqueezeNet v1.1 has 2.4x less computation than v1.0, without sacrificing accuracy. 
