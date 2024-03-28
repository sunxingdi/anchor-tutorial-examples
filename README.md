# Solana Anchor框架官方案例解读

### 工具配套

- Rust版本
- Solana版本
- Anchor版本
  
编译时注意这三个工具版本的配套关系，不配套可能会编译失败。

### 案例构建

克隆项目

```shell
cd /home/solana
git clone https://github.com/coral-xyz/anchor.git
```

安装依赖
```shell
cd /home/solana/anchor/examples/tutorial
yarn install
```

修改Cargo.toml，设置不编译IDL

```shell
打开：/home/solana/anchor/examples/tutorial/basic-0/programs/basic-0/Cargo.toml
删除：idl-build = ["anchor-lang/idl-build"]
增加：no-idl = []
```

安装依赖

```shell
cd /home/solana/anchor/examples/tutorial/basic-0
yarn add @coral-xyz/anchor
```

设置日志打印级别
```shell
打印所有日志
export RUST_LOG=info
```

编译程序
```shell
cd /home/solana/anchor/examples/tutorial/basic-0
anchor build
```

测试程序
```shell
cd /home/solana/anchor/examples/tutorial/basic-0
anchor test
```

查看程序日志
```shell
cat .anchor/program-logs/Fg6PaFpoGXkYsidMpWTK6W2BeZ7FEfcYkg476zPFsLnS.basic_0.log
```

### 案例解读

[案例配置解读](./docs/案例配置解读.md)

[案例0解读](./docs/案例0解读.md)




```shell
```


```shell
```


```shell
```


```shell
```


```shell
```