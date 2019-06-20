# 未决交易中继

### 概览

上一章节中，我们要给一笔交易记账的话，必须自己手动进行一次挖矿，才会把交易记录加到一个区块里面去。 这一章节中，我们将会引入未决交易中继的机制。有了这个机制之后，我们要进行一笔交易的时候，就不需要自己动手挖矿，而是将自己的交易发送到我们的区块链网络中去(即中继传递的概念)，由其他节点在挖矿之后，将我们的交易记录加到他们挖出的新的区块中去。其中这些交易就被称之为「未决交易」。一个典型的例子就是，当一个用户想要发起一笔交易(把一定数量的币发送到指定的地址)，他会把这笔交易广播到整个网络，并希望其他矿工把该笔交易放到区块中去。

对于一个加密货币系统来说，这个功能异常的重要。因为这将意味着我们再也不需要因为要进行一笔交易而自己进行挖矿以对交易记录进行保存。这将大大提高效率。 毕竟，如比特币一样，随时着时间转移，挖一个矿是越来越难。 如果我们这些家里没矿(矿机)的用户想跟别人交易一些比特币，还要自己挖个矿，那这个交易就不知道何年何月才能达成了。

为了达到广播到其他节点并进行同步的目的，和第一章节进行区块广播和同步一样，我们需要对「未决交易」也要进行广播。 也就是说，我们的区块链系统现在会包含以下的广播和同步：

- 区块链 (即区块链及包含在区块中的「已决交易」记录)
- 未决交易 (还没有包含在任何区块中的交易)





























