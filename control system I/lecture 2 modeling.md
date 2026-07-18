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
	we have to model P properly, the outcome sensitive to modeling errors
	we cannot alter the dynamics of P, cannot make unstable system stable.

Basic control architectures: Feedback(反馈控制)
	![image.png](https://fastly.jsdelivr.net/gh/lefthandYao/my-image-bed@main/pc/20260718104409754.png)
	given error: y-r, and we want to design C that can make the y closer to r