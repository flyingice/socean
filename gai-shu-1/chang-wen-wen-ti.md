# 常问问题

## Socean是什么？

Socean（SO-shen，与Ocean押韵）是一个运行在Solana区块链上的质押池。

## 质押池是什么？

质押池允许代表用户管理资金池（SOL）并将其委托给一组验证者。质押池向储户发放代币凭证（scnSOL）以代表他们在池子中的份额。

Socean是一个算法质押池，这意味着它通过基于客观数据的透明逻辑作出质押决策。我们打算让Socean在未来变得完全自主，仅仅依靠可独立验证的预言机数据来做决策。

有关更多信息，请参阅Solana基金会关于质押池的[<mark style="color:blue;">官方公告</mark>](https://forums.solana.com/t/stake-pool-manager-faq-and-grant/2168)。

## 为什么我应该通过质押池进行质押？

**解锁质押的全部潜力。**已质押的SOL是不能流通的。相反，质押池凭证代币（代表已质押SOL的份额）是可替代的。质押池凭证代币可让您获得质押奖励，同时用它来借贷和提供流动性--这增加了您的总收益。[此处](defi-an-li.md)跳转了解有关DeFi使用的更多信息。

**减少麻烦同时增加质押多元化。**现今大多数质押者手动委托给一两个验证者。然而，只是跟踪它们就已经足够麻烦，而将质押从一个验证者转移到另一个还需要等到纪元边界。权益池能够动态监控和重新委托，并在此过程中最小化质押奖励的损失。Socean还提供监控工具来跟踪验证者，矿池性能以及质押奖励。

**保护网络。**通过将质押的SOL系统地分散于大量验证节点，质押SOL于质押池中有助于网络去中心化。更加分散的质押分布进而使网络攻击更加困难。

## 为什么我要通过Socean质押？

**公平、透明的委托策略。**我们对[我们的委托策略](https://app.gitbook.com/s/zscfE3PRMybYavzp3Vnn/)进行了很多思考，该策略在促进网络健康的同时为质押者提供最大的年化收益。我们已经在[白皮书](jian-yao-bai-pi-shu.md)中公布了委托策略的全部细节。和其它质押池不同，我们不进行幕后交易，也没有偏向一组特定的验证者：任何验证者都可以被我们的委托算法选择，只要它具备良好性能。

**专业的知识。**我们的团队成员积极为Solana运行环境的核心开发做贡献，充当主网验证节点，并参与各种Solana生态系统项目。我们已经将安全性和易用性功能整合到质押池的[开源实现](https://github.com/solana-labs/solana-program-library/tree/master/stake-pool)中。

我们已和Solana基金会合作数月之久来帮助其开发质押池项目。我们已经获得了基金会的拨款用于开发质押池生态。

**安全的源码实现。**与其它运行自己代码的质押池不同，我们采用Solana基金会的开源参考实现。这确保了我们的质押池通过安全审核，并及时收到漏洞修复和更新。程序可以从源码编译并与[链上版本比对](https://docs.solana.com/cli/deploy-a-program#dumping-a-program-to-a-file)。

**强大的生态系统集成。**我们将发布与Solana上的DeFi生态系统中其它合作伙伴的关键集成。

## 为什么我不该通过Socean质押？

**您想把所有鸡蛋放进一个篮子里。**Socean试图在高年化收益，多元化和去中心化三者间取得平衡。我们始终以提高年化收益为目标，但我们绝不会把所有SOL全部委托给少数几个验证者，或者那些在同一数据中心的验证节点，并以此来换取最后0.1%的年化收益。

**您偏好特定验证节点。**根据算法质押池的定义，Socean会平等对待所有验证节点。我们永远不会与“有信誉的”或者“友好的”验证者进行幕后交易。除了运行节点之外，还有其它方法可以激励验证者和奖励其贡献。如果偏好某个验证者，您可以分配一部分SOL给它，再将余下的质押到Socean或其它质押池。

## 我如何通过Socean质押？

通过Socean质押的最简单方法是直接存入◎SOL。在Socean的网站上[连接您的钱包](https://www.socean.fi)，即刻将◎SOL兑换为SOCN代币。

您还可以在公开市场上交易或者通过自动做市商交换来获得SOCN代币。查阅[通过Socean质押](../jiao-cheng/tong-guo-socean-zhi-ya.md)了解更多详情。

## 我的资金安全吗？

是的。我们采用Solana基金会的[质押池参考程序](https://github.com/solana-labs/solana-program-library)，它部署在生产环境中且接受过多轮审计，反馈和核查。三轮审计由[Kudelski](https://solana.com/SolanaKudelskiStakePoolAudit.pdf)、[Neodyme](https://solana.com/SolanaNeodymeStakePoolAudit.pdf)和[Quantstamp](https://solana.com/SolanaQuantstampStakePoolAudit.pdf)完成。所有问题均被我们或者Solana Labs修复。

我们将安全作为重中之重。您拥有池中SOL代币的非托管份额，它们可以赎回基础SOL。这和指数基金或者交易所交易基金（ETFs）类似。

我们还为[质押池程序](https://github.com/solana-labs/solana-program-library/tree/master/stake-pool)开发了额外的安全及可用性功能，现已被Solana团队采纳，并且充分了解程序以及Solana运行环境的相关细节。

## Socean如何委托我的资金？

Socean通过透明且规范的委托策略分配其资金。我们将资金委托给那些具有良好历史记录、去中心化的（依据地理、司法管辖和数据中心）且不属于[最小安全组](https://medium.com/solana-labs/announcing-the-solana-foundation-delegation-strategy-5bcccf9104ab)的验证节点。

我们将验证节点性能分析和金融与经济理论（均方差分析，期望效用理论）相结合，用以最大化年化收益率，最小化质押奖励差异，并提升网络健康度。有关更多详细信息，请[点击此处](../jiao-cheng/xie-gei-yan-zheng-zhe.md)查阅验证者白皮书。

我们将撰写报告，让社区深入了解我们的数据分析，突出展示验证节点和集群性能的变化趋势，并阐明我们质押分配逻辑的更新。

## 将来会有治理代币吗？

我们仍在开发治理和代币结构。请放心，我们致力于与战略合作伙伴、贡献者和用户分享奖励和控制权。

## 会有空投吗？

我们一直计划奖励早期用户和忠诚质押者。我们已经向Socean的前3000名质押者发放了收藏品（详情请[点击此处](https://medium.com/@soceanfinance/introducing-the-socean-collectibles-program-49f5fe1459ee)），并将持续奖励质押进Socean的用户。

![奖励Socean早期质押者的收藏品](../.gitbook/assets/PathFinder.png)

## 我如何了解Socean的最新进展？

关注我们的社交平台：[Discord](https://discord.com/invite/k8ZcW27bq9)，[Twitter](https://twitter.com/SoceanFinance)，[Medium](https://medium.com/@soceanfinance)。

## Socean收取什么费用？

我们收取一次性存入费用（**0.15%**）、一次性提取费用（**0.3%**）和持续性管理费（**～0.16%每年**）。这些费用可能会有所变化。

Socean团队将在更改费用之前通知所有用户，以便给SOCN持有者足够时间来调整持仓。

质押池程序限制了短时间内改变费用的方式和幅度。比如，提取费用被限制为每个纪元最多增至1.5倍。这确保您有足够的时间在费用重大更改前撤出您的SOL。

将来Socean会完全在链上治理，费用将由多数票决。

## 我是验证者。如何让Socean质押在我这里？

让Socean质押委托给您的最佳方式是始终保持高性能，并且不要集中在某一地理/司法管辖区域或者数据中心。我们不进行幕后交易。

请查看我们的[验证者加入流程](../jiao-cheng/xie-gei-yan-zheng-zhe.md)开始。
