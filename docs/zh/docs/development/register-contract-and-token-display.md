# 如何在Scan上注册合约和代币展示



## 部署合约

在Scan上将合约展示上链，第一步是将合约部署到Conflux。
打开Scan的[合约部署界面](https://confluxscan.io/contract-deployment)

- 连接 Conflux Portal 钱包

![image.png](./figure/ad36030021d14115b7fdd4f0b3f4cc53~tplv-k3u1fbpfcp-watermark.image)

- 将[ConfluxStudio](https://conflux-wiki.github.io/conflux-wiki/development/tools/#ide)，[cfxtruffle](https://conflux-wiki.github.io/conflux-wiki/development/tools/#conflux-truffle)，[remix](https://conflux-wiki.github.io/conflux-wiki/development/tools/#conflux-remix) 编译后的 .json 文件导入（import JSON file），或手动拷贝 bytecode （必填）和 ABI （选填）。

![image.png](./figure/75b4cb31dd4b4a409c787eb479b2d19d~tplv-k3u1fbpfcp-watermark.image)

!!! note

​	注：bytecode为必填项，ABI选填。

请注意下方的提示：

1. 合同部署即通过发送交易向 Conflux 网络发布合约代码。在部署合约之前，请确保您的帐户中 CFX 余额充足。
2. 仅支持 ConfluxStudio，cfxtruffle ，remix 编译后的 .json 文件导入；同时支持手动拷贝 bytecode （必填）和 ABI （选填）。
3. 暂不支持输入构造函数参数。
4. 您可以点击页面右上角的账户，在您的账户交易历史中查看合约部署详情。



![image.png](./figure/1db9345206ca4d46b8df52bceab08293~tplv-k3u1fbpfcp-watermark.image)

- 点击提交，并签名交易。

![image.png](./figure/eeddd04da2cb4a49900c84b8d8100bc2~tplv-k3u1fbpfcp-watermark.image)

- 在ConfluxScan的交易信息中，接收方地址即为创建的合约地址。

![image.png](./figure/64ec720c3f8f4d659e9d151638bcefcc~tplv-k3u1fbpfcp-watermark.image)



## 合约注册

部署完合约之后，此时的Scan上仍旧无法查看该合约，需要注册合约才能将合约的名字展示在Scan上。

- 点击链接打开[合约注册](https://confluxscan.io/contract)界面

![image.png](./figure/e9b8151714a6486bbc5ffa1a0cc73441~tplv-k3u1fbpfcp-watermark.image)

在合约注册的信息栏填写合约地址和合约姓名。

- 合约姓名应当和部署合约时写在合约里的一致；合约地址应当为Conflux地址。

![image.png](./figure/0d5b02f3d6f04028bdceb8aa10490d1a~tplv-k3u1fbpfcp-watermark.image)

- 右侧上传窗口支持合约图标的上传和代币图标的上传。

![image.png](./figure/2bf6d3219ee940a687e57914c34d6551~tplv-k3u1fbpfcp-watermark.image)

!!! note

​	注：非CRC20的合约不可以上传代币图标



- 只有合约的拥有者和管理者可以上传图标，其他人上传图标会弹出提示。

![image.png](./figure/679ca1064901425787571b00182e4ac6~tplv-k3u1fbpfcp-watermark.image)



## 代币展示

~~项目方如果想在Scan上展示代币，需要联系工作人员（cike@confluxnetwork.org）申请审核。~~**但目前的scan已不需要审核即可展示代币相关信息，开发者只需要按照CRC20标准开发并部署代币合约即可获得展示。**

![image.png](./figure/21a76dc4c65f4a099a2fd88f2a6b3189~tplv-k3u1fbpfcp-watermark.image)