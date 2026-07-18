this course focus on dynamic control systems
	1. evolve over time
	2. have inputs and outputs

our main objectives:
	1. modeling
		1. use mathmatical tools to represent a daynamic control system
		2. we focus on system that can be modeled by ordinary differential equation (ODEs) -- which is LTI
		3. and we focus on single input and single output system
		4. use classical control tools (frequency domain)
	2. analysis
		1. understand the basic characterstics of a system (stability, controllabllity, obseravability)
		2. understand how the inputs effect the output
		3. analyze the response of these systems and address stability and performance of the system
	3. synthesis
		1. figure out how to design a system that we expect, and ensure it works as we expect

content:
modeling
	1. introduction, signal and system
	2. modeling, linearization
analysis
	3. time response, stability
	4. diagonalization, modal coordinates
	5. transfer functions 1: definition and properties
	6. transfer functions 2: poles and zeros
	7. analysis of feedback systems: internal stability, root locus
	8. frequency response
	9. analysis of feedback system2: the nyquist condition
synthesis
	10. specifications for feedback systems
	11. PID control
	12. Loop shaping
	13. Implementation issues
	14. Robustness


todays objective
	1. understand the control system in terms of input and output signals
	2. distinguish systems

static systems
	![image.png](https://fastly.jsdelivr.net/gh/lefthandYao/my-image-bed@main/pc/20260716175304217.png)
	the property of the system only depends on current time's input

Time invarient 
	![image.png](https://fastly.jsdelivr.net/gh/lefthandYao/my-image-bed@main/pc/20260718100040178.png)
	给一个delay后，系统特性不变

linearity
	![image.png](https://fastly.jsdelivr.net/gh/lefthandYao/my-image-bed@main/pc/20260718100128616.png)

causality
	![](https://fastly.jsdelivr.net/gh/lefthandYao/my-image-bed@main/pc/20260718100344810.png)
	如果现在得output只和过去的input有关 -> causal
	任何物理系统都是因果系统


可以通过一些手段将非线性系统用线性系统进行近似