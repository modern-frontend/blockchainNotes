# ICO DApp 要解决什么问题？
## 更好的 ICO — DAICO
> 任何 ICO 都面临团队不负责任或者项目仅仅是一个骗局的风险，任何投票系统都面临51%攻击的问题、贿赂选票和其他博弈上的缺陷。在 DAICO 中，这些风险都得到了最小化。Dai 可以替代以太作为项目募集资金的代币。
>DAICO 合约由一个需要募集资金的开发团队发布。DAICO 合约由“贡献模式（Contribution Mode）” 开始，指定一个机制：每个人都可以将以太贡献到合约当中，并得到相应的代币。可以是有封顶的售卖、无封顶的售卖、荷兰式拍卖、互动式的代币发行、KYC的动态个人封顶售卖或者团队选择的任何一种机制。当贡献阶段结束后，就无法再继续贡献以太，初始的代币余额将设定，之后代币可以被交易。
>在贡献阶段结束后，合约有一个主要状态变量：tap (单位: wei/sec)，初始值为零。tap 决定每秒钟开发团队可以从合约中提现的数量。
同时，还有机制可以让代币持有者通过投票获得解决方案。有两种解决方案：
### 提高 tap 值
### 永久地自毁合约(将合约进入 withdraw 模式，剩余的以太可以按比例地提现给代币持有者)
>两种方案都可以通过仲裁的多数票决启动。注意，无法通过投票降低 tap 值。所有者可以自愿降低 tap 值，但是他们无法单方面提高 tap 值。
这样做的目的是，投票者可以给开发团队一个合理而不太高的每月预算，假如团队不断证明其能力，预算可以通过投票提高。如果投票者对团队的开发进展不满意，他们可以完全关闭 DAICO 并取回自己的资金。
 
## 博弈安全性
>任何投票系统都面临51%攻击的问题、贿赂选票和其他博弈上的缺陷。任何ICO都面临团队不负责任或者项目仅仅是一个骗局的风险。在 DAICO 中，这些风险都得到了最小化，除非开发者和投票者联合才能产生破坏。

1. 51%攻击以提高 tap - 诚实开发者可以自发降低 tap，或者不提现多余的资金。
2. 开发者滥用资金而不专注项目进展 - 投票者可以不那么快的提高 tap 值，即使 tap 值提高了，投票者也可以随时自毁合约
3. 51%攻击以自毁合约 - 诚实开发者可以再发布一个 DAICO

>注意，两种潜在的51%攻击：1) 将资金发送到攻击者选择的第三方 2) 降低 tap 值将资金永远锁在合约里，在系统中都是不被允许的。

### 可做的改变

1. 将 tap 值设为 usd/sec (每秒多少美元) 或者其他位价
2. 将 Dai 作为募集资金而不是以太
3. 尝试除了简单投票之外的其他机制


