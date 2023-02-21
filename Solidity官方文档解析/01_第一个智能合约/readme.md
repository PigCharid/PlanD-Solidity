先构建自己的第一个智能合约程序

## 1、开发工具：Remix

[官网](https://remix.ethereum.org/)----（需要翻墙）

目前使用进行Solidity开发框架和工具也有很多了，关于智能合约的开发工具，后续会整了一个专门的笔记，我们先采用remix进行开发，他是一个在线的IDE，只要在网站上打开就可以正常使用了。

remix使用非常简单，新手也没有任何的挑战，简单介绍一下这个工具

[官方的手册文档](https://remix-ide.readthedocs.io/en/latest/)

![image-20230221105751411](/Users/pigcharid/Library/Application Support/typora-user-images/image-20230221105751411.png)

**1：切换文件、搜索、编译和部署**

**2：文件区**

**3：代码块**

**4：运行结果**



## 2、第一个智能合约

可以先把文件区里面的内容全部删除，或者直接在contracts目录下，创建一个`HelloSolidity.sol`

```solidity
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;
contract HelloWeb3{
    string public _string = "Hello Solidity!";
}
```

这就是我们第一个智能合约代码，我们定义了一个string类型的状态变量，并且定义了字符串"Hello Solidity!"



## 3、编译和部署

### 3.1编译

通过Ctrl+s直接编译，可以通过页面上操作，建议直接开启自动编译

![image-20230221110911504](/Users/pigcharid/Library/Application Support/typora-user-images/image-20230221110911504.png)



### 3.2部署

在默认情况下，remix会用JS虚拟机来模拟以太坊链，运行智能合约，类似在浏览器里跑一条测试链。并且remix会分配几个测试账户给你，每个里面有100 ETH（测试代币），可劲儿用。你点Deploy（黄色按钮），就可以部署咱们写好的合约了。

![image-20230221111733867](/Users/pigcharid/Library/Application Support/typora-user-images/image-20230221111733867.png)

部署完毕以后，”HelloSolidity！“就会被存到链上，我们也能成功获取该状态变量的值。

## 4、总结

这一小节，我们完成自己的一个智能合约程序，关于remix相关操作不熟练的同学可以自己再多去使用学习一下，下面我们就开始慢慢按照官网文档的内容开始Solidity的学习！