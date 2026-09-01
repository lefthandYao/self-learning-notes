analogy: mail system
	we dont care the content in the mail, we care about the whole picture

the internet is federated
	there is no single operator

challenges
	federated
	scalable
	constantly evolving
	diverse(all users are different)
	asynchronous
		there is a physical limit(speed of light)
	internet must handle failures at scale

Protocols
	rules for how to people communicate
	syntax: format of message
	semantics: what should I do in response to messages


Layers
	physical layer: moving bits across space
		voltages on electrical wire
		light signals on optical fiber
		wireless radio waves
	local networks（link layer）: connect everyone in local town
		link between machines
		machines exchange packets
	connecting local networks（Internet layer）
		set post office
		![image.png|210](https://fastly.jsdelivr.net/gh/lefthandYao/my-image-bed@main/pc/20260901184359979.png)

Internet: Network of networks
	![image.png](https://fastly.jsdelivr.net/gh/lefthandYao/my-image-bed@main/pc/20260901184520532.png)
	圆形：End hosts
	方形：Switches（routers）

![image.png](https://fastly.jsdelivr.net/gh/lefthandYao/my-image-bed@main/pc/20260901185959432.png)
routers can communicate in different ways

layers 3 offers best-effort
	packets are limited in size
	packets could get lost reorderd, corrupted
	network wont tell if failed
	no garantee
so, 3 layers is not enough

Building layars 4-7
	realiablity(transport layer)
		re-sending lost packets
		splits up and reassembles large data
		flows(connections) instead of packets
			stop thinking about individual packages
	layer 5 and 6 are obsolete
	application layer
		design build different services

Headers
	packets needs extra metadate, to tell what to do with the packet
	contains:
		Destination address
		Source address
		payload: the actual data in the packet
	![image.png](https://fastly.jsdelivr.net/gh/lefthandYao/my-image-bed@main/pc/20260901191419114.png)
	everybody needs to agree on the format of the header

Multi-Headers
Analogy:
	first wrapped by senders(multi-layers) then unwrapped by accepters
	![image.png](https://fastly.jsdelivr.net/gh/lefthandYao/my-image-bed@main/pc/20260901192100061.png)
	each person communicates with its peers at the same layer
	a protocol at a specific layer only makes sense to people at that layer
Internet:
	![image.png](https://fastly.jsdelivr.net/gh/lefthandYao/my-image-bed@main/pc/20260901192410718.png)
	![image.png](https://fastly.jsdelivr.net/gh/lefthandYao/my-image-bed@main/pc/20260901192538399.png)

Routers
Analogy:
	post office needs routers
		firstly unwrapped the outer header
		judge whether can connect to mail room
		if not, wrapped the outer hearder to the next post office
Internet：
![image.png](https://fastly.jsdelivr.net/gh/lefthandYao/my-image-bed@main/pc/20260901193425971.png)
	routers don't support reliable delivery
	routers don't care abot application data
![image.png](https://fastly.jsdelivr.net/gh/lefthandYao/my-image-bed@main/pc/20260901193856047.png)
