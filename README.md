
## 介绍

该项目主要是通过实践的方法来加深学习和理解区块链的相关原理知识，覆盖区块链的所有核心功能：
> * 网络节点通讯
> * 挖矿
> * 钱包
> * 交易和验证
> * 共识机制
> * 链式结构

涉及的如下知识点：

> * 密码学基础
> * 数字证书
> * Merkle树和SPV机制
> * Kademlia算法、P2P技术
> * 区块链共识机制
> * 比特币交易原理
> * 区块链网络设计

## 项目组成
迷你区块链客户端

## 项目环境
安装必要文件：
环境：*Anaconda2+python2*

安装必要库函数：使用pip安装
```
pip install gunicorn
pip install configparser
pip install rsa
pip install constant
```
运行期间如果报库函数缺失的错误，安装对应的库

### **Step1：启动迷你区块链客户端（模拟3个节点）**
测试demo中一共使用3个节点，大家可以根据需要自己调节。

打开终端，windows下使用Anaconda Promote，运行代码：
```
python run.py -p 5000 &
python run.py -p 5001 &
python run.py -p 5002 &
```
### **Step2：模拟交易**
```
python simulation_test.py

```
### **Step3：迷你区块链的json api接口调用**
区块链客户端实现了json api，可以直接通过api调用来获取各个节点之间的信息
