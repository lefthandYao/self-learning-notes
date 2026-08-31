objectives
	1. general form response of a linear system by adding its initial condition response and its forced response
	2. matrix exponential
	3. use matrix exponential to compute the response
	4. understand several definititions of stability for a dynamical system
	5. check whether a LTI system is stable or not by inspection of A

system example
![image.png](https://fastly.jsdelivr.net/gh/lefthandYao/my-image-bed@main/pc/20260723171538416.png)
利用系统的linearity，把U拆解成Upast和Ufuture
![image.png|312](https://fastly.jsdelivr.net/gh/lefthandYao/my-image-bed@main/pc/20260831085713028.png)
线性方程的通解： x(t) = initial condition response(零输入相应) + forced response(零状态相应)
	initial response（homogeneous response)
		代表系统的初始状态x(t0)，与外部输入u无关
		Upast累积决定了initial response
		![image.png](https://fastly.jsdelivr.net/gh/lefthandYao/my-image-bed@main/pc/20260831090048298.png)
		u(t)=0, x(t0)=x0的条件下解出的x(t)就是initial response
	forced response
		系统没有储能的情况下，纯粹由外部输入u产生的运动
		Ufuture决定了forced response
		![image.png](https://fastly.jsdelivr.net/gh/lefthandYao/my-image-bed@main/pc/20260831090103188.png)
		假设x(t0) = 0求解出的x(t)就是forced response
state transition function、
x(t)是initial response：
![image.png|435](https://fastly.jsdelivr.net/gh/lefthandYao/my-image-bed@main/pc/20260831091505856.png)
forced response是u(t)和状态转移函数做卷积
![image.png](https://fastly.jsdelivr.net/gh/lefthandYao/my-image-bed@main/pc/20260831091733429.png)
相当于信号与系统里面学过的h(t)impulse response

time constant
用于衡量