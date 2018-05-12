# FasterRcnn_Keras
bulid a simple faster rcnn model for VOC2007 base on Keras

This work aims to understand Faster RCNN architecture described by http://arxiv.org/pdf/1506.01497.pdf

Keras is a high-level deeplearning networks platform, it's easy to build a complex module such as Faster RCNN,
which is highly helpful for architecture understanding.

Comparing with the orignal work, some charges are made for GPU-Mem-Limit or computing speed:
1. a resize module is used instead of a roipooling layer
2. fully connected layer reduce from 4096 to 2048
3. a batchsize of 32 intead of 128 is feed after rpn layer

My softerware Env:
Ubuntu 16.04 + tensorflow-gpu 1.4 + cuda 8.0 + CuDNN for cuda8.0

My hardware Env:
GTX1060 6G

A jupyter-notebook based file is available for single step debug

some of the results:


![exp0](https://github.com/superlich7/FasterRcnn_Keras/blob/master/result_imgs/example0.jpg)

![exp1](https://github.com/superlich7/FasterRcnn_Keras/blob/master/result_imgs/example1.jpg)

![exp2](https://github.com/superlich7/FasterRcnn_Keras/blob/master/result_imgs/example2.jpg)

This work is mainly build base on https://github.com/yhenon/keras-frcnn
