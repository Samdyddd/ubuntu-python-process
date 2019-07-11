# ubuntu-python-process
linux ubuntu配置过程


1. ubuntu大多自带python2 和python3, 
```
// 查看python版本，默认是python2；
python -V

```

切换python3为默认的版本；
```
sudo update-alternatives --install /usr/bin/python python /usr/bin/python2 100

sudo update-alternatives --install /usr/bin/python python /usr/bin/python3 150

```

在安装pip3前更新软件

```
sudo apt update

// 安装pip3
sudo apt install python3-pip
// 查看版本
pip3 --version

```

构建python模块所需的开发软件包
```
// build-essential: ubuntu缺省，并没有提供c/c++的编译环境，该包提供了编译c/c++所需的所有依赖包；
// python3-dev: linux发行版通常会把类库的头文件和相关的pkg-config分拆成一个单独的xxx-dev包，当需要安装一个源外的python类库，而这个类库内含需要编译调用的python api的c/c++文件；
// Python3-setuptools: 
// 使用sudo apt search查看是否已有以下软件包，没有请按照；
sudo apt install build-essential python3-dev python3-setuptools

```

