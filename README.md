# luci-app
luci for [luci-app](https://github.com/zznnx/luci-app)

## 使用方法

### 增加feed源

```shell
echo >> feeds.conf.default
echo 'src-git luci_app https://github.com/zznnx/luci-app.git;main' >> feeds.conf.default
./scripts/feeds update luci_app
./scripts/feeds install -a -p luci_app
```

### 集成软件包

```shell
make menuconfig
```

选择软件包
```plain
LuCI --->
3. Applications --->
```

### 构建固件
```shell
make
```
