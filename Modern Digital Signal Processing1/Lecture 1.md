prerequisite：
	calculus
	algebra
	probability
	complex variables

textbook：
	S.M.Kay Fundamental of Statistical Signal Processing 
	S.Haykin Adaptive Filter Theory 5th Edition
	P.Stoica Spectral Analysis of Signal

理念：
	no reading, no learning
	no writing, no reading
	no data, no truth
		数据都是上帝给的，模型是人造的（尽量不要做仿真）
	no analytic, no understanding
	no programming, no cognition

scope：
	与本科最大不同
		加入了统计，对象为随机信号
	Unit 1: Linear Processing
		Fundamental
			Statistical Fundation
			Orthogonal
			Orthogonalization
		Typical mothod
			Wiener
			Kalman
		Extension
			SVM
			Kernal
			Regularization
	Unit 2: Adaptive Processing
		Adaptive Filter
			optimization
			random gradient descending
		Typical
			LMS
			RLS
		Extension
			Deep Learning
	Unit 3: Spectral Processing 
		recognize power spectral of the signal
			direct(non-parametric)
			filter banks

differences between mdsp1 and mdsp2
	1: 1950's-1980's
		linear
		orthogonal
		stationary
		Gaussian
	2: 1980's-Now
		Non-linear
		Non-orthogonal
		Non-stationary
		Non-Gaussian

Review of Probability Theory
	Uncertainty -> statistical experiment ->sample point
	->sample space -> possibility（可能性）
		知识的局限性，带来不确定性
		不确定是一种对自己无知的妥协
		所有可能出现的结果构成了sample space
		possibility是对每一个sample point而言的
		probability是对sample space里面的子集而言的
	概率与统计
		是两门完全不同的学科，只有符号语言有相同的部分
		概率是从模型到决策
		统计是从数据到模型
		大数据是从数据直接到决策
		![image.png](https://fastly.jsdelivr.net/gh/lefthandYao/my-image-bed@main/pc/20260901155131821.png)


样本空间很重要（随机到底怎么随机）Bertrand Paradox

随机变量的概念
![image.png](https://fastly.jsdelivr.net/gh/lefthandYao/my-image-bed@main/pc/20260901155147441.png)

随机变量是一个函数：从样本空间到实数轴
	目的是量化样本空间
随机变量没有不确定性，所有不确定性都只停留在样本点出现与否

discrete random variables：
![image.png](https://fastly.jsdelivr.net/gh/lefthandYao/my-image-bed@main/pc/20260901160056371.png)
	![image.png](https://fastly.jsdelivr.net/gh/lefthandYao/my-image-bed@main/pc/20260901155316209.png)
	随机变量满足...分布，以下这些经典分布，能体现自然界中的广泛规律

离散型概率分布：
伯努利分布：
	![image.png](https://fastly.jsdelivr.net/gh/lefthandYao/my-image-bed@main/pc/20260901155719272.png)
	![image.png](https://fastly.jsdelivr.net/gh/lefthandYao/my-image-bed@main/pc/20260901155641885.png)
	二项分布：
	![image.png](https://fastly.jsdelivr.net/gh/lefthandYao/my-image-bed@main/pc/20260901160204238.png)
	![image.png](https://fastly.jsdelivr.net/gh/lefthandYao/my-image-bed@main/pc/20260901160222969.png)
	泊松分布：
	![image.png](https://fastly.jsdelivr.net/gh/lefthandYao/my-image-bed@main/pc/20260901160552428.png)
	![image.png](https://fastly.jsdelivr.net/gh/lefthandYao/my-image-bed@main/pc/20260901160605205.png)


continue random variables：
![image.png](https://fastly.jsdelivr.net/gh/lefthandYao/my-image-bed@main/pc/20260901160127035.png)
概率密度
	![image.png](https://fastly.jsdelivr.net/gh/lefthandYao/my-image-bed@main/pc/20260901155337545.png)

