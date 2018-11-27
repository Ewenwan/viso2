# viso2


        ROS Stack containing a wrapper for libviso2, a visual odometry library. 
        
        http://www.ros.org/wiki/viso2 for the list of contained packages.


        从多个二维图片中重建3D影像是机器视觉必不可少的部分，这篇论文【1】提出的就是做3D重建的工作。
        这篇论文提出了一种巧妙的实时的方法做3D地图重建——使用稀疏特征和视觉里程计相结合的方法。
        这种方法包含了立体匹配和创建点云。用这种方法计算出来的视觉里程计是当年11年最好的。
        该法可以每秒执行25f，同时建立3~4fps的深度地图，可以用于实时3d重建（这个用的是11年的处理器）

        本文的贡献在于：
        1、使用几千个特征匹配实时计算了场景流；
        2、简单但是又鲁棒的视觉里程计被提出；
        3、使用ego-motion，集合从LIBELAS的立体测量，解决了匹配连接问题。

