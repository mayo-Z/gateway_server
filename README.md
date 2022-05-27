# 项目介绍

这是微服务网关服务的配套测试服务器，可用于模拟下游节点。

技术栈：go+vue2.0+element

后端项目：https://github.com/uptocorrupt/go_gateway

下游测试服务器：https://github.com/uptocorrupt/gateway_server

联系邮箱：hhd5050@foxmail.com

# 代码运行

- git clone

```
git clone https://github.com/uptocorrupt/gateway_server.git
```
- 确保本地环境安装了Go 1.12+版本
```
go version
```

- 下载类库依赖

```
go env -w GO111MODULE=on 
go env -w GOPROXY=https://goproxy.cn
cd go_gateway
go mod tidy
```
- 修改对应服务器的下游ip地址和端口
- 运行

```
go run main.go
```

