进入容器
```bash
	docker start -ai ubuntu
	cd xv6‑labs‑2021
	make qemu
```

退出docker：
```bash
	# 退出docker
	exit
	# 重新进入docker
	docker start ubuntu
	docker exec -it ubuntu /bin/bash
```
