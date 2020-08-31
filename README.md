## 背景
 `go-micro`v2.9.1,目前最新的稳定版本，依赖了`quic-go`v0.14.1,但这个版本在go1.15编译能通过但运行会panic。使用`quic-go`v0.18.0存在一些不兼容不能编译通过，基于v0.18.0做一个兼容旧api的处理。

## 使用
 `go-micro` 的最新版解除对`quic-go`依赖，但还没发行一个稳定版本，等待`go-micro`发布最新稳定版本可以不再使用此库

```shell script
 go mod edit --replace=github.com/spf13/viper=github.com/Socketsj/quic-go@latest
```

[quic-go](https://github.com/lucas-clemente/quic-go)
