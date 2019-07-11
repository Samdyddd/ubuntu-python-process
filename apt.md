# apt 命令详解

ubuntu 16.04将apt命令引入，apt = apt-get, apt-cache和apt-config集合

apt-cache和apt-get是apt包的管理工具，他们根据/etc/apt/sources.list里的软件源地址列表搜索目标软件、并通过维护本地软件吧列表来安装和卸载软件。

## apt-cache
```
// 搜索软件包
sudo apt-cache search package_name
// 或
// 模糊搜索sof*开头的软件包
sudo apt-cache search sof*

```

```
// 查看软件包信息
sudo apt-cache show package_name
```

```
// 软件包依赖关系
sudo apt-cache show depends package_name

```

```
// 查看每个软件包简要信息（巨多）
sudo apt-cache dump
```

## apt-get

```
// 安装软件
sudo apt-get install package_name
```

```
// 更新已安装的软件包
sudo apt-get upgrade
```

```
// 更新软件包列表
sudo apt-get update
```

```
// 卸载一个软件包但是保留相关配置文件
sudo apt-get remove package_name
// 卸载但是同时删除配置文件
sudo apt-get -purge remove package_name
```

```
// 删除软件包备份
sudo apt-get clean
```







