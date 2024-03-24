# kitex_rpc

快速生成rpc,依赖字节跳动的 hz.  支持redis,mysql,pulsar,naocs,elastic 等常用中间件

案例地址 [案例 洁骏汽车服务有限公司](http://www.ch123.com.cn/ "洁骏汽车服务有限公司")

使用方式  xxx/xxx 换成自己的项目地址
go mod init github.com/xxx/xxx

https://www.cloudwego.io/zh/docs/kitex/getting-started/prerequisite/

go install github.com/cloudwego/thriftgo@latest

go install github.com/cloudwego/kitex/tool/cmd/kitex@latest

protobuf: https://github.com/protocolbuffers/protobuf/releases  windows版本放到gopath目录下

kitex -type protobuf  -template-dir layout -I idl/ -module github.com/xxx/xxx  idl/hello.proto

go mod tidy

github.com/jhump/protoreflect v1.14.1 需要这个版本

github.com/apache/thrift v0.13.0 需要这个版本

修改 conf/test/app.yml 里的配置

go run ./

设置proto默认路径的方法
![2RTTA3XF@STW6GVJJMQ) 3V](https://github.com/flyerxp/hertz_web/assets/52146821/d60a167a-6530-444c-af64-7ea36f742d94)
