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
		possibility是先验的，对每一个sample point而言的
		probability是对sample space里面的子集而言的
	