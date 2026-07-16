操作系统的历史
1. 1950s - 1960s 操作系统概念形成
	1. 算力成为服务，operator 负责操作程序切换
2. 1960s - 1970s 集成电路、总线出现
	1. 有更快的处理器、更快、更大的内存、虚拟存储出现
	2. 可以同时载入多个程序而不用换卡
	3. 有完善的中断/异常机制
	4. 个人电脑（PC）登上历史舞台（Altair）
	5. 资源虚拟化
		1. 空分复用（MMU -> 进程）
		2. 时分复用（CPU时分复用）
3. UNIX 奠定了 pre-AI 时代计算机世界的基础
	1. 1973 信号API、管道、grep
		1. 信号API： UNIX进程间异步通信（IPC) 的软中断机制
		2. 管道：将一个进程的输出（stdout）直接连接到另一个进程的输入（stdin）
		3. grep： 文本搜索工具（global regular expression print）
	2. 1983 BSD socket
		1. UCB 的网络编程接口
	3. 1984 procfs
		1. 虚拟文件系统
		2. 一切皆文件
		3. 可以通过查看/proc下的文件来查看内核状态和进程信息
	4. UNIX 衍生
		1. 1BSD
		2. GNU
		3. MACOS
		4. AIX
			1. 服务器架构的商业UNIX操作系统
		5. MINIX
			1. 为了教学目的编写的微内核、类UNIX操作系统
		6. WINDOWS
			1. 不属于UNIX
			2. 全新的windowsNT内核
			3. 微内核，集成了
		7. LINUX
		8. IOS
		9. ANDROID
	

操作系统分为
	1. userspace
		1. vi (visual editor)
		2. cc (C compilor)
		3. shell
	2. kernal
		1. file system (provide API)
			1. 管理和组织存储设备上的数据
		2. process managing
		3. memory allocation
		4. access control