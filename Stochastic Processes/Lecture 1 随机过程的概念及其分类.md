概率论：单个随机变量的特性
随机过程：多个随机变量，关注多个随机变量之间的关联关系
	两种主要的关联方式
		Linear Corelation（线性相关）
			Time domain
			Frequency domain
			Gaussian
		Markov Property（马尔可夫性）
			Discrete time
			Continuous time
			Poisson
		Martingala（鞅）
			modern fiance principle

textbook:
	随机过程及其应用习题解答 (陆大䋮, 张颢) 
ref：
	概率、随机变量与随机过程 （Probability, Random Variables and Stochastic Processes） (美）帕普里斯

Linear Corelation
	Joint Distribution （定性理解）
		不相关：y的均值不随x变化
		独立：y的分布也不能随x变化
		如果固定住一个随机变量，另一个的分布不变->独立
		![image.png](https://fastly.jsdelivr.net/gh/lefthandYao/my-image-bed@main/pc/20260904092439924.png)
		圆：y的均值随x不变，不相关
		纺锤：宽度减小，相关度增大
		![image.png](https://fastly.jsdelivr.net/gh/lefthandYao/my-image-bed@main/pc/20260904102810293.png)
	计算相关性：
		均方距离Y~kx
		![image.png](https://fastly.jsdelivr.net/gh/lefthandYao/my-image-bed@main/pc/20260904104813108.png)
		探究随机变量之间的关联（关注交叉项）
		交叉项E(XY)满足内积的三条核心公理：
			对称性：
			![image.png|148](https://fastly.jsdelivr.net/gh/lefthandYao/my-image-bed@main/pc/20260904105549649.png)
			线性：
			![image.png](https://fastly.jsdelivr.net/gh/lefthandYao/my-image-bed@main/pc/20260904105605718.png)
			正定性：
			![image.png](https://fastly.jsdelivr.net/gh/lefthandYao/my-image-bed@main/pc/20260904105638006.png)
		E(XY) = 0 -> 正交 
		E(XY) = EX·EY -> 不相关
		如果正交的X和Y分别加一个EX，EY的偏置，二者等价，所以至少有一个均值为0的时候，二者等价