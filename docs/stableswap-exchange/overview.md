<h1> Curve StableSwap Exchange: Overview </h1>

Curve achieves extremely efficient stablecoin trades by implementing the StableSwap invariant, which has significantly lower slippage for stablecoin trades than many other prominent invariants (e.g., constant-product). Note that in this context stablecoins refers to tokens that are stable representations of one another. This includes, for example, USD-pegged stablecoins (like DAI and USDC), but also ETH and sETH (synthetic ETH) or different versions of wrapped BTC. 

!!!pdf "StableSwap Whitepaper"
    For a detailed overview of the StableSwap invariant design, please read the official [whitepaper](../assets/pdf/stableswap-paper.pdf).

A Curve pool is essentially a smart contract that implements the StableSwap invariant and therefore contains the logic for exchanging stable tokens. However, while all Curve pools implement the StableSwap invariant, they may come in different pool flavors.

In its simplest form, a Curve pool is an implementation of the StableSwap invariant with 2 or more tokens, which can be referred to as a plain pool. Alternative and more complex pool flavors include pools with lending functionality, so-called lending pools, as well as metapools, which are pools that allow for the exchange of one or more tokens with the tokens of one or more underlying base pools.

Curve also integrates with Synthetix to offer cross-asset swaps.


<h2>StableSwap-NG</h2>

The Stableswap-NG AMM infrastructure represents a technically enhanced iteration of the previous stableswap implementation.