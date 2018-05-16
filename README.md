# simple_tcp_test

TCP传输测试工具

### 生成200M的文件
```
dd if=/dev/zero of=test bs=1M count=200
```

### 使用
```
./client 192.168.30.3 10000 test
```

###　开启BBR拥塞控制算法
sysctl -w net.ipv4.tcp_congestion_control=bbr
