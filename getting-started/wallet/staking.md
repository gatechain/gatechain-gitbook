# Staking

Centralized mining is a crucial factor that must be considered in the staking process. Although various decentralized staking protocols have emerged in the market over the past few years, a small number of validators and staking service providers still control most of the network. Fundamentally, if independent validators offer a relatively poor user experience, we will see a large amount of network participation occurring through external staking services—as they lower the cognitive barrier for end users. Therefore, GateChain's design process strives to avoid this issue.

Most POS models require accounts participating in consensus to stake a certain amount of assets. Accounts with higher stake amounts are more likely to be selected into the Validators Set. The consensus process only occurs among validators, and block rewards are distributed proportionally according to the staked amounts. Moreover, staked assets cannot be freely transferred or moved. This design has three main drawbacks:

1. The qualification for participating in block consensus becomes a bidding target. Accounts with fewer assets cannot become independent validators through staking. If they want to participate in consensus and receive block rewards, they can only do so by delegating to accounts with more assets or professional POS mining institutions.

2. Network centralization issues. Since the validator set is determined by staked asset rankings and remains fixed for a period, network attacks or physical node failures can affect consensus achievement and network security.

3. Scalability issues. As the mainnet expands and the amount of staking gradually increases, the number of validators cannot increase linearly, as this would affect block consensus speed.

GateChain fundamentally abandons the staking approach. Any account can become a consensus account and participate in block consensus to receive rewards by just paying a regular transaction fee.

1. Accounts with fewer assets need not worry, as the probability of being selected for the committee only relates to consensus weight and loyalty coefficient. A properly configured node can participate in consensus and earn rewards without asset delegation.

2. Since the committee is randomly elected during each consensus round (guaranteed by VRF algorithm), hackers cannot launch attacks in such a short time. When a node goes offline, it only affects that node's consensus and won't significantly impact network operation. (Through the consensus account heartbeat mechanism, the network can quickly restore consensus speed after large accounts go offline)

3. Since the committee size is part of the mainnet consensus, as the network expands, the committee size can still maintain a reasonable range, ensuring quick consensus achievement.
