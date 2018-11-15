# DiyProtocol

### 背景

由于tcp是流协议, 数据传输像流水一样没有边界, 无法分辨一次数据的读取是一个包还是多个，或者是不足一个, 这样就需要我们在应用层,
自己来区分.

![tcp字节流](https://i.loli.net/2018/11/15/5bed7f16bfa3c.png)

一般有三种常见的方式
1. 定长包
2. 定长的包头 + 变长的包体, 包头中写入包体的长度


本文介绍方式2

### 代码

go get github.com/weiwenwang/DiyProtocol

本人附上一个demo, 里面代码注释详细.
