# swin_unet
将SWIN Transformer结构引入Unet网络中，以腹部多器官分割作为案例进行测试。

具体为：每个CNN特征层直接输入该层的SWin Transformer，
即每层的SWin Transformer都有2个输入——该层的CNN特征层 + 上一层的Swin Transformer输出，
而该层SWin Transformer的输出也有2个去向——对应Decoder层 + 下一层的SWin Transformer输入。



