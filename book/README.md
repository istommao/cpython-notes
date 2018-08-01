# Introduction


> CPython学习笔记

https://github.com/istommao/cpython-notes

## 资源
- http://pgbovine.net/cpython-internals.htm
- https://github.com/rainyear/CPython-Internals-Lecture-Notes
- http://woodrat.xyz/2017/06/21/CPython%E6%BA%90%E7%A0%81%E9%98%85%E8%AF%BB%E7%AC%94%E8%AE%B0%281%29
- https://python.freelycode.com/contribution/detail/1034

## 源码安装

`代码clone`
```bash
# 如果未安装git
yum install git

git clone https://github.com/python/cpython.git
cd cpython
git checkout v3.7.0
```

`编译前系统库安装`
```bash
# gcc make
yum install gcc make

# zlib
yum install zlib-devel

# 3.7版本需要一个新的包libffi-devel
yum install libffi-devel

# sqlite安装
yum install sqlite-devel

# readline安装
yum install readline-devel

# openssl安装
yum install openssl-devel

# tk安装
yum install tk-devel
```

`编译安装`

```bash
# 查看configure可选项
./configure --help

# 最小化安装

./configure --without-PACKAGE

make install
```
