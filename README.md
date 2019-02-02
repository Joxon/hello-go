# 简介 / Overview

[Offical docs](https://golang.org/doc/)

The Go programming language is an open source project to make programmers more productive.

Go is expressive, concise, clean, and efficient. Its **concurrency** mechanisms make it easy to write programs that get the most out of multicore and networked machines, while its novel type system enables flexible and modular program construction. Go compiles quickly to machine code yet has the convenience of **garbage collection** and the power of **run-time reflection**. It's a fast, **statically typed, compiled language** that feels like a dynamically typed, interpreted language.

## 亮点 / Highlights

- 并行性支持
- 垃圾回收
- 运行时反射
- 静态类型
- 编译型语言

# 配置 / Configurations

- Windows 10
- [Go MSI Installer](https://golang.org/dl/)
- VS Code

## 安装 Go 语言插件 / Installing the Go Extension

成功安装 Go 插件后，安装第三方工具成功的日志：

```
Installing 9 tools at C:\Users\User\go\bin
gocode
go-outline
go-symbols
guru
gorename
gocode-gomod
godef-gomod
goreturns
golint

Installing github.com/mdempsky/gocode SUCCEEDED
Installing github.com/ramya-rao-a/go-outline SUCCEEDED
Installing github.com/acroca/go-symbols SUCCEEDED
Installing golang.org/x/tools/cmd/guru SUCCEEDED
Installing golang.org/x/tools/cmd/gorename SUCCEEDED
Installing github.com/stamblerre/gocode SUCCEEDED
Installing github.com/ianthehat/godef SUCCEEDED
Installing github.com/sqs/goreturns SUCCEEDED
Installing golang.org/x/lint/golint SUCCEEDED

All tools successfully installed. You're ready to Go :).
```

若遇到`FAILED`提示，一般是因为墙的干扰。此处可将 VSCode 中`Settings -> Http: Proxy`设置为`http://127.0.0.1:1080`，利用本地代理服务（前提是开启了相关服务）完成安装。

## 环境变量 / Env

- GOPATH：Go 项目的工作目录，默认为 C:\Users\Username\go。源代码/src、生成的二进制文件/bin，都放在这个目录。一般在系统变量中属于用户变量，可以根据自己的喜好放置在自定义的路径，但是一般只有一个。在 VSCode 里面可以设置`"go.inferGopath": true`来自动推断工作路径，但是一旦切换到别的工作路径，编译好的第三方工具需要重新下载源码并编译，也可从旧目录中复制过去。
- GOROOT：Go 语言的工具集目录，默认是 C:\Go。

# 运行 / Run

`go run hello.go` 或 安装[Code Runner](https://marketplace.visualstudio.com/items?itemName=formulahendry.code-runner)后右键点击`Run Code`。

# 教程 / Tours

- [English Version](https://tour.golang.org/welcome/1)
- [中文版](https://tour.go-zh.org/welcome/1)
