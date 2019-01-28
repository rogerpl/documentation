
### 使用预构建二进制安装包

基于 Go 语言，我们提供了通用的本体客户端安装程序，你可以点击[这里](https://github.com/ontio/ontology/releases)下载。

当然，你也可以通过 curl 命令获取最新的客户端。

```shell
curl https://dev.ont.io/ontology_install | sh
```

### 使用源码编译

此外，你也可以从源码开始构建你的本体客户端。

- 获取源码

```shell
go get github.com/ontio/ontology
```

- 使用包管理工具 `glide` 获取依赖

```shell
cd $GOPATH/src/github.com/ontio/ontology
glide install
```

- 编译源码

```shell
make all
```

源码成功编译后会生成两个可以执行程序：

- ontology：本体客户端。
- sigsvr：签名服务器。