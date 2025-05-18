# Sui Staking Smart Contract

 This project implements a robust staking mechanism on the Sui blockchain, enabling users to stake their SUI tokens and earn rewards over a specified duration.
## Overview
- RewardState: Tracks reward-related parameters such as duration, finish time, and reward rate.

- UserState: Maintains individual user staking information, including balances and rewards.

Treasury: Holds the total staked SUI tokens and manages reward distribution.
## Features
- Secure Staking Mechanism: Users can stake SUI tokens to earn rewards.

- Reward Distribution: Implements a reward distribution system based on staking duration and amount.

- User State Management: Tracks individual user stakes, rewards, and balances.

- Treasury Management: Manages the pool of staked tokens and distributes rewards accordingly.

- Admin Controls: Allows administrators to set reward durations and amounts.

##  Usage
- Staking Tokens:
Users can stake their SUI tokens by invoking the stake function, which updates their UserState and the global Treasury.
GitHub

- Claiming Rewards:
After the reward duration, users can claim their rewards using the claim_rewards function, which calculates and transfers the appropriate amount based on their stake.
GitHub

- Unstaking Tokens:
Users can unstake their tokens at any time by calling the unstake function, which updates their UserState and the Treasury.


##  Security Considerations
- Access Control: Only authorized administrators can set reward durations and amounts.

- Safe Math Operations: All calculations are performed using safe math to prevent overflows.

- Audit: It's recommended to perform a thorough audit before deploying to the mainnet.
