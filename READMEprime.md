<img src="assets/images/short_banner.png" alt="DeFi Score Banner">

The DeFi Score is a framework for assessing risk in permissionless lending platforms. It's a single, consistently comparable value for measuring protocol risk, based on factors including smart contract risk, collateralization, and liquidity.

We encourage the Ethereum community to evolve the methodology, making it more effective and easier to use.

* Read the detailed [whitepaper](#).
* Join the discussion on [Telegram](https://t.me/dscore).

### Scores
Here are a few scores outputted by the model. We've included reasons why they score the way they do. Note: scores are out of 10.

| Pool           | DeFi Score | Why?                                                        |
|----------------|------------|-------------------------------------------------------------|
| Compound - ETH | 8.5        | Audited, formally verified, highest liquidity in the market |
| Compound - DAI | 5.5        | One of the least liquid compound markets historically       |
| Compound - ZRX | 6.0        | Middling liquidity                                          |
| dYdX - ETH     | 7.0        | Good liquidity, no formal verification                      |
| dYdX - DAI     | 5.2        | Low liquidity                                               |

### Example Implementation
Here is a sample visualization of how a score could be displayed to end users. Although the underlying methodology is complex, it should be simple for a user to understand.

<img src="assets/images/example.png" alt="DeFi Score Example">

### The Components
What goes into calculating the score?

<img src="assets/images/components_sm.png" alt="DeFi Score Components">

<dl>
  <dt>Smart Contract Security (35%)</dt>
  <dd>Errors, bugs and unexpected outcomes in smart contracts can cause real financial harm. These risks can be minimized by proactive code audits and formal verification from reputable security firms.

  Our model assesses code security by looking at three pieces of off-chain but public data:

  1. Audited Code: Has the code been audited by a reputable security team?
  2. Formal Verification: Has the code been formally verified by a reputable security team?
  3. Bounty Program: Does the development team offers a public bug bounty program?

  </dd>
</dl>
<dl>
  <dt>Smart Contract Openness (15%)</dt>
  <dd>Part of the promise of DeFi is that the functionality of smart contracts is completely on-chain, which means they are verifiable and transparent. Developers of DeFi platforms still have the ability to obscure their code in various ways, such as not verifying the bytecode and using off chain oracles processes. Security through obscurity offers weak security guarantees at best, and at worst results in delays in finding critical bugs.</dd>
</dl>

<dl>
  <dt>Financial Risk: Collateral (25%)</dt>
  <dd>Part of the promise of DeFi is that the functionality of smart contracts is completely on-chain, which means they are verifiable and transparent. Developers of DeFi platforms still have the ability to obscure their code in various ways, such as not verifying the bytecode and using off chain oracles processes. Security through obscurity offers weak security guarantees at best, and at worst results in delays in finding critical bugs.</dd>
</dl>

<dl>
  <dt>Financial Risk: Liquidity (10%)</dt>
  <dd>The currently scoped platforms all attempt to incentive liquidity by using dynamic interest rate models which produce varying rates depending on the level of liquidity in each asset pool. However, incentivized liquidity does not mean guaranteed liquidity. The absolute level of liquidity is used instead of the percentage utilization (outstandingDebt/totalAssets) because it has a side effect of also scoring larger pools higher.</dd>
</dl>

<dl>
  <dt>Additional Considerations (15%)</dt>
  <dd>While there are some promising innovations in the DeFi insurance space, none are widespread or mature enough yet. Also, none of these platforms’ development teams are actually decentralized yet and none have been approved by the United States or other nations’ banking/finance regulatory bodies yet.</dd>
</dl>

### Further Reading:
[DeFi Score: Assessing Risk in Permissionless Lending Protocols](#)

### Key Sponsors:
* Jack Clancy

### Additional Sponsors:
* Jordan Lyall
* Todd Murtha
* Thomas Lipari
* [and the rest]

### Community
Join the DeFi Score community on [Telegram](https://t.me/dscore).

### License
<a rel="license" href="http://creativecommons.org/licenses/by-sa/2.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/2.0/80x15.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/2.0/">Creative Commons Attribution-ShareAlike 2.0 Generic License</a>.
