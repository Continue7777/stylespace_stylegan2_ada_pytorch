# stylespace_stylegan2_ada_pytorch

实现方案：
+ forawrd_hook改变style。
+ backward_hook计算雅可比矩阵获取梯度图。

小结论：
+ 单通道确实可以改变指定区域或者特征。（对于发型的修改限于局部）
+ w+空间需要自己重新找通道，也可以实现相应效果，大概率是因为重建的空间不一致造成。
