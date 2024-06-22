任务1：
对比监督学习和自监督学习在图像分类任务上的性能表现

基本要求：
(1) 实现任一自监督学习算法并使用该算法在自选的数据集上训练ResNet-18，随后在CIFAR-100数据集中使用Linear Classification Protocol对其性能进行评测；
(2) 将上述结果与在ImageNet数据集上采用监督学习训练得到的表征在相同的协议下进行对比，并比较二者相对于在CIFAR-100数据集上从零开始以监督学习方式进行训练所带来的提升；
(3) 尝试不同的超参数组合，探索自监督预训练数据集规模对性能的影响；

任务2：
在CIFAR-100数据集上比较基于Transformer和CNN的图像分类模型

基本要求：
（1） 分别基于CNN和Transformer架构实现具有相近参数量的图像分类网络；
（2） 在CIFAR-100数据集上采用相同的训练策略对二者进行训练，其中数据增强策略中应包含CutMix；
（3） 尝试不同的超参数组合，尽可能提升各架构在CIFAR-100上的性能以进行合理的比较。

任务3：
基于NeRF的物体重建和新视图合成
基本要求：
（1） 选取身边的物体拍摄多角度图片/视频，并使用COLMAP估计相机参数，随后使用现成的框架进行训练；
（2） 基于训练好的NeRF渲染环绕物体的视频，并在预留的测试图片上评价定量结果。