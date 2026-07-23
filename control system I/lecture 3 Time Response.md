objectives
	1. general form response of a linear system by adding its initial condition response and its forced response
	2. matrix exponential
	3. use matrix exponential to compute the response
	4. understand several definititions of stability for a dynamical system
	5. check whether a LTI system is stable or not by inspection of A

system example
![image.png](https://fastly.jsdelivr.net/gh/lefthandYao/my-image-bed@main/pc/20260723171538416.png)
线性方程的通解： x(t) = initial condition response(零输入相应) + forced response(零状态相应)
	initial response
		代表系统的初始状态x(t0)，与外部输入u无关
	forced response
		系统没有储能的情况下，纯粹由外部输入u产生的运动
state transition function(微分方程的解)