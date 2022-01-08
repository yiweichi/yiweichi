---
sort: 3
---
# 使用手册
## 系统工作原理图

![DOTC.TRADE](/assets/images/trade.png)

>如上图所示，图片中央位置为在区块链上的智能合约，当卖家要卖出虚拟币资产（比如USDT)的时候，他需要发布订单，每一个订单有一个唯一的编号。从1累加上去。订单号不会重复。

>卖家发布订单的时候，实际上dotc.trade的DApp客户端程序会申请用户的钱包向智能合约支付待售出的资产（比如USDT)，以基础币支付区块链网络的Gas费，以及以基础币支付的违约金。

>买家在订单上点击购买，那么，买家需要以基础币支付的Gas费，以及卖家设定的违约金，

>Gas费是由区块链的矿工赚取。

## 钱包安装与配置

>DOTC支持多种区块链,比如[哈耶克链](https://hayek.link),[币安智能链](https://binance.org),[欧易的OKEx Chain(OEC)链](https://www.okex.com/oec),这些区块链都是与以太坊链类似,都支持EVM虚拟机的区块链.这类区块链都支持智能合约的运行.我们之所以目前并不支持以太坊链,原因其实只有一个,那就是以太坊链的交易Gas太过高昂.交易双方做一笔DOTC交易,支付的Gas费接近300美元.我想,这是我们的用户难以承受的费用.所以,我们才选择将DOTC部署在其他与以太坊EVM虚拟机完全兼容的其他区块链上.

>你如果要使用DOTC服务,首先你需要准备一个钱包。我们推荐大家使用 ![MetaMask](https://metamask.io/images/favicon.png)MetaMask钱包,<a href="https://metamask.io" target="_blank">点击这里即可进入MetaMask的官方网站</a>还有[imToken钱包](https://token.im/).或者,你已经使用的其他支持以太坊的钱包.

>如果您在中国大陆地区，有些钱包你可能需要翻墙上网才能下载.如果您使用的是苹果系统,那么,在您的应用商店中您可能找不到对应的钱包软件.因为这类软件在中国大陆地区都被屏蔽.解决方法,推荐您在淘宝网或者其他网站购买一个美国或者香港的苹果ID.价格一般在5元人民币左右.或者,您可以更改您的apple ID国家地区为非中国大陆地区.如何更改你苹果Apple ID的国家地区，<a href="https://support.apple.com/zh-cn/HT201389" target="_blank">请点这里阅读相关说明</a>

### 钱包安装

#### 苹果手机上安装MetaMask钱包 

>登录您的美国或者香港的苹果ID在您的手机或者iPad,打开苹果应用商店中搜索Metamask或者imToken,即可下载安装相应的钱包.

#### 安卓手机上安装MetaMask钱包

>安卓手机下载，如果你手机可以直接访问Google Play应用商店，则你可以直接在其中搜索到MetaMask或者imToken并且安装。但是，在中国大陆的绝大部分手机，都无法访问Google Play应用商店。此时，你可以访问如下网站下载apk文件进行安装。![avatar](https://metamask.io/images/favicon.png) [点这里进入下载页面](https://bafybeifunqckmw3qmhfeejeixkzzt5e3cd5ju2jwrajskyrtawwnx6uhda.ipfs.infura-ipfs.io/io.metamask_2021-08-30.apk)

#### 安卓手机上安装imToken钱包

>对于imToken钱包,他们官网上有APK文件下载.您可以用浏览器点这里访问[imToken官网](https://token.im/)直接下载安装.

#### Chrome浏览器上安装MetaMask钱包

>如果您使用的是windows系统,最为推荐的方式，是在您的电脑上下载安装MetaMask钱包。MetaMask钱包在windows,Linux，Mac电脑上都可以安装，但是，它不是一个独立可以运行的程序。而是一个浏览器的插件应用。首先，我们强烈推荐你在电脑上安装Chrome浏览器.[点击这里进入Chrome下载安装教程](https://support.google.com/chrome/answer/95346?hl=zh-Hans&co=GENIE.Platform%3DDesktop)

>在你安装好你的Chrome浏览器之后，启动你的Chrome浏览器，在chrome浏览器地址栏输入 chrome://extensions/ 进入扩展程序界面，搜索 MetaMask，按提示安装好MetaMask钱包并启用之后。你就可以在Chrome浏览器的右上角看到MetaMask钱包的图标。点击进入即可设置你的钱包。


### 配置你的钱包

#### 保护好你的12(或者24)个英文单词

>当你安装好了你的钱包之后，你首先要做的是按照提示创建你的钱包。需要注意的是，此时请准备好一张纸与一支笔，你需要记录下12或者24个英文单词。这些英文单词是由MetaMask(imToken)钱包随机生成的。这是生成你钱包私钥的机密信息。

>请务必不要用手机拍照来保存在手机或者电子邮箱等不安全的地方。因为，一旦他人知晓你的这12(或24)个英文单词，那么，你的钱包里的所有资产将可以被转走。

>如果你把写下这12或者24个英文单词的纸条保存好。即便你的电脑或者手机丢失。你也可以通过这12(或24)个英文单词恢复你的钱包私钥。从而取回你钱包里的所有资产。

#### 添加HAYEK网络

>此时，你已经安装好了你的M钱包，同时，你也创建了你的钱包账户。

>在你的钱包主界面的上方位置，你会看到有一串 0x 开头字母数字串，你点击它，即可把你的钱包地址复制下来。粘贴到其他任何软件中去。你会发现你粘贴出来的字符串类似  0x3CEfe2a38fA388B6e25C2D3350eB8fB3A31ed0E8 这样一串0x开头的字符串.这就是你的钱包地址。这个地址可以向任何人公开，而不会让你的钱包里的资产被盗窃。

>他人向你的钱包转账发送虚拟币，也需要知道您的这个钱包地址。钱包地址全球唯一。不会有其他人的钱包地址和你相同。

>你已经有了钱包地址，MetaMask钱包已经连接到了以太坊的区块链上。但是，你如果要使用哈耶克链或者其他链，那么，你需要在你的MetaMask钱包软件菜单中依次点击: “设置”->“网络"->"添加网络"。然后，按照下图的方式填写。再点击“保存”按钮。完成之后，您的钱包即可使用哈耶克链了。

![avatar](/imgs/1.jpg)

您可以复制以下参数填写到您MetaMask网络配置中去。

网络名称
```key
HAYEK
``` 
RPC URL
```key
https://rpc.hayek.link
``` 
链ID
```key
1000
``` 
符号
```key
HYK
``` 
区块链浏览器URL
```key
https://explorer.hayek.link
``` 

#### 添加Binance Smart Chain 币安链

>添加方法与添加哈耶克链网络一样,只是使用以下参数

网络名称
```key
Binance Smart Chain Mainnet
``` 
RPC URL
```key
https://bsc-dataseed1.binance.org
``` 
链ID
```key
56
``` 
符号
```key
BNB
``` 
区块链浏览器URL
```key
https://bscscan.com
``` 

#### 添加OKEx Chain(OEC)网络

>添加方法与添加哈耶克链网络一样,只是使用以下参数

网络名称
```key
OKExChain Mainnet
``` 
RPC URL
```key
https://exchainrpc.okex.org
``` 
链ID
```key
66
``` 
符号
```key
OKT
``` 
区块链浏览器URL
```key
https://www.oklink.com/okexchain
``` 

#### 在imToken中添加节点

>按照前文的方法安装好imToken钱包之后,按顺序点击: 我->使用设置->节点设置->ETHEREUM, 点右上角的+号,选择 "自定义" 填写哈耶克网的的网络名称:HAYEK

>RPC地址:https://rpc.hayek.link

>链ID(Chain ID):1000

>符号(Symbol):HYK

>区块浏览器:https://explorer.hayek.link

>如果添加币安或者OKEx等其他链,则使用前文中的参数即可.


## 切换到相应的区块链

>imToken钱包：依次点击左下的“钱包”，点击最上方中央位置的链名称"Ethereum Mainnet",选择对应的链名称。

>Metamask钱包：在钱包主界面，点击最上方的“Ethereum Main Network”,在下拉列表中选择相应的链名称即可。

>其他钱包：比如Token　Pocket钱包，操作方法非常类似。你只要找到钱包界面的Ethererum字样，基本上就可以找到你要切换的链名称。

>如果找不到相应的链名称，则请查看前文添加相应的区块链进钱包。

## 获得基础币

>DOTC系统是一个去中心化的链上担保交易系统，买家卖家所有的操作，都需要支付Gas费。所以，你在使用DOTC之前，你必须在你的钱包中有足够的基础币。基础币就是在区块链上可以用来支付矿工Gas费的币种。以太坊的基础币是以太币ETH,币安智能链的基础币是BNB，OKEx链的基础币是OKT，哈耶克连的基础币是HYK

### 哈耶克链（HAYEK)(推荐)

>哈耶克链：哈耶克链的基础币是HYK，在哈耶克链上，获取基础币是最为容易的。您只需要在钱包里面访问DOTC.TRADE，过几分钟，系统就会自动往你的钱包地址上赠送少量HYK币。足够您完成购买USDT的操作。

>在钱包中查看USDT：在哈耶克链上，USDT的合约地址为：0xa5E265Bf313b24476dA9681D61bDbdC03c66F271  ，在您的钱包里面，您需要复制该地址手工添加USDT代币进你的钱包。

>添加USDT代币进imToken钱包:依次点击“钱包”，右边中间位置的+号按钮，自定义代币，粘贴合约地址，保存。

>添加USDT代币进Metamask钱包:在钱包主界面，点击下方的“添加代币”，自定义代币，粘贴USDT智能合约地址进代币地址，点击添加代币按钮。

### 币安链（Biance smart chain)
>币安链（Biance smart chain)：币安链的基础币是BNB，类似于以太坊上的以太币ETH，在币安链上，卖家和买家都必须先购买一定数量的BNB币。

>获得BNB的方法有很多，但是，最简单的方法是到币安交易所购买BNB并且提现到自己钱包。[点这里进入币安交易所官网](https://www.binance.com/)

>提现BNB：在选择主网络的时候，请选择Biance Smart Chain(BEP20)

>提现USDT:作为卖家，您有可能也在币安交易所购买USDT，再在DOTC平台卖出。以赚取差价。此时，在选择主网络的时候，您也需要选择BEP20字样的选项。

>在钱包中查看USDT：在币安链上，USDT的合约地址为：0x55d398326f99059fF775485246999027B3197955，在某些钱包里面，您可能需要复制该地址手工添加USDT代币进你的钱包。

>添加USDT代币进imToken钱包:依次点击“钱包”，右边中间位置的+号按钮，自定义代币，粘贴合约地址，保存。

>添加USDT代币进Metamask钱包:在钱包主界面，点击下方的“添加代币”，自定义代币，粘贴USDT智能合约地址进代币地址，点击添加代币按钮。

### OK链OKEx Chain (OEC)

>OK链OKEx Chain (OEC)：OK链的基础币是OKT，在OK链上，卖家和买家都必须先购买一定数量的OKT币。

>获得OKT的方法有很多，但是，最简单的方法是到欧易交易所购买OKT并且提现到自己钱包。[点这里进入欧易交易所官网](https://www.okex.com)

>提现OKT：在选择主网络的时候，提现网络请选择：OKT-OEC

>提现USDT:作为卖家，您有可能也在欧易交易所购买USDT，再在DOTC平台卖出。以赚取差价。此时，在选择提现网络的时候，你需要选择USDT-OEC

>在钱包中查看USDT：在OK链上，USDT的合约地址为：0x382bb369d343125bfb2117af9c149795c6c65c50，在某些钱包里面，您可能需要复制该地址手工添加USDT代币进你的钱包。

>添加USDT代币进imToken钱包:依次点击“钱包”，右边中间位置的+号按钮，自定义代币，粘贴合约地址，保存。

>添加USDT代币进Metamask钱包:在钱包主界面，点击下方的“添加代币”，自定义代币，粘贴USDT智能合约地址进代币地址，点击添加代币按钮。

## 钱包内访问DOTC.TRADE

>不管是买入还是卖出操作，首先，你需要打开您的钱包，使用钱包中的DApp浏览器来访问https://dotc.trade应用程序。

>imToken钱包：依次点击最下方的浏览，在最上方的输入框中输入 https://dotc.trade，点击“进入DOTC交易”

>Metamast钱包：依次点左上角的三条横线，点击“浏览器”，在输入框中输入“https://dotc.trade",回车或者确认进入DOTC官网，点击“进入DOTC交易“。

>其他钱包操作基本类似。

>操作成功后，您会看到一个粉红色背景的界面，右上角会出现您钱包的地址。证明您已经成功使用钱包登录进了DOTC系统。如果在右上角看不到您的钱包地址，则可能是您没有选择正确的区块链网路。

## 卖出操作

>进入DOTC交易之后，依次点击“我的订单”，“发布订单”，即可进入发布订单界面。

![卖出](/assets/images/publish.jpg)

### 订单

>订单是DOTC系统的基本概念，订单由卖家发布。每一个订单包括订单编号，所售代币（比如ＵＳＤＴ），数量，单价，货币（法定货币），卖家地址，买家地址，卖家违约金，买家违约金，第三方法院，订单描述信息等几个部分。

>订单一旦发布，即意味着已经冻结了卖家的两部分资产：待售资产（比如USDT）以及违约金(一般是基础币，比如ETH,BNB,OKT,HYK)

>订单与订单之间的资产相互隔离：即便是同一个卖家的不同订单，资产都是相互独立的。法院在判决的时候，不能在判决A订单的时候却处置B订单的资产。

#### 订单编号

>每一个订单,有一个唯一的数字编号.卖家在发布订单的时候，智能合约会自动给每一个订单分配一个唯一的订单编号。不需要卖家填写。

#### 数量，代币，价格，货币

>数量是您准备卖出的加密货币的资产的数量，这个数量可以是0或者比0更大的数字。可以有几位小数。

>选择代币：点击此按钮，即可弹出一个下拉列表框，显示当前DOTC系统所在链支持的虚拟币以及您当前的余额。比如，我们可以选择USDT

>单价：请在单价输入框中输入您要求买家支付的单价。可以有4位小数。

>选择货币：点击此按钮，会弹出一个列表框，让您选择买家需要支付给您的货币种类。比如，我们可以选择CNY人民币


#### 卖家违约金

>卖家违约金是指如果卖家在交易过程中,违反双方约定,(比如,收到买家付款却不及时在平台确认付款导致买家延迟取得所买加密货币),那么,买家可以发起争议(起诉),经过举证和仲裁人员调查核实,链上法院则会做出对违约方不利的判决.

>比如,如果买家已经付款,但是卖家不及时确认.那么,将会判决将该笔订单中卖家所缴纳的卖家违约金赔偿给买家.

>违约金并不包括在交易标的资产(比如USDT)之中.违约金只能采用当前链的基础币支付（比如HYK，BNB，OKT等

>在设置您的卖家违约金的时候，请确保您的钱包中有大于您所设金额的基础币。

>一般来说，卖家违约金要设置的比第三方法院所收取的诉讼费更高的金额。否则，买家不会接受您的订单。因为，如果卖家待买家付款后，却拖延不确认订单。买家必须支付诉讼费来起诉卖家。如果卖家的违约金低于诉讼费。买家即便通过法院判决拿走卖家所有的违约金，也不能弥补诉讼费损失。所以，我们建议卖家要设置一个高于所选法院诉讼费的违约金。才能取信于买家。

>卖家违约金越高,则代表交易对买家来说越安全.

#### 买家违约金

>买家违约金基本与卖家违约金类似,如果买家要锁定卖家的订单.那么,买家必须要支付卖家所设定的买家违约金.后续交易中,如果买家违约.(比如,超过约定时间没有付款),那么,卖家同样可以发其争议(起诉),要求第三方法院判决将买家的违约金赔偿给卖家.这样设计的目的,是为了防止没有诚意的买家恶意锁定卖家订单,却不完成交易.

>设置低于法院诉讼费的买家违约金对卖家具有一定的风险，一旦买家锁定订单却不付款，那么，卖家必须支付诉讼费起诉买家。即便法院判决将买家的所有违约金支付给卖家，也无法弥补卖家诉讼费损失。

>但是，买家违约金也不宜设置的过高，这对销售不利。我们需要考虑到，即便卖家设置一个较低的违约金，没有诚意的买家，是不会支付这笔违约金来锁定卖家订单的。因为，买家不履约付款，这笔违约金是一定会被法院判决支付给卖家的，同时买家也不可能获得所售的资产（比如USDT)。

#### 选择法院

>点击“选择法院”，会弹出一个所有法院的列表框。同时，还会显示该法院的诉讼费，以及网址，请在其中选择一个买卖双方都信任的法院。一旦您选择了这家法院，那么，后续交易如果出现纠纷，则只能联系这家法院的服务人员进行判决。

>订单中的法院，实际上是一个智能合约的地址。

#### 订单描述信息

>如果把整个订单理解为一份交易合同，那么，订单描述信息则是该合同的正文部分。在这部分所填写的信息必须谨慎填写。并且严格履行。

>订单描述信息分很多类型，点击“选择信息类型”，会看到一个当前所支持的所有信息类型的列表。需要注意的是，有些信息是明文公开的，比如telegram，微信，支付宝,QQ，银行卡号等等。如果你填写了这些信息，则代表您的这些信息在区块链上是完全公开的，任何人都可以看到。

>私密微信，银行卡现金存款，加密合同等几个信息，属于加密信息。这些信息的原文部分并不直接保存在区块链上，而是将原文进行了hash运算，再将hash值保存在区块链上。所以，没有任何第三方可以知晓这些信息的原文内容。绝对保护了卖家的隐私。但是，如果您的订单中添加了这一类信息中的一个，那么，买家在锁定您的订单的时候预先和您取得联系，获取这些信息的原文填写进订单购买界面，才能成功购买。

>正常情况下，一个卖单必须包含一个公开的联系方式，如果您不想使用任何实名制的联系方式，我们建议您填写一个telegram或者电子邮件，作为买家与您联系的方式。

>选择一个信息类型之后，您必须填写这个类型对应的信息原文。不要忘记了，您还必须点击按钮“添加信息”，才能让该信息添加进订单描述信息。

##### 加密合同

>加密合同属于加密信息. 其实,它就是一段文字.长度不限，比如,典型的秘密合同条款,可能如下:"1,买家必须将款项在3天之内通过SWIFT汇款到 汇丰银行 454353453453 账号,收款人:XXX,收款地址:XXXX".

>当卖家发布订单的时候添加一项加密合同.加密合同的内容,不会公开在区块链上.公开在区块链上仅仅是加密合同文本内容的Hash编码.如果交易双方不对外透露,没有人可以根据这个公开的Hash编码还原出交易双方的合同内容.这样,就确保了交易的安全性与隐私性. 带有加密合同的订单,买家需要先联系卖家,索取加密合同原文,输入正确的加密合同原文之后,才可以完成锁定订单的操作.这一个过程,就代表着买家已经知晓并且同意了卖家所起草的合同.对于加密合同,交易双方都应该妥善保管好加密合同原文.以备交易发生纠纷的时候,向仲裁人员提供加密合同原文.仲裁人员才可以依据加密合同原文经过Hash运算之后取得hash值，再与链上订单中的对应hash值比对。如果一致，则确定为正确的合同原文。

>请务必注意，卖家是所有加密信息的起草者，卖家必须妥善保管这些加密信息的原文，如果发生纠纷，卖家和买家都不能提供正确的加密信息原文。那么，法院将会做出对卖家不利的判决。

##### 微信与私密微信

>微信与私密微信，都是填写微信账号，而不能填写该微信所绑定的手机号或者QQ号。如果卖家填写不符合要求，一旦发生纠纷，法院会做出对卖家不利的判决。

>微信与私密微信的区别是，微信是公开的，而私密微信，是加密的，链上只保存了微信账号的hash值。

##### 银行卡现金存款

>银行卡现金存款属于加密信息，卖家填写该项信息，意味着买家向卖家付款的时候，必须采用ATM机现金存款方式。详细操作请点击这里。

##### 其他信息类型

>对于其他信息类型，其含义与类型名称一致。不再赘述。

>卖家所填写的所有可以用于付款的联系方式，都是合法的支付方式，卖家不得拒绝。例如，卖家既填写了微信，也填写了支付宝，还填写了银行卡。则意味着买家可以选择其中任意一种付款方式向卖家付款。

#### 批准

>当您第一次卖出某种虚拟币的时候，那么，在发布订单的最下方会出现“批准”或者“授权”按钮。这是因为需要将您的这种虚拟币授权给DOTC智能合约以完成后续交易。按提示完成操作之后，再过几分钟。该按钮会变为：“发布我的订单”

#### 发布我的订单

>如果上面所有的信息都完整正确的填写了。那么，最下方的按钮会变为“发布我的订单”，点击它，按照提示完成钱包操作。在过十几秒钟到几十秒钟，您的订单将会被所有的买家看到。

>因为区块链是每过几秒钟到15秒钟产生一个新区块。所以，您在发布订单之后，不要着急重复点击发布我的订单按钮。过个几十秒钟之后，您点击发布卖单左边的向左箭头，回到DOTC主界面。再点击 “我的订单”，“我卖出的订单”，就可以看到您所有的发布的卖单。点击对应订单，即可看到订单详情。

## 买入操作

>进入DOTC交易之后，依次点击“在售订单”，“选择订单过滤条件”，即可进入订单过滤条件选择界面。

![卖出](/assets/images/filter.jpg)

### 在售代币

>在售代币是你准备购买的代币.缺省状态下，在售代币是USDT，当然，您点击USDT，即可更换查找其他待售代币。

### 付款货币

>付款货币是你准备用来付款的法定货币。缺省状态下，是CNY，您也可以点击CNY来切换成其他付款货币。

### 价格

>价格缺省是设置为从0到无穷大，意思就是，搜索出所有价格的卖单。您可以修改这两个参数，缩小您的价格范围。精准的找到您所需要的卖单。

### 数量

>数量代表着订单的所售代币的数量，缺省是设置为从0到无穷大，意思就是，搜索出所有数量的卖单。您可以修改这两个参数，缩小您的数量的范围。精准的找到您所需要的卖单。

### 最少买家违约金以及最多买家违约金

>这两项，是为了方便您查找符合您要求的违约金订单。

### 设置订单过滤条件

>点击此按钮之后，会列出符合您过滤条件的订单。点击订单，即可看到订单详情

### 订单详情以及购买操作

>在售订单列表显示了每一个订单的所售代币，数量，单价。点击订单，该订单即会展开，显示出该订单的详细情况。

### 法院

>在订单详情中有一个项目叫法院，如果该项显示为“未经验证的法院”，则表示该订单所设置的法院未经DOTC官方验证，存在交易风险。尽量不要购买。

### 订单描述信息与联系卖家

>一般来说，每一个订单上面都会有卖家的联系方式。请使用对应的联系方式与卖家取得联系。

>有些订单，卖家会设置加密信息，此时，买家必须联系卖家，并且向卖家询问这些加密信息的原文，复制粘贴进订单详情相应的输入框中去，如果卖家给出的加密信息原文与链上的Hash值一致，那么，在订单详情的最下方，会出现“购买”按钮。

### 购买按钮

>点击“购买”按钮之前，请确保您的钱包里有足够的基础币（比如OKT,BNB,HYK等币），您钱包里的这些基础币的余额，必须高于订单的买家违约金金额。

>点击“购买”按钮，则代表您已经与卖家达成了交易。同时，会启动钱包操作，请求钱包向链上担保交易智能合约支付违约金，购买操作一旦在链上操作完成，您必须进入付款环节。如果不付款，那么，卖家可以起诉您，显然，您在这种情况下属于违约。链上法院大概率会判决将您的违约金赔偿给卖家。

### 我买入的订单

>同一个卖单，有可能同时有几个人点击“购买”，那么，您是否成功的购买，则需要您点击“我的订单”，“我买入的订单”。此时，您可以看到您已经买入的订单列表。出现在“我买入的订单”列表中的订单，才是需要您付款的订单。没有出现在此列表中的订单，代表尚未在链上锁定。您不能付款。

>注意：即便出现在了“我买入的订单”之中，您还需要等待十分钟之后再付款，因为，有些链可能存在区块重组的情况。如果出现区块重组，而您的购买交易没有重新打包进后续区块。那么，您支付的款项面临巨大风险。

### 付款

>在“我买入的订单”中列出来的订单，再等待十几分钟之后，您可以开始付款了。但是，请务必只按照订单描述中所列出的方式付款给对应的账号。如果卖家在和您沟通的时候，要求您向其他付款账号支付货款，而这个付款方式并未出现在订单描述信息中。那么，请拒绝付款。坚持按照订单描述中所指定的收款账号或者微信号付款。

## 查看自己的买入和卖出订单

>依次点击“我的订单”，“我买入的订单”，即可查看到自己当前已经买入的订单。已经结束的订单，不在此显示。

>依次点击“我的订单”，“我卖出的订单”，即可查看到自己当前正在卖出的订单。已经结束的订单，不在此显示。

## 取消订单

>卖家发布的卖单，显示在“我卖出的订单”之中。如果尚未有人点击购买，则可以取消订单。在我卖出的订单中，找到要取消的订单，点击它展开，就可以看到取消按钮。点击取消按钮，即可取消订单。成功取消的订单，您所支付的USDT和违约金，退回到您钱包。

## 确认订单

>只有卖家需要确认订单。在“我卖出的订单”列表中，找到您需要确认的订单。请确保检查您已经收到了卖家在银行，支付宝，微信给您的付款。再点击 “确认”。订单一旦确认操作成功。那么，订单上的USDT会支付给买家。双方支付的违约金退回各自钱包。订单结束。

>订单一旦确认，交易已经完成。您的在售资产则无法追回。所以，请谨慎操作。

## 卖家起诉买家

>进入“我的订单”，“我卖出的订单”，找到您需要发起起诉的订单，点击它，展开订单详情。从订单被买家点击购买的时间，到订单可以发起起诉，大概需要经过半小时时间。过了半小时之后，才可以发起起诉。此时，订单详情页会出现发起起诉的按钮。点击它，请确保您钱包里有足够的基础币支付诉讼费。等待半小时才可以发起起诉的原因是避免滥诉。

>成功发起起诉之后，请积极与链上法院的工作人员联系举证。配合链上法院工作人员的调查要求。

>如果卖家的订单中设置了加密信息，比如：加密微信，加密合同等非公开信息。则卖家需要提供这些加密信息的原文给法院工作人员。法院工作人员通过hash函数，计算出您所提供的原文对应的hash值，再与链上订单中的hash值比对。如果一致，则证明原文相符。

>如果卖家不能提供正确的加密信息原文，则可能面临败诉风险。

>卖家配合调查：链上法院工作人员为了确保判决公正，可能会要求卖家提供收款银行卡的查询密码。以检查您的银行卡上是否有该笔收款到账。此时，卖家应该在网上银行中设置一个临时的查询密码，提交给链上法院工作人员使用。待其查询完毕，卖家再修改查询密码。

>为了您的资金安全，链上法院工作人员不会向您索取支付密码。请不要提供支付密码给链上法院工作人员。

>在链上法院工作人员调查期间，卖家可以把卡上资金全部转移到其他卡上。

>不配合链上法院工作人员的查询要求的，可能会面临败诉风险。

>对于微信和支付宝支付方式，卖家可能需要提供账号登录密码给法院工作人员以备查询。在此期间，请转走您账户上的所有资产。

## 买家起诉卖家

>进入“我的订单”，“我买入的订单”，找到您需要发起起诉的订单，点击它，展开订单详情。从订单被买家点击购买的时间，到订单可以发起起诉，大概需要经过半小时时间。过了半小时之后，才可以发起起诉。此时，订单详情页会出现发起起诉的按钮。点击它，请确保您钱包里有足够的基础币支付诉讼费。等待半小时才可以发起起诉的原因是避免滥诉。

>成功发起起诉之后，请积极与链上法院的工作人员联系举证。配合链上法院工作人员的调查要求。

## 链上法院判决与执行

>链上法院在对买卖双方调查取证之后，会做出判决。判决书的内容并不像现实中的法院那么冗长繁琐，而仅仅是包括两个0到100的数字x,y。x是代表卖家取得所售资产的百分比。y代表卖家取得该订单双方所缴纳的违约金总和的百分比。举个例子，判决书的内容是10,20，那么，意味着该法院认为卖家败诉，该订单上的所售资产（比如100USDT)只有10%归卖家，也就是10USDT。同时，假设该订单卖家缴纳了10个OKT的违约金，买家缴纳了5个OKT的违约金。违约金总和就是10+5=15个OKT币。卖家取得该订单的违约金总和15个OKT币的20%,也就是说，卖家可以拿到3个OKT币。

>判决书只载明了卖家拿到的两部分资产的百分比。剩余部分，就是归买家所有。也就是说，法院无论怎么做判决。都只能将订单上的资产分配给卖家或者买家。在有些担保交易平台，比如电报群担保交易，很有可能担保人侵吞买卖双方的保证金。在DOTC平台，这种情况就不可能发生。这是由公开的智能合约保障的。

>链上法院只能在买卖任何一方发起起诉之后，才会做出判决。与现实法院不同的是，链上法院没有执行权。链上法院是第三方智能合约。它不能调用DOTC的核心交易合约(trading合约)来直接分配资产。要分配订单上的资产，必须由买卖双方中的任何一方来发起判决执行操作。这时，DOTC核心交易合约（trading合约）才会读取相应订单编号的判决书。然后根据判决书的分配方案来分配订单中冻结的双方资产。将资产转移到买卖双方的钱包地址。

>如果买卖双方都不愿意执行法院判决，那么，买卖双方还可以继续协商解决。协商不成，可以要求法院重新制作判决书（这可能需要额外付费）

>也就是说，链上法院的判决书，仅仅是链上法院所认为的公正分配方案。并不具有强制性。是否执行判决，还是取决于买卖双方。

>链上法院是一个商业机构，它出售一种服务，那就是公正的判决服务。而且，这种服务是收费的。诉讼费是法院的唯一利润来源。DOTC系统以及我们正在开发的其他系统，都会涉及到链上法院服务。这些法院是多样的，各种不同专业的法院，各种不同语言的法院，他们会相互竞争。有信用的，清廉的，判决公正的，判决效率高，收费低廉的法院，最终将会在市场获胜。而那些胡乱判决，收取贿赂，收费高昂，效率低下的法院，最终将会被市场所淘汰。这正是我们的司法市场化的理念。

>我们有理由相信，链上法院为了自己的生存，在做判决的时候，一定会优先尊重买卖双方的合同本意与合同执行的实际情况来做出公正的判决。如果买卖双方的合同本意违反所在国的法律，链上法院的判决没有理由会去违背买卖双方的合同本意而去遵守当地法律。所以，买卖双方在使用本系统的时候，必须要考虑到这一点。也就是说，在链上法院的眼里，买卖双方的合同本意，高于当地法律。当然，这也不是100%是这样，最终链上法院的法官如何判决，是将当地法律凌驾在买卖双方合同之上还是之下，都取决于法官的自由意志。

>我们要相信，法官为了自己的利益，一定会选择对他口碑最有利的判决原则。

### 执行判决

>不管是哪一方发起的起诉，只要法院做出了判决。买卖双方都可以执行判决。

>买家执行判决：点“我的订单”，“我买入的订单”，找到已经有判决结果的订单。点击按钮“执行判决”。

>卖家执行判决：点“我的订单”，“我卖出的订单”，找到已经有判决结果的订单。点击按钮“执行判决”

>判决执行成功之后，订单上的资产立即按照判决书的分配方案支付到双方的钱包。

>执行判决仅仅需要执行方支付区块链的Gas费。而不需要支付其他费用。

## ATM机现金存款交易

>当前在中国大陆，由于电信诈骗非常猖獗。公安机关在大力打击电信诈骗。根据媒体报道，电信诈骗犯罪分子一般躲藏在东南亚国家，比如印尼，缅甸，柬埔寨等国家。电信诈骗团伙向农村一些文化层次较低的人士购买银行卡用于收取诈骗款。电信诈骗受害人将款项转移到这些人士的银行卡上之后，电信诈骗犯罪分子一般会通过购买USDT的方式来将赃款洗白或者转移到境外。如果你在欧易，币安等平台出售您的USDT，则很有可能会遇到这种诈骗来的资金。受害人报警之后，警方会根据资金流向瞬间找到您的收款银行卡。当然，首先是您的银行卡会被冻结。后续调查过程中，如果发现您参与了帮助电信诈骗团伙洗钱犯罪，则您会受到刑事处罚。遭遇牢狱之灾。

>ATM机现金存款买卖USDT，买家向卖家支付的是现金，现金是不具名的，银行系统无法将赃款现金与卖家的收款银行卡关联起来。所以，不会出现冻卡的情况。

>此外，电信诈骗犯罪分子如果将诈骗所得取成了现金，他何必要再买USDT呢？他可以在中国境内随便买成别的东西。

>ATM机上都有摄像头，电信诈骗犯罪分子是不可能冒险在中国境内的取款机上存取款的。如果电信诈骗犯罪分子的银行卡已经在境外，那么，电信诈骗犯罪分子一般会在境外通过银联系统取出当地货币。也就不存在拿现金来购买USDT的行为了。

>综上，我们推荐合法的卖家或者买家，通过ATM机现金存款交易来买卖USDT。避免冻卡，避免牢狱之灾。

>我们最近发现，在网上有一个叫汇旺的电报担保交易群中，有超过几万人在其中帮助电信诈骗团伙洗钱。我提醒读者一定要谨慎参与。您赚的那点小钱，很可能要付出牢狱之灾作为代价。

>虚拟币交易市场被电信诈骗团伙的猖獗洗钱活动所污染，导致正常的非刑事犯罪的自愿的虚拟币买卖活动也常常遭遇冻卡。此时，我们强烈推荐合法虚拟币买家和卖家，使用我们最新的ATM机现金存款交易服务。

>从本质上来讲，ATM机现金存款交易，其担保交易方式与DOTC的其他交易方式并无本质区别。首先也是卖家发布订单，将待售的USDT等资产以及违约金转移到DOTC的核心交易合约（trading合约）,买家支付违约金锁定卖家订单，买家找到一个具有存款功能的ATM机上，向卖家指定的银行卡上存现金。卖家收到买家的存款即确认放款给买家，各自违约金退回各自钱包。交易完成。具体流程与注意事项如下。

### 卖家发布ATM机现金存款交易卖单

>发布ATM机现金存款交易卖单就是普通的发布卖单操作。唯一的区别就是，卖家需要在订单描述信息中添加一项"银行卡现金存款”,如下图所示。内容为“中国银行，赵长鹏，卡号：466477......”

![发布ATM卖单](/assets/images/atm/publishatm.jpg)

>需要注意的是，银行卡现金存款 这个描述项目是加密的。链上并不会保存原文。所以，卖家还需要添加自己的电报telegram账号，以便买家向您索取加密信息原文填写进去之后，才可以点击“购买”按钮。

>因为ATM机现金存款单笔金额不能超过2万元人民币，存款面额必须是100元。所以，卖家在发布卖单的时候，必须要仔细设置数量和价格，使得买家需要支付的金额少于2万元人民币，并且是100元的整数倍。

>因为网上银行的详单中并没有详细的ATM存款信息，链上法院在取证的时候，只能依据存款金额来判断买家是否存款。所以，在同一天内，卖家的同一个银行卡上不能有其他相同金额的进账。所以，请谨慎计算好交易金额，同一张卡同一天不能有相同的进账金额。如果出现相同的金额进账，则视同买家已经付款。

>在“银行卡现金存款”项目中，卖家必须写明：银行名称，卖家姓名，卡号。

>请不要忘记了点击“添加信息”按钮。否则，该项信息并不会加入到订单描述信息中去。

>确保您的这张卡开通了手机银行业务。因为，后续操作，还需要卖家启用手机银行来扫描二维码。

### 买家点击购买

>买家购买的操作与前面提到的购买操作并无差别。仅仅需要点击所选订单的“购买”按钮。

>买家收到卖家在电报（或者其他联系方式）上发来的“银行卡现金存款”项目的原文，填写进订单相应位置进行核验。核验成功之后才会显示“购买”按钮，买家此时务必将卖家发来的信息截屏保存。因为，后续存款操作必须要仔细核对卖家姓名和卡号是否一致。

### 买家付款

>当点击“购买”按钮操作完成之后，务必检查“我的订单”，“我买入的订单”中是否已经有该项订单，如果有，则代表“购买”操作成功

>等待至少10分钟后，您需要准备相应金额的百元现金，最好多准备一点，因为，有些ATM机可能会拒收某些残破的百元人民币。

>准备好足够现金之后，带上您的手机，到您附近的对应银行的具有存款功能的ATM机上进行如下操作。

>注意：卖家的收款银行是哪家银行，买家只能到相应银行的ATM机上操作。跨行操作是不支持的。

#### 向卖家拍照发送ATM机存款二维码

>到具有存款功能的ATM机上之后，你可以找到类似无卡存款，或者二维码存款这样的选项。在中国银行的存款ATM机上，您可以看到下图界面。

![中国银行](/assets/images/atm/1.jpg)

>在ATM机上点选“扫码存取/存折取现/密码汇款取现”按钮，出现以下界面

![中国银行](/assets/images/atm/2.jpg)

>点选“扫码存款”按钮，看到以下二维码。

![中国银行](/assets/images/atm/3.jpg)

>拿出您的手机，清晰的拍下这个二维码，通过“电报”或者QQ等联系方式发送给卖家。卖家收到您的二维码之后，需要打开自己的手机银行，进入“扫一扫”功能，扫描您的二维码，并选择对应的银行卡号。此时，您的ATM机上会出现以下界面。

![中国银行](/assets/images/atm/4.jpg)

>买家需要仔细核对显示的姓名部分除*字以外的部分是否与订单描述信息中的姓名一致。如果一致，继续操作。如果不一致，不要继续操作。如果核对一致之后，此时请一次性放入现金到存款机入钞口。如果有不被存款机接受的钞票，请更换一张。操作完成之后，您会看到如下界面

![中国银行](/assets/images/atm/5.jpg)

>此时，存款机上显示了完整的卖家银行账号，请买家务必认证核对是否与订单描述信息中经过核验的账号是否完全一致。如果不一致，则点击取消操作。您的钞票会被退回。

>请务必注意：如果卖家通过电报或者QQ等联系方式发送了多个银行账号或者卡号。请只认准在订单购买页面经过了核对一致的哪个账号。如果卖家在电报或者QQ聊天工具软件里告诉您他换了账号。请务必不要存款。因为，后续法院做判决的时候，只会检查链上核对过的哪个银行账户上是否有进账。聊天工具里发过来的其他银行账号不能作为付款证据。

>核对无误之后，在存款机上点击“确认”之后，别忘了选择打印凭条按钮。您会得到以下纸质的存款凭条。

>请把存款凭条拍照发送给卖家。以便卖家核对。

>请保存好此存款凭条直至交易结束。一旦有纠纷，此凭条需要提交到链上法院作为付款证据。

![中国银行](/assets/images/atm/6.jpg)

### 卖家操作

>卖家在收到买家发来的ATM存款机上的二维码之后，请尽快打开您的手机银行，进入“扫一扫”功能，扫描二维码。按提示选择对应的银行卡号。确认之后，买家的ATM存款机屏幕上会显示您的姓名的后面部分。以及完整的银行账号或者卡号。

>收到买家付款之后，卖家还需要进入“我的订单”，“我卖出的订单”中找到对应订单，点击“确认我已经收到买家付款”。超过不合理的时间确认放款，可能会遭到买家起诉。
