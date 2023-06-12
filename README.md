# EE5346_Group8

本项目代码结合[NetVLAD](https://github.com/Nanne/pytorch-NetVlad)的PyTorch版本以及[ToDayGAN](https://github.com/AAnoosheh/ToDayGAN)自编码器神经网络进行搭建，相关依赖库请参照NetVLAD的依赖库。

本项目所使用的数据库为[Pittsburgh 250k](https://github.com/Relja/netvlad/issues/42)，如有需要请联系NetVLAD原文作者下载。本代码可实现训练、测试、聚类三大功能，具体用法请继续参照[NetVLAD](https://github.com/Nanne/pytorch-NetVlad)。为直观地体现代码的运行效果，你可以直接以下方的命令行用我们训练好的ToDayGAN神经网络节点进行测试:
    
    python main.py --mode=test --dataset=pittsburgh --arch=todaygan --resume=runsPath/trained_todaygan_netvlad --split=test

如果使用vgg16神经网络节点进行测试，则使用该命令行：

    python main.py --mode=test --dataset=pittsburgh --arch=vgg16 --resume=runsPath/trained_vgg16_netvlad --split=test