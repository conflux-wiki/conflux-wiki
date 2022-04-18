# 开发资源

## 常用

-   [Conflux对接Q&A](https://shimo.im/docs/KlkKVPllv9T2bZqd)
-   [Conflux-faqs合集](https://github.com/conflux-fans/conflux-faqs)
-   [Conflux公众号技术文章&教程&视频&漫画目录](https://shimo.im/sheets/913JVX0avGt61j3E/wIyyF)
-   [Conflux UI库](https://github.com/Conflux-Chain/design-resource-lab)

## 开发说明

-   [Conflux的 CVM 和 EVM 虚拟机层的主要区别](https://juejin.im/post/6854573220268343309)
-   当前版本Conflux 默认有反重入机制。重入指的是一个合约在调用其他合约时，其他合约又直接或间接地调用了这个合约。比如合约 A 调用合约 B, 在合约 B 执行期间，又调用了合约 A, 则构成了重入调用。重入调用是一些 Defi 攻击的原因。但是，一些逻辑正常的合约也会有重入调用。比如说，合约 A 调用闪电贷合约，闪电贷调用合约 A 的 callback 函数，就构成重入调用。
-   Conflux 默认开启反重入机制，即重入调用发生后，所有写操作将被禁止，包括：向账本写入数据 （SSTORE 指令），发起有转账的合约调用，生成 event


## CIP

-   [Conflux 改进提案](https://www.github.com/Conflux-Chain/CIPs)
-   [Conflux CIP介绍](https://juejin.cn/post/6914956571432730637/)

## 技术论坛

-   [Conflux社区论坛](https://forum.conflux.fun)


## 节点与RPC

-   [Conflux GPU 挖矿教程文档（v1.1.2）](https://forum.conflux.fun/t/topic/5131)
-   [Conflux网络中"奇奇怪怪“的Node](https://juejin.cn/post/6854573217655291917)
-   [Conflux RPC 和以太坊 RPC的 区别](https://juejin.im/post/6876328114461343757/)
-   [Conflux RPC 地址列表(仅供开发测试使用，不保证可用性)](https://github.com/conflux-fans/conflux-rpc-endpoints)
-   [如何配置自己节点的rpc端口和数据存放路径](https://forum.conflux.fun/t/topic/5147)
-   [Conflux网络上首款类Infura API访问服务限时公测中](https://mp.weixin.qq.com/s/S_3BllKl_1ahTDA2v1gEAQ)


## Conflux开发者文档

-   [官网](https://developer.conflux-chain.org/)
-   [js-conflux-sdk](https://github.com/Conflux-Chain/js-conflux-sdk)
-   [Conflux js-sdk与以太坊web3. js区别](https://juejin.im/post/6876311074602221582)
-   [如何在Conflux网络中使用js-conflux-sdk来构建一个简单的DApp](https://juejin.im/post/6845166890768138248)
-   [onflux 智能合约开发体验(js-conflux-sdk@0.13.4)](https://juejin.im/post/6844904176720281607)
-   [java-conflux-sdk](https://github.com/Conflux-Chain/java-conflux-sdk)
-   [go-conflux-sdk](https://github.com/Conflux-Chain/go-conflux-sdk)
-   [Conflux SDK 使用体验收集](https://forum.conflux.fun/t/topic/225)
-   **[Conflux V2硬分叉开发介绍](https://developer.confluxnetwork.org/v2-hardfork/hydra_overview)**
-   **[Conflux espace介绍：完全兼容EVM](https://developer.confluxnetwork.org/v2-hardfork/hydra_overview#conflux-espace)**


## Dex开发文档

-   [开发文档](https://conflux-dev.github.io/conflux-dex-docs/shuttleflow/)
-   [Conflux 进阶课 | DEX 双子协议：链上结算 BoomFlow & 链下撮合 MatchFlow](https://mp.weixin.qq.com/s/L7zFOIWkCtDz8DI1jKvvQg)
-   [Conflux Shuttleflow文档](https://conflux-dev.github.io/conflux-dex-docs/shuttleflow/)
-   [使用ShuttleFlow实现ETH和cETH之间的转换](https://forum.conflux.fun/t/topic/5130)
-   [如何使用 ShuttleFlow 实现灵活跨链](https://forum.conflux.fun/t/topic/5478)


## 内置合约

-   [内置合约](https://github.com/Conflux-Chain/conflux-rust/edit/master/internal_contract/README.md)
-   [Conflux 内置合约功能详细介绍](https://juejin.im/post/6876330619798814728)
-   [Conflux的存储抵押机制](https://juejin.im/post/6855551378123653127)
-   [新项目如何高效启动？Conflux 代付机制了解一下](https://juejin.cn/post/6904212662629236749/)

## 开发工具指南

-   [Conflux与以太坊合约开发工具区别](https://juejin.im/post/6876310280733720583)
-   [Conflux 开发教程 | 使用 IDE 开发 DApp 的实战操作指南](https://forum.conflux.fun/t/topic/1680/)
-   [Conflux Studio 开发 DApp 教程](https://juejin.cn/post/6862234416941858830)
-   [Conflux Truffle 使用完全指南](https://juejin.cn/post/6862239117934067726)
-   [Conflux-remix（Conflux社区自行开发）](http://remix.conflux.work/)
-   [使用Remix玩转Conflux上的智能合约](https://github.com/conflux-dao-toc/conflux-remix-plugin/blob/main/conflux-guide.md)