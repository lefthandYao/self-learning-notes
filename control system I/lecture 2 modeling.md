objectives
	探讨为什么要引入控制系统
	介绍几种不同的控制架构
	如何建立物理系统的数学模型
	用四个矩阵表示线性时不变系统
	探讨非线性系统的近似（非平衡点的概念）

为什么要引入控制系统
	stabilization
		make sure the system does not blow up
	regulation
		maintain operating in spite of disturbance
	tracking
		follow the reference trajectory that changes over time

Basic control architectures: Feed-Forward(前馈控制)
	![image.png](https://fastly.jsdelivr.net/gh/lefthandYao/my-image-bed@main/pc/20260718103727125.png)
	P plant 被控对象： 一般是实际的物理对象，例如需要被控制的机械臂或电阻丝（产热），或电机
	attempt to compute what should be the control input u that would make y=r;
	目的在于找到F使得输入什么，受控系统就能输出什么或者保持什么
	Essentially, F should be an inverse of P
	**we have to model P properly**, the outcome sensitive to modeling errors
	we cannot alter the dynamics of P, **cannot make unstable system stable.**

Basic control architectures: Feedback(反馈控制)
	![image.png](https://fastly.jsdelivr.net/gh/lefthandYao/my-image-bed@main/pc/20260718104409754.png)
	given error: y-r, and we want to design C that can make the y closer to r
	![image.png](https://fastly.jsdelivr.net/gh/lefthandYao/my-image-bed@main/pc/20260718105103112.png)
	我们通过传感器来得到误差（其实是直接得到y）
	在循环稳定的前提下，我们希望C的增益尽可能大
	**does not require a precise knowledge of P** - robust to modeling errors
	**can stablize unstable systems**, but can also make stable systems unstable
	we need error to develop in oder to figure out apporpriate control
	u 需要被计算出来（不过应该是通过系统C得到的）

Basic control architectures: two degrees of freedom
	![image.png](https://fastly.jsdelivr.net/gh/lefthandYao/my-image-bed@main/pc/20260718105741844.png)
	我们经常忽略反馈调节

System State(只有动态系统有系统状态的概念)
	系统过去所有的可以用于预测未来输出结结果的信息
		系统参数：水箱的横截面积，水管的粗细
		系统状态：水箱过去的加水量，水位

Dimension of a system
	状态维度：最少需要几个独立状态变量，就能完整记录系统全部“历史记忆”
	对于静态系统：0维度
	动态系统：看有几个需要被调控的变量

LTI State-space model
	four matrix to represent 
	![image.png](https://fastly.jsdelivr.net/gh/lefthandYao/my-image-bed@main/pc/20260718111502279.png)
	x(t) : 状态向量（储存系统的全部记忆，可能包含速度，水位高度，电压，电流等等表示状态的量）（状态向量的维数就是系统维数）
	u(t) : 外部输入
	y(t) : 系统输出（我们要观测的量）
	方程1：储存系统的变化由外部输入和所有过去已知的状态决定
	方程2： 输出由储存系统和外部输入决定
	所有高阶导数都可以用这四个矩阵表示
	假设n维系统
		A : n * n
		B : n * 1
		C : 1 * n
		D : 1 * 1
	**我们需要自己找到如何定义x（t）**
	ABC是随我们选定不同的状态变量决定的

Nonlinear 
	现实中大部分系统都是非线性的
	构建LTI近似系统
	这种近似方法只针对大直流信号+微小扰动（交流）
	我们需要找到平衡点
	![image.png](https://fastly.jsdelivr.net/gh/lefthandYao/my-image-bed@main/pc/20260718114822543.png)
	 