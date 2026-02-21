# DAO Governance Alpha

A robust framework for decentralized decision-making. This repository provides the essential smart contracts to launch a DAO where token holders control the protocol's treasury and parameters.

## Governance Lifecycle
1. **Proposal:** A token holder submits a proposal (e.g., "Transfer 10 ETH from Treasury").
2. **Voting Delay:** A short period allowing users to delegate or prepare for the vote.
3. **Voting Period:** Users cast votes weighted by their token balance.
4. **Queue & Execute:** Successful proposals enter a Timelock to ensure safety before final execution.



## Key Components
* **Governor Contract:** Handles the logic for counting votes and maintaining proposal states.
* **Governance Token:** An ERC20 token with "snapshots" to prevent double-voting.
* **Timelock Controller:** A security delay mechanism that acts as the "Owner" of the protocol's sensitive functions.

## Security Features
* **Quorum:** Minimum number of votes required for a proposal to be valid.
* **Proposal Threshold:** Minimum tokens required to create a new proposal.
* **Timelock Delay:** Prevents "governance attacks" by giving users time to exit if they disagree with a passed vote.

## License
MIT
